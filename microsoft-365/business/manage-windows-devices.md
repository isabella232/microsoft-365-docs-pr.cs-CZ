---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dozvíte se, jak povolit aplikaci Microsoft 365 chránit místní služby AD připojené k zařízením Windows 10.
ms.openlocfilehash: 392c57a7350a901c1481be632e880cc9fcaa6140
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575972"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li toto nastavení nastavit, můžete implementovat zařízení, která jsou připojena k této **službě**. Jedná se o zařízení, která jsou připojena k vaší budově v prostředí Active Directory a k Azure Active Directory.

Následující video podrobně popisuje postup nastavení tohoto postupu pro nejběžnější scénář, který je také podrobně popsána v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů z místní domény služby Active Directory se seznamte [s přípravou synchronizace adresářů na sadu Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Ujistěte se, že v adresáři neexistují duplicity pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty by měly být jedinečné a všechny duplicity by měly být odstraněny.
   
   - Doporučujeme nastavit atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailovou adresou, která odpovídá Licencovanému uživateli Microsoft 365. Například *Mary.Shelley@contoso.com* místo *Mary @ contoso. místní*
   
   - Pokud je doména služby Active Directory ukončena v Nesměrovatelné příponě jako *. Local* nebo *. LAN*namísto internetové směrovatelné přípony, například *. com* nebo *. org*, bude nutné nejprve upravit příponu UPN místních uživatelských účtů, jak je popsáno v [Připravit nesměrovatelnou doménu pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. instalace a konfigurace Azure AD Connect

Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře služby Active Directory do Azure Active Directory, nainstalujte připojení k adresáři Azure Active Directory a nastavte synchronizaci adresářů. Další informace naleznete v tématu [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) .

> [!NOTE]
> Postup je pro společnost Microsoft 365 Business zcela stejný. 

Při konfiguraci možností pro Azure AD Connect doporučujeme povolit funkci **Synchronizace hesel** a **bezproblémové jednotné přihlašování**, stejně jako funkce **zpětného zápisu hesla** , která je podporována také v aplikaci Microsoft 365 Business.

> [!NOTE]
> Existují další kroky pro zpětný zápis hesla mimo zaškrtávací políčko v Azure AD Connect. Další informace naleznete v tématu [Postupy: Konfigurace zpětného zápisu hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. nastavit hybridní Azure spojení AD

Dříve než povolíte, aby zařízení Windows 10 byla připojena k hybridní Azure AD, měli byste se ujistit, že splavíte následující předpoklady:

   - Používáte nejnovější verzi připojení k programu Azure AD.

   - Azure AD Connect synchronizovalo všechny počítačové objekty zařízení, které chcete použít jako hybridní Azure AD. Pokud objekty počítače patří do určitých organizačních jednotek, zkontrolujte, zda jsou tyto organizační jednotky nastaveny pro synchronizaci také v Azure AD Connect.

Chcete-li registrovat existující domény spojené se systémem Windows 10, jak je připojena hybridní Azure AD, postupujte podle pokynů v [výukovém programu: Konfigurace hybridního připojení k adresáři Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tato možnost hybridně povolí existující objekty služby Active Directory připojené k počítačům se systémem Windows 10 a budou připraveny k vytvoření mraků.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Povolit automatický zápis pro systém Windows 10

 Informace o automatickém zápisu zařízení systému Windows 10 pro správu mobilních zařízení v nástroji Intune naleznete v tématu [zápis zařízení systému Windows 10 automaticky pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Můžete nastavit zásady skupiny na úrovni místního počítače nebo pro hromadné operace, můžete vytvořit toto nastavení zásad skupiny v řadiči domény pomocí konzoly pro správu zásad skupiny a šablon ADMX.

## <a name="5-configure-seamless-single-sign-on"></a>5. konfigurace bezproblémové jednotného přihlašování

  Bezproblémový zápis SSO automaticky podepíše uživatele do svých zdrojů shluku Microsoft 365 při použití podnikových počítačů. Jednoduše nasaďte jednu ze dvou možností zásad skupiny popsaných v [Azure Active Directory – bezproblémové jednotné přihlášení: rychlý Start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Možnost **Zásady skupiny** neumožňuje uživatelům měnit jejich nastavení, zatímco možnost **předvoleb zásad skupiny** nastavuje hodnoty, ale také je nechává konfigurovatelné uživatelem.

## <a name="6-set-up-windows-hello-for-business"></a>6. nastavení systému Windows Hello for Business

 Systém Windows Hello for Business nahrazuje hesla silným dvoufaktorového ověřování (2FA) pro přihlášení k místnímu počítači. Jeden faktor je asymetrický pár klíčů a druhý je PIN nebo jiné místní gesto, jako je například otisk prstu nebo obličeje, pokud to zařízení podporuje. Doporučujeme nahradit hesla 2FA a Windows Hello for Business, pokud je to možné.

Chcete-li nakonfigurovat hybridní systém Windows Hello for Business, zkontrolujte [důvěryhodnost hybridního klíče Windows Hello for Business předpoklady](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Potom postupujte podle pokynů v [konfiguraci hybridních klíčů Windows Hello pro nastavení důvěryhodnosti obchodního klíče](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
