---
title: Jak povolit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím Microsoftu 365 pro firmy
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
description: Zjistěte, jak povolit Microsoft 365 chránit místní zařízení s Windows 10 připojená ke službě Active Directory v pouhých několika krocích.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407072"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Jak povolit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím služby Microsoft 365 Business Premium

Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránila vaše zařízení s Windows 10, a přitom udržovat přístup k místním prostředkům, které vyžadují místní ověřování.
K nastavení této ochrany můžete implementovat hybridní zařízení připojená **k Azure AD.** Tato zařízení jsou připojená k vaší místní službě Active Directory a k Azure Active Directory.

Toto video popisuje kroky nastavení pro nejběžnější scénář, který je podrobně popsaný v krocích popsaných v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Než začnete, proveďte tyto kroky:
- Synchronizace uživatelů s Azure AD pomocí Azure AD Connect.
- Dokončete synchronizaci organizační jednotky (OU) služby Azure AD Connect.
- Ujistěte se, že všichni synchronizovaní uživatelé domény mají licence na Microsoft 365 Business Premium.

Postup [najdete v tématu](manage-domain-users.md) Synchronizace uživatelů domény s Microsoftem.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Ověření autority MDM v Intune

Přejděte do [Správce koncových](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) bodů a na stránce Microsoft Intune vyberte Registrace zařízení a pak na stránce **Přehled** zkontrolujte, jestli je autorita **MDM** **Intune.**

- Pokud **oprávnění MDM nemá** hodnotu **Žádné,** klikněte na autoritu **MDM** a nastavte ji na **Intune.**
- Pokud je autorita **MDM** Microsoft Office  **365,** přejděte na Zařízení pro registraci zařízení a vpravo použijte dialog Přidat autoritu MDM k přidání autority MDM Intune (dialogové okno Přidat autoritu MDM je dostupné jenom v případě, že je autorita MDM nastavená na Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Ověření, že pro připojení k počítačům je povolená služba Azure AD

- Přejděte do Centra pro správu v adresáři a v seznamu Centra pro správu vyberte Zobrazit vše, pokud není služba <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> Azure Active Directory viditelná.   
- V Centru **pro správu Azure Active Directory** přejděte na Azure Active **Directory,** zvolte **Zařízení** a pak **Nastavení zařízení.**
- Ověření,**že uživatelé mohou připojit zařízení k Azure AD** je povolené 
    1. Pokud chcete povolit všechny uživatele, nastavte **možnost Všechny.**
    2. Pokud chcete povolit konkrétní uživatele, **nastavte možnost Selected (Vybráno),** aby se umožnila konkrétní skupina uživatelů.
        - Přidejte požadované uživatele domény synchronizované v Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)
        - Výběrem **možnosti Vybrat** skupiny povolíte obor uživatele MDM pro tuto skupinu zabezpečení.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Ověření, že je pro MDM povolený Azure AD

- Přejděte do Centra pro správu at a vyberte Správce koncových bodů (vyberte Zobrazit vše, pokud není správce koncových <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> bodů viditelný).   
- V Centru **pro správu Microsoft Endpoint Manageru** přejděte na **Zařízení,**  >  **do které Windows Windows**  >  **zamíská**  >  **automatickou registraci.**
- Ověřte, jestli je povolený obor uživatele MDM.

    1. Pokud chcete zaregistrovat všechny  počítače, nastavte možnost Vše tak, aby se při přidání pracovního účtu do Windows automaticky zaregistrovaly všechny uživatelské počítače připojené k Azure AD a nové počítače.
    2. Pokud chcete **zaregistrovat** počítače konkrétní skupiny uživatelů, nastavte možnost Někteří.
        -  Přidejte požadované uživatele domény synchronizované v Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)
        -  Výběrem **možnosti Vybrat** skupiny povolíte obor uživatele MDM pro tuto skupinu zabezpečení.

## <a name="4-create-the-required-resources"></a>4. Vytvoření požadovaných zdrojů 

Provádění požadovaných úkolů pro konfiguraci hybridního spojení [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) se zjednodušila pomocí rutiny [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Když tuto rutinu vyvoláte, vytvoří a nakonfiguruje potřebný spojovací bod služby a zásady skupiny.

Tento modul můžete nainstalovat tak, že z instance PowerShellu vytáčíte následující příkaz:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Doporučujeme tento modul nainstalovat na Windows Server, na který běží Azure AD Connect.

Pokud chcete vytvořit požadovaný spojovací bod služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Při provádění tohoto úkolu budete potřebovat přihlašovací údaje globálního správce Microsoft 365 Business Premium. Až budete připravení vytvořit prostředky, vyvolalte tyto kroky:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

První příkaz vytvoří připojení ke cloudu Microsoftu a po zobrazení výzvy zadejte své přihlašovací údaje globálního správce Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Propojení Zásady skupiny

1. V konzole Zásady skupiny Management Console (GPMC) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad* skupiny.
2. Vyberte zásadu vytvořenou v výše uvedeném kroku a klikněte na **OK.**

## <a name="get-the-latest-administrative-templates"></a>Získejte nejnovější šablony pro správu

Pokud zásadu nevidíte, povolte automatickou registraci MDM pomocí výchozích přihlašovacích údajů **Azure AD,** může to být proto, že nemáte nainstalovaný ADMX pro Windows 10, verzi 1803 nebo novější. Pokud chcete tento problém vyřešit, postupujte takto (Poznámka: Nejnovější jazyk MDM.admx je zpětně kompatibilní):

1.  Stáhnout: Šablony pro správu (.admx) pro Windows 10 – aktualizace z října [2020 (20H2)](https://www.microsoft.com/download/102157)
2.  Nainstalujte balíček v řadiči domény.
3.  Přejděte do složky v závislosti na verzi šablon pro správu: **C:\Program Files (x86)\Microsoft Zásady skupiny\Windows 10 Aktualizace z října 2020 (20H2)**
4.  **Přejmenujte složku Definice** zásad ve výše uvedené cestě na **PolicyMis.**
5.  Zkopírujte **složku PolicySystems** do sdílené složky SYSVOL ve výchozím nastavení v umístění **C:\Windows\SYSVOL\domain\Policies.** 
    -   Pokud plánujete používat centrální úložiště zásad pro celou doménu, přidejte obsah zásad.
6.  V případě, že máte několik řadičů domény, počkejte, až se funkce SYSVOL replikuje, aby zásady byly k dispozici. Tento postup bude fungovat i pro všechny budoucí verze šablon pro správu.

V tomto okamžiku by se vám měla zobrazit zásada Povolit automatickou registraci MDM pomocí výchozích dostupných přihlašovacích údajů **Azure AD.**
