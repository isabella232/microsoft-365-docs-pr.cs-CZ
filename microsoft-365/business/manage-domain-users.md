---
title: Synchronizace uživatelů domény s Microsoft 365
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
description: Synchronizace uživatelů s řízenými doménami Microsoft 365 pro firmy.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306443"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizace uživatelů domény s Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Než synchronizujete uživatele a počítače z místní domény Active Directory, přečtěte si téma [Příprava synchronizace adresářů do Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization). Zejména:

   - Zkontrolujte, že v adresáři neexistují žádné duplicity pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplicitní položky musí být odebrány.
   
   - Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá Licencovanému uživateli aplikace Microsoft 365. Třeba: *Mary.Shelley@contoso.com* místo *Mary@contoso. Local*
   
   - Pokud doména služby Active Directory končí v Nesměrovatelné příponě, *jako je třeba. com nebo.* org, místo internetové přihlášené *přípony, jako*je třeba *. com* nebo *. org*, upravte příponu UPN místních uživatelských účtů, jak je popsáno v části [Příprava domény, která není směrovatelný](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

Pomocí **příkazu Spustit IdFix** v kroku čtyři (4) níže se také ujistěte, že je váš místní adresář Active Directory připravený na synchronizaci adresářů.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. instalace a konfigurace Azure AD Connect

Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte Azure Active Directory Connect a nastavte synchronizaci adresářů. 

 1. V centru pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vyberte v levém navigačním podokně možnost **Nastavení** .

 2. V části **přihlášení a zabezpečení**zvolte **Zobrazit**  v části **synchronizace uživatelů z adresáře vaší organizace**.

 3. Na stránce **synchronizovat uživatele z adresáře organizace** zvolte **Začínáme**.

 4. V prvním kroku spusťte nástroj IdFix (příprava synchronizace adresářů).

 5. Postupujte podle pokynů průvodce a Stáhněte si Azure AD Connect a použijte ho k synchronizaci uživatelů, kteří řídí vaši doménu, na Microsoft 365.


Další informace najdete v tématu [Nastavení synchronizace adresářů pro Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .

Když nakonfigurujete možnosti pro Azure AD Connect, doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesel** , která je taky podporovaná v Microsoft 365 pro firmy.

> [!NOTE]
> Za zaškrtávacím políčkem služby Azure AD Connect je k dispozici několik dalších kroků. Další informace najdete v tématu [Postupy: Konfigurace zpětného zápisu hesel](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Pokud chcete spravovat zařízení s Windows 10 připojená k doméně taky, přečtěte si článek Povolení hybridního připojení Azure AD [pro správu zařízení s Windows 10 připojenými k doméně v Microsoft 365 Business Premium](manage-windows-devices.md) . 