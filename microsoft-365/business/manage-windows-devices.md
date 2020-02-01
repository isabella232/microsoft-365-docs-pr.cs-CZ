---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
f1.keywords:
- NOCSH
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
description: Přečtěte si, jak povolit Microsoft 365 chránit místní zařízení se systémem Active Directory připojená k windows 10.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593795"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business k ochraně zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení připojená ke**službě Azure AD . Tato zařízení jsou spojena s místní službou Active Directory i s Azure Active Directory.

Toto video popisuje postup, jak nastavit tento pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů z místní domény služby Active Directory zkontrolujte, že [synchronizace adresářů s Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)najdete v části Příprava na synchronizaci adresářů . Zejména:

   - Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **pošta**, **proxyAdresy**a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.
   
   - Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoft 365. Například: *mary.shelley@contoso.com* spíše než *mary@contoso.local*
   
   - Pokud doména služby Active Directory končí nesměrovatelnou příponou, jako *je místní* nebo *.lan*, namísto internetové horečné přípony, jako je *například .com* nebo *.org*, upravte příponu hlavního názvu místních uživatelských účtů, jak je popsáno v [části Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalace a konfigurace Azure AD Connect

Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte Azure Active Directory Connect a nastavte synchronizaci adresářů. Další informace najdete v [tématu Nastavení synchronizace adresářů pro Office 365.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Kroky jsou přesně stejné pro Microsoft 365 Business. 

Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporována v Microsoft 365 Business.

> [!NOTE]
> Zaškrtávací políčko Azure AD Connect zaškrtávací políčko jsou i další kroky pro zpětný zápis hesla. Další informace naleznete v tématu [Postup: konfigurace zpětného zápisu hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurace hybridního připojení azure reklam

Než povolíte, aby zařízení s Windows 10 byla připojena k hybridní azure ad, ujistěte se, že splňujete následující požadavky:

   - Používáte nejnovější verzi Azure AD Connect.

   - Připojení Azure AD synchronizované všechny objekty počítače zařízení, které chcete být hybridní Azure AD připojil. Pokud objekty počítače patří do konkrétních organizačních jednotek (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v připojení Azure AD také.

Chcete-li zaregistrovat existující zařízení s Windows 10 připojenou k doméně jako připojení hybridní azure ad, postupujte podle pokynů v [kurzu: Konfigurace hybridního připojení služby Azure Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tento hybrid umožňuje, aby se k počítačům se systémem Windows 10 připojily stávající místní služby Active Directory a připravily je na cloud.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Povolit automatickou registraci pro Windows 10

 Pokud chcete automaticky zaregistrovat zařízení s Windows 10 pro správu mobilních zařízení v Intune, přečtěte si článku [Automatické registrace zařízení s Windows 10 pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zásady skupiny můžete nastavit na úrovni místního počítače nebo pro hromadné operace, můžete použít šablony Konzoly pro správu zásad skupiny a šablony ADMX k vytvoření tohoto nastavení zásad skupiny v řadiči domény.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurace bezproblémového jednotného přihlášení

  Bezproblémové jednotné přihlašuje automaticky uživatele do svých cloudových prostředků Microsoft 365, když používají podnikové počítače. Jednoduše nasaďte jednu ze dvou možností zásad skupiny popsaných v [Azure Active Directory Bezproblémové jednotné přihlašování: Rychlý start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Možnost **Zásady skupiny** neumožňuje uživatelům měnit jejich nastavení, zatímco možnost **Předvolby zásad skupiny** nastavuje hodnoty, ale také je ponechá uživatelsky konfigurovatelné.

## <a name="6-set-up-windows-hello-for-business"></a>6. Nastavení Windows Hello pro firmy

 Windows Hello for Business nahrazuje hesla silným dvoufaktorovým ověřováním (2FA) pro přihlášení k místnímu počítači. Jedním z faktorů je asymetrický pár klíčů a druhý je KÓD PIN nebo jiné místní gesto, jako je otisk prstu nebo rozpoznávání obličeje, pokud jej zařízení podporuje. Pokud je to možné, doporučujeme nahradit hesla 2FA a Windows Hello pro firmy.

Chcete-li nakonfigurovat hybridní windows hello pro firmy, přečtěte si [vztah důvěryhodnosti hybridního klíče Windows Hello pro obchodní předpoklady](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Potom postupujte podle pokynů v [části Konfigurovat hybridní nastavení důvěryhodnosti klíčů systému Windows Hello pro firmy](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
