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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Přečtěte si, jak povolit Microsoft 365 k ochraně místních zařízení se službou Active-Directory se systémem Windows 10 v několika krocích.
ms.openlocfilehash: 625eb7ac344b060409101d650ff30044d073f5bf
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561454"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá službu Windows Server Active Directory místně, můžete nastavit Microsoft 365 Business tak, aby chránila vaše zařízení s Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení připojená k Azure AD**. Tato zařízení jsou připojená k místní službě Active Directory i ke službě Azure Active Directory.

Toto video popisuje kroky, jak nastavit to pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů s místní doménou služby Active Directory zkontrolujte [možnost Připravit na synchronizaci adresářů s Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.
   
   - Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoftu 365. Příklad: *mary.shelley@contoso.com* spíše než *mary@contoso.local*
   
   - Pokud doména služby Active Directory končí nesměrovatelnou příponou, například *.local* nebo *.lan*, namísto přípony směrovatelné pro internet, *například .com* nebo *.org*, upravte příponu hlavního názvu uživatele místních uživatelských účtů nejprve, jak je popsáno v [části Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalace a konfigurace služby Azure AD Connect

Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte službu Azure Active Directory Connect a nastavte synchronizaci adresářů. Další informace najdete [v tématu Nastavení synchronizace adresářů pro Office 365.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Kroky jsou přesně stejné pro Microsoft 365 Business. 

Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporovaná v Microsoft 365 Business.

> [!NOTE]
> Existují některé další kroky pro zpětný zápis hesla za zaškrtávací políčko v Azure AD Connect. Další informace naleznete v [tématu How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurace hybridního připojení k azure reklamě

Než povolíte, aby se zařízení s Windows 10 připojila k hybridnímu Azure AD, ujistěte se, že splňujete následující požadavky:

   - Používáte nejnovější verzi Služby Azure AD Connect.

   - Azure AD connect synchronizovala všechny objekty počítače zařízení, která chcete být hybridní Azure AD připojen. Pokud objekty počítače patří do konkrétníorganizační jednotky (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v Azure AD připojení také.

Pokud chcete zaregistrovat stávající zařízení s Windows 10 připojená k doméně jako hybridní Azure AD, postupujte podle pokynů v [kurzu: Konfigurace hybridního připojení služby Azure Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tento hybrid umožňuje vaše stávající místní služby Active Directory připojované k počítačům se systémem Windows 10 a připravit je na cloud.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Povolení automatické registrace pro Windows 10

 Pokud chcete automaticky zaregistrovat zařízení s Windows 10 pro správu mobilních zařízení v Intune, přečtěte si pár [automaticky zaregistrovat zařízení s Windows 10 pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zásady skupiny můžete nastavit na úrovni místního počítače nebo pro hromadné operace, pomocí konzoly pro správu zásad skupiny a šablon ADMX můžete vytvořit toto nastavení zásad skupiny v řadiči domény.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurace bezproblémového jednotného přihlašování

  Bezproblémové jednotné přihlašuje automaticky přihlašuje uživatele do svých cloudových prostředků Microsoft 365 při použití podnikových počítačů. Jednoduše nasadit jednu ze dvou možností zásad skupiny popsaných ve [službě Azure Active Directory Bezproblémové jednotné přihlašování: Rychlý start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Možnost **Zásady skupiny** neumožňuje uživatelům měnit nastavení, zatímco možnost **Předvolby zásad skupiny** nastavuje hodnoty, ale také je ponechává nakonfigurovatelné uživateli.

## <a name="6-set-up-windows-hello-for-business"></a>6. Nastavení Windows Hello pro firmy

 Windows Hello pro firmy nahrazuje hesla silným dvoufaktorovým ověřováním (2FA) pro přihlášení k místnímu počítači. Jedním z faktorů je asymetrický pár klíčů a druhým je KÓD PIN nebo jiné místní gesto, například otisk prstu nebo rozpoznávání obličeje, pokud jej vaše zařízení podporuje. Doporučujeme, abyste hesla nahradili 2FA a Windows Hello pro firmy, kde je to možné.

Chcete-li nakonfigurovat hybridní Windows Hello pro firmy, přečtěte si odkaz na [požadavky hybridního klíče, kterým důvěřujete windows hello pro firmy](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Potom postupujte podle pokynů v [tématu Konfigurace hybridního windows hello pro firmy, kterým se důvěryhodnost vyslovuje](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
