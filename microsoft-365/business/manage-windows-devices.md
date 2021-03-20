---
title: Povolení spravování zařízení s Windows 10 připojených k doméně microsoftem 365 pro firmy
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Zjistěte, jak povolit Microsoft 365 k ochraně místních zařízení s Windows 10 připojených ke službě Active Directory v několika krocích.
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913188"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Povolení spravování zařízení s Windows 10 připojených k doméně pomocí Microsoft 365 Business Premium

Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránil vaše zařízení s Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Pokud chcete nastavit tuto ochranu, můžete implementovat hybridní **zařízení připojená ke službě Azure AD.** Tato zařízení jsou připojená k místní službě Active Directory i k azure active directory.

Toto video popisuje postup, jak to nastavit pro nejběžnější scénář, který je také podrobně popsaný v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Než začnete, proveďte následující kroky:
- Synchronizujte uživatele s Azure AD s Azure AD Connect.
- Dokončete synchronizaci organizační jednotky Azure AD Connect.
- Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence na Microsoft 365 Business Premium.

Postup [najdete v tématu Synchronizace uživatelů](manage-domain-users.md) domény s Microsoftem.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Ověření autority MDM v Intune

Přejděte na [Endpoint Manager a](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) na stránce Microsoft Intune vyberte Registrace zařízení a potom na stránce **Přehled** zkontrolujte, že autorita **MDM** je **Intune**.

- Pokud **má autorita MDM** **hodnotu Žádná,** klikněte na autoritu **MDM a** nastavte ji na **Intune.**
- Pokud je autoritou **MDM** Microsoft Office  **365,** přejděte na Zařízení zaregistrovaná zařízení a pomocí dialogového okna Přidat autoritu MDM vpravo přidejte autoritu Intune MDM (dialogové okno Přidat autoritu MDM je dostupné jenom v případě, že je autorita MDM nastavená na Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Ověřte, jestli je azure AD povolená pro připojení k počítačům

- Přejděte do Centra pro správu a v seznamu Centra pro správu vyberte Azure Active Directory (vyberte Zobrazit vše, pokud <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> Azure Active Directory  **není** viditelný). 
- V **Centru pro správu Azure Active Directory** přejděte na Azure Active **Directory** , zvolte **Zařízení a** pak Nastavení **zařízení**.
- Ověření,**že se uživatelé smí připojit k azure AD, je** povolené 
    1. Pokud chcete povolit všechny uživatele, nastavte na **Vše**.
    2. Pokud chcete povolit konkrétní uživatele, nastavte **vybranou** možnost tak, aby povolte určitou skupinu uživatelů.
        - Přidejte požadované uživatele domény synchronizované ve službě Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)
        - Pokud **chcete pro tuto skupinu** zabezpečení povolit rozsah uživatelů MDM, zvolte Vybrat skupiny.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Ověřte, jestli je pro MDM povolené Azure AD.

- Přejděte do Centra pro správu a vyberte Správa koncových bodů t (vyberte Zobrazit vše, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> pokud Endpoint **Manager** není viditelný)  
- V Centru **pro správu Microsoft Endpoint Manageru** přejděte na Zařízení **s**  >    >  **Windows – automatická**  >  **registrace**.
- Ověřte, jestli je povolený obor uživatele MDM.

    1. Pokud chcete zaregistrovat všechny  počítače, nastavte na Vše tak, aby se automaticky zaregistrovaly všechny uživatelské počítače, které jsou připojené k Azure AD, a nové počítače, když uživatelé přidávají pracovní účet do Windows.
    2. Pokud chcete **zaregistrovat** počítače určité skupiny uživatelů, nastavte možnost Některé.
        -  Přidejte požadované uživatele domény synchronizované ve službě Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)
        -  Pokud **chcete pro tuto skupinu** zabezpečení povolit rozsah uživatelů MDM, zvolte Vybrat skupiny.

## <a name="4-create-the-required-resources"></a>4. Vytvoření požadovaných zdrojů 

Provádění požadovaných úkolů pro konfiguraci hybridního připojení [k Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) se zjednodušil pomocí rutiny [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) která se nachází v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Když tuto rutinu vyvoláte, vytvoří a nakonfiguruje požadovaný spojovací bod služby a zásady skupiny.

Tento modul můžete nainstalovat tak, že z instance PowerShellu vyjádříte toto:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Doporučujeme nainstalovat tento modul na Windows Server se službou Azure AD Connect.

Pokud chcete vytvořit požadovaný spojovací bod služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Při provádění tohoto úkolu budete potřebovat přihlašovací údaje globálního správce Microsoftu 365 Business Premium. Až budete připravení vytvořit zdroje, vyvolat následující:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

První příkaz vytvoří spojení s cloudem Microsoftu a po zobrazení výzvy zadejte přihlašovací údaje globálního správce Microsoftu 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Propojení Zásady skupiny

1. V Zásady skupiny Management Console (GPMC) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad* skupiny.
2. Vyberte zásadu vytvořenou ve výše uvedeném kroku a klikněte na **OK.**

## <a name="get-the-latest-administrative-templates"></a>Získání nejnovějších šablon pro správu

Pokud nevidíte zásadu Povolit automatickou registraci **MDM** pomocí výchozích přihlašovacích údajů Azure AD , může to být proto, že nemáte admx nainstalovaný pro Windows 10, verzi 1803 nebo novější. Pokud chcete tento problém vyřešit, postupujte takto (Poznámka: nejnovější mdm.admx je zpětně kompatibilní):

1.  Stáhnout: [Šablony pro správu (.admx) pro Windows 10 – aktualizace z října 2020 (20H2).](https://www.microsoft.com/download/102157)
2.  Nainstalujte balíček na řadič domény.
3.  Přejděte do složky **C:\Program Files (x86)\Microsoft Zásady skupiny\Windows 10. října 2020 Update (20H2)** v závislosti na verzi Šablony pro správu.
4.  **Přejmenujte složku Definice** zásad ve výše uvedené cestě na **PolicyDefinitions**.
5.  Zkopírujte **složku PolicyDefinitions** do sdílené složky SYSVOL ve výchozím nastavení umístěnou ve složce **C:\Windows\SYSVOL\domain\Policies**. 
    -   Pokud máte v plánu používat centrální úložiště zásad pro celou doménu, přidejte tam obsah PolicyDefinitions.
6.  V případě, že máte několik řadičů domény, počkejte, až se funkce SYSVOL replikuje, aby byly zásady dostupné. Tento postup bude fungovat i pro všechny budoucí verze šablon pro správu.

V tomto okamžiku byste měli mít možnost zobrazit zásadu Povolit automatickou registraci **MDM pomocí výchozích přihlašovacích údajů Azure AD.**