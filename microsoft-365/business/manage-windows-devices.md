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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dozvíte se, jak povolit aplikaci Microsoft 365 chránit místní služby AD připojené k zařízením Windows 10.
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068099"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Tuto možnost můžete nastavit tak, že nejprve synchronizujete službu Active Directory s Azure Active Directory a poté zaregistrujete zařízení systému Windows 10 s Azure AD a nastavíte je pro správu mobilních zařízení společností Microsoft 365 Business.
Následující video podrobně popisuje postup nastavení tohoto postupu pro nejběžnější scénář.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Nastavení zařízení připojených k doméně, která budou spravována společností Microsoft 365 Business

Chcete-li nastavit zařízení spojená s doménou organizace tak, aby měla užitek z možností poskytovaných službou Active Directory společnosti Azure, můžete kromě prostředí služby Active Directory implementovat také zařízení, která byla připojena k objektu **Hybrid Azure**. Jedná se o zařízení, která jsou připojena k vaší budově v prostředí Active Directory a k Azure Active Directory. Tato zařízení mohou být chráněna a spravována společností Microsoft 365 Business. 
  
Dokončete následující kroky a vytvořte tak zařízení Windows 10 Hybrid Azure AD a spravováno společností Microsoft 365 Business.
  
1. **Příprava na synchronizaci adresářů**: před synchronizací uživatelů a počítačů z místní domény služby Active Directory se seznamte [s přípravou synchronizace adresářů na sadu Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Ujistěte se, že v adresáři neexistují duplicity pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty by měly být jedinečné a všechny duplicity by měly být odstraněny..
   
   - Doporučujeme nastavit atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailovou adresou, která odpovídá Licencovanému uživateli Microsoft 365. Například **Mary.Shelley@contoso.com** místo **Mary @ contoso. místní**
   
   - Pokud je doména služby Active Directory ukončena v Nesměrovatelné příponě jako **. Local** nebo **. LAN**namísto internetové směrovatelné přípony, například **. com** nebo **. org**, bude nutné nejprve upravit příponu UPN místních uživatelských účtů, jak je popsáno v [Připravit nesměrovatelnou doménu pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **Instalace a konfigurace Azure AD Connect**: Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů z Azure připojení ke službě Active Directory. Další informace naleznete v tématu [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) .
    
    > [!NOTE]
    > Postup je pro společnost Microsoft 365 Business zcela stejný. 
    
Při konfiguraci možností pro Azure AD Connect doporučujeme povolit funkci **Synchronizace hesel** a **bezproblémové jednotné přihlašování**, stejně jako funkce **zpětného zápisu hesla** , která je podporována také v aplikaci Microsoft 365 Business.

> [!NOTE]
> Existují další kroky pro zpětný zápis hesla mimo zaškrtávací políčko v Azure AD Connect. Viz [Postupy: Konfigurace zpětného zápisu hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Konfigurace hybridního připojení AD**: dříve, než povolíte, aby se zařízení systému Windows 10 připojilo k hybridní Azure AD, měli byste se ujistit, že splajíš následující předpoklady:

   - Používáte nejnovější verzi připojení k programu Azure AD.

   - Azure AD Connect synchronizovalo všechny počítačové objekty zařízení, které chcete použít jako hybridní Azure AD. Pokud objekty počítače patří do určitých organizačních jednotek, zkontrolujte, zda jsou tyto organizační jednotky nastaveny pro synchronizaci také v Azure AD Connect.

Chcete-li registrovat existující domény spojené se systémem Windows 10, jak je připojena hybridní Azure AD, postupujte podle pokynů v [výukovém programu: Konfigurace hybridního připojení k adresáři Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tato možnost hybridně povolí existující objekty služby Active Directory připojené k počítačům se systémem Windows 10 a budou připraveny k vytvoření mraků.
    
4. **Povolení automatického zápisu pro systém Windows 10**: Chcete-li automaticky zapsat zařízení systému Windows 10 pro správu mobilních zařízení v nástroji Intune, vyhledejte informace [o zápisu zařízení systému Windows 10 automaticky pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Můžete nastavit zásady skupiny na úrovni místního počítače nebo pro hromadné operace, můžete vytvořit toto nastavení zásad skupiny v řadiči domény pomocí konzoly pro správu zásad skupiny a šablon ADMX.

5. **Konfigurovat bezproblémové jednotné přihlašování: bezproblémový**zápis SSO automaticky podepíše uživatele do svých zdrojů shluku Microsoft 365 při použití podnikových počítačů. Jednoduše nasaďte jednu ze dvou možností zásad skupiny popsaných v [Azure Active Directory – bezproblémové jednotné přihlášení: rychlý Start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Možnost **Zásady skupiny** neumožňuje uživatelům měnit jejich nastavení, zatímco možnost **předvoleb zásad skupiny** nastavuje hodnoty, ale také je nechává konfigurovatelné uživatelem.

6. **Nastavení systému Windows Hello for Business**: systém Windows Hello for Business nahrazuje hesla silným dvoufaktorového ověřování (2FA) pro přihlášení k místnímu počítači. Jeden faktor je asymetrický pár klíčů a druhý je PIN nebo jiné místní gesto, jako je například otisk prstu nebo obličeje, pokud to zařízení podporuje. Doporučujeme nahradit hesla 2 FA a Windows Hello for Business, pokud je to možné.

Chcete-li nakonfigurovat hybridní systém Windows Hello for Business, zkontrolujte [důvěryhodnost hybridního klíče Windows Hello for Business předpoklady](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Potom postupujte podle pokynů a [nakonfigurujte hybridní nastavení vztahu důvěryhodnosti systému Windows Hello pro obchodní klíč](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
