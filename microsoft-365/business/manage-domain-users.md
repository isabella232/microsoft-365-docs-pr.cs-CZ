---
title: Synchronizace uživatelů domény s Microsoftem 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
- MOE150
description: Synchronizujte uživatele s microsoftem 365 pro firmy.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081817"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizace uživatelů domény s Microsoftem 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů z místní domény služby Active Directory zkontrolujte možnost [Příprava na synchronizaci adresářů s aplikací Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.
   
   - Doporučujeme nakonfigurovat **atribut userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoft 365. Například: *mary.shelley@contoso.com* spíše než *mary@contoso.local*
   
   - Pokud doména služby Active Directory končí nesměrovatelnou příponou, jako je *místní* nebo *lan*, namísto přípony směrovatelné serverem Internet, například *.com* nebo *.org*, upravte příponu hlavního názvu uživatele místních uživatelských účtů jako první, jak je popsáno v části [Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

**Spustit IdFix** v kroku čtyři (4) níže, bude také ujistěte se, že místní Active Directory je připraven pro synchronizaci dir.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Instalace a konfigurace služby Azure AD Connect

Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte azure active directory connect a nastavte synchronizaci adresářů. 

 1. V Centru pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vyberte **Nastavení** v levém navigačním panelu.

 2. V části **Přihlášení a zabezpečení**zvolte **Zobrazit** v části **Synchronizovat uživatele z adresáře vaší organizace**.

 3. Na stránce **Synchronizovat uživatele z adresáře vaší organizace** zvolte **Začínáme**.

 4. V prvním kroku spusťte nástroj IdFix pro přípravu na synchronizaci adresářů.

 5. Podle pokynů průvodce stáhněte Azure AD Connect a použijte ho k synchronizaci uživatelů s řízenou doménou s Microsoftem 365.


Další informace najdete v tématu [Nastavení synchronizace adresářů pro Microsoft 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporovaná v Microsoftu 365 pro firmy.

> [!NOTE]
> Existují některé další kroky pro zpětný zápis hesla nad rámec zaškrtávacího políčka ve službě Azure AD Connect. Další informace naleznete v [tématu How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Pokud chcete spravovat i zařízení s Windows 10 připojená k doméně, přečtěte si [tématu Povolení správy zařízení s Windows 10 s doménou pomocí Microsoftu 365 Business Premium](manage-windows-devices.md) a nastavení hybridního připojení Azure AD Join. 