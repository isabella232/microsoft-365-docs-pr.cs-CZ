---
title: Povolení správy zařízení s Windows 10 s doménou microsoftem 365 pro firmy
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
description: Přečtěte si, jak v několika krocích povolit microsoftu 365 ochranu místních zařízení se systémem Windows 10 připojenými k adresáři A active Directory.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560837"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Povolení správy zařízení s Windows 10 s doménou pomocí Microsoft 365 Business Premium

Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení spojené Azure AD**. Tato zařízení jsou připojena k místnímu službě Active Directory i k vašemu službě Azure Active Directory.

Toto video popisuje postup, jak nastavit tento scénář pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Než začnete, ujistěte se, že provedete tyto kroky:
- Synchronizujte uživatele s Azure AD pomocí služby Azure AD Connect.
- Dokončete synchronizaci organizační jednotky Azure AD Connect (OU).
- Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence k Microsoft 365 Business Premium.

Postup naleznete v tématu [Synchronizace uživatelů domény](manage-domain-users.md) společnosti Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Ověření autority MDM v Intune

Přejděte na [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) a na stránce Microsoft Intune vyberte **Registrace zařízení**a pak na stránce **Přehled** zkontrolujte, jestli je **autorita MDM** **Intune**.

- Pokud **autorita MDM** není **žádná**, klepněte na **autoritu MDM a** nastavte ji na **Intune**.
- Pokud je **autorita MDM** **Microsoft Office 365**, přejděte na **Zařízení**  >  **pro registraci zařízení** a použijte dialogové okno Přidat **autoritu MDM** vpravo k přidání autority **Intune MDM** (dialogové okno **Přidat autoritu MDM je** k dispozici jenom v případě, že je **autorita MDM** nastavená na Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Ověření, že azure ad je povolena pro připojení k počítačům

- Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte **Azure Active Directory** (v seznamu **Centra pro správu** vyberte Zobrazit vše, pokud azure active directory není viditelná). 
- V **Centru pro správu Služby Active Directory Azure**přejděte na **Azure Active Directory** , zvolte **Zařízení** a potom **nastavení zařízení**.
- Ověřit, že**uživatelé mohou připojit zařízení k Azure AD** je povolena 
    1. Chcete-li povolit všechny uživatele, nastavte hodnotu **Vše**.
    2. Chcete-li povolit konkrétní uživatele, nastavte na **Hodnotu Vybrané,** která povolí určitou skupinu uživatelů.
        - Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).
        - Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Ověření, že azure ad je povolena pro MDM

- Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte možnost **Endpoint Managemen**t (vyberte **Zobrazit vše,** pokud **endpoint Manager** není viditelný)
- V **Centru pro správu Správce koncových bodů společnosti Microsoft**přejděte na **Položku**Automatické  >  **Windows**  >  registrace**systému**Windows  >  **Automatic Enrollment**zařízení .
- Ověřte, zda je povolen obor uživatele MDM.

    1. Chcete-li zaregistrovat všechny počítače, nastavte na **Vše,** abyste automaticky zaregistrovali všechny uživatelské počítače, které jsou připojeny k Azure AD a novým počítačům, když uživatelé přidají pracovní účet do Windows.
    2. Chcete-li zaregistrovat počítače určité skupiny uživatelů, nastavte hodnotu **Některé.**
        -  Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).
        -  Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.

## <a name="4-create-the-required-resources"></a>4. Vytvořte požadované zdroje 

Provádění požadovaných úloh pro [konfiguraci hybridního spojení Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) bylo zjednodušeno použitím rutiny [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) která se nachází v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. Při vyvolání této rutiny vytvoří a nakonfiguruje požadovaný bod připojení služby a zásady skupiny.

Tento modul můžete nainstalovat vyvoláním následující z instance prostředí PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Doporučujeme nainstalovat tento modul na Windows Server se systémem Azure AD Connect.

Chcete-li vytvořit požadovaný bod připojení služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Při provádění tohoto úkolu budete potřebovat pověření globálního správce Microsoft 365 Business Premium. Až budete připraveni k vytvoření prostředků, vyvolat následující:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

První příkaz naváže spojení s cloudem Microsoftu a po zobrazení výzvy zadejte přihlašovací údaje globálního správce Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Propojení zásad skupiny

1. V Konzole GPMC (Group Policy Management Console) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad skupiny.*
2. Vyberte zásadu vytvořenou ve výše uvedeném kroku a klepněte na tlačítko **OK**.

## <a name="get-the-latest-administrative-templates"></a>Získejte nejnovější šablony pro správu

Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , může to být způsobeno tím, že nemáte nainstalované kódY ADMX pro Systém Windows 10 verze 1803, verze 1809 nebo verze 1903. Chcete-li tento problém vyřešit, postupujte takto (Poznámka: nejnovější MDM.admx je zpětně kompatibilní):

1.  Ke stažení: [Šablony pro správu (.admx) pro Windows 10 Květen 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Nainstalujte balíček do primárního řadiče domény (PDC).
3.  Navigace v závislosti na verzi složky: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.
4.  Přejmenujte složku **Definice zásad** ve výše uvedené cestě k **policydefinition .**
5.  Zkopírujte složku **PolicyDefinitions** do **souboru C:\Windows\SYSVOL\domain\Policies**. 
    -   Pokud máte v plánu použít centrální úložiště zásad pro celou doménu, přidejte obsah PolicyDefinitions tam.
6.  Chcete-li, aby byla tato zásada k dispozici, restartujte primární řadič domény. Tento postup bude fungovat i pro všechny budoucí verze.

V tomto okamžiku byste měli vidět zásady **Povolit automatické registrace MDM pomocí výchozích přihlašovacích údajů Azure AD** k dispozici.
