---
title: Povolení správy zařízení s Windows 10 s doménou microsoftem 365 pro firmy
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Přečtěte si, jak v několika krocích povolit microsoftu 365 ochranu místních zařízení se systémem Windows 10 připojenými k adresáři A active Directory.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471041"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Povolení správy zařízení s Windows 10 s doménou pomocí Microsoft 365 Business Premium

Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení spojené Azure AD**. Tato zařízení jsou připojena k místnímu službě Active Directory i k vašemu službě Azure Active Directory.

Toto video popisuje postup, jak nastavit tento scénář pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů z místní domény služby Active Directory zkontrolujte možnost [Příprava na synchronizaci adresářů s Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.
   
   - Doporučujeme nakonfigurovat **atribut userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoft 365. Například: *mary.shelley@contoso.com* spíše než *mary@contoso.local*
   
   - Pokud doména služby Active Directory končí nesměrovatelnou příponou, jako je *místní* nebo *lan*, namísto přípony směrovatelné serverem Internet, například *.com* nebo *.org*, upravte příponu hlavního názvu uživatele místních uživatelských účtů jako první, jak je popsáno v části [Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalace a konfigurace služby Azure AD Connect

Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte azure active directory connect a nastavte synchronizaci adresářů. Další informace najdete v tématu [Nastavení synchronizace adresářů pro Office 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

> [!NOTE]
> Kroky jsou přesně stejné pro Microsoft 365 pro firmy. 

Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporovaná v Microsoftu 365 pro firmy.

> [!NOTE]
> Existují některé další kroky pro zpětný zápis hesla nad rámec zaškrtávacího políčka ve službě Azure AD Connect. Další informace naleznete v [tématu How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurace hybridního připojení Azure AD

Než povolíte, aby se zařízení s Windows 10 připojila k hybridnímu Azure AD, ujistěte se, že splňujete následující požadavky:

   - Používáte nejnovější verzi Azure AD Connect.

   - Azure AD connect synchronizoval všechny objekty počítače zařízení, která chcete být hybridní Azure AD připojen. Pokud objekty počítače patří do konkrétní organizační jednotky (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v Azure AD připojení také.

Chcete-li zaregistrovat stávající zařízení s Windows 10 připojená k doméně jako hybridní Azure AD, postupujte podle pokynů v [kurzu: Konfigurace hybridního připojení Služby Azure Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Tento hybrid umožňuje stávající místní službu Active Directory připojit k počítačům s Windows 10 a připravit je na cloud.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Povolit automatickou registraci pro Windows 10

 Pokud se chcete automaticky zaregistrovat zařízení s Windows 10 pro správu mobilních zařízení v Intune, [přečtěte si tématu Automatické registrace zařízení s Windows 10 pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Zásady skupiny můžete nastavit na úrovni místního počítače nebo pro hromadné operace můžete pomocí Konzoly pro správu zásad skupiny a šablon ADMX vytvořit toto nastavení zásad skupiny v řadiči domény.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurace bezproblémového jednotného přihlašování

  Bezproblémové jednotné přihlašování automaticky přihlašuje uživatele do cloudových prostředků Microsoftu 365, když používají podnikové počítače. Jednoduše nasaďte jednu ze dvou možností zásad skupiny popsaných v [bezproblémovém jednotném přihlašování služby Azure Active Directory: Rychlý start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Možnost **Zásady skupiny** neumožňuje uživatelům měnit nastavení, zatímco možnost **Předvolba zásad skupiny** nastavuje hodnoty, ale také je nechává konfigurovatelné uživatelem.

## <a name="6-set-up-windows-hello-for-business"></a>6. Nastavení Windows Hello pro firmy

 Windows Hello pro firmy nahrazuje hesla silným dvoufaktorovým ověřováním (2FA) pro přihlášení do místního počítače. Jedním z faktorů je pár asymetrických klíčů a druhým je KÓD PIN nebo jiné místní gesto, jako je otisk prstu nebo rozpoznávání obličeje, pokud ho vaše zařízení podporuje. Doporučujeme, abyste pokud možno nahradili hesla 2FA a Windows Hello pro firmy.

Chcete-li nakonfigurovat hybridní Windows Hello pro firmy, přečtěte si [hybridní klíč důvěry Windows Hello pro obchodní požadavky](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Pak postupujte podle pokynů v [nastavení důvěryhodnosti hybridního windows hello pro obchodní klíč](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
