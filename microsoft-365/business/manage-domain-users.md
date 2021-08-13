---
title: Synchronizace uživatelů domény s Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Synchronizujte uživatele řízené doménou s Microsoft 365 pro firmy.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809306"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synchronizace uživatelů domény s Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Příprava na synchronizaci adresářů 

Před synchronizací uživatelů a počítačů z místní domény služby Active Directory si prohlédněte příprava synchronizace adresářů [na Microsoft 365](../enterprise/prepare-for-directory-synchronization.md). Konkrétně:

   - Ujistěte se, že v adresáři nejsou žádné duplicitní položky pro následující atributy: **pošta**, **proxyAddresses** a **userPrincipalName**. Tyto hodnoty musí být jedinečné a všechny duplicitní položky musí být odebrány.
   
   - Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencované Microsoft 365 uživateli. Příklad: *mary.shelley@contoso.com* místo *mary@contoso.local*
   
   - Pokud doména služby Active Directory končí nesmyšitelnou příponou, jako je *.local* nebo *.lan*, místo internetové směrovatelné přípony, jako je *.com* nebo *.org,* upravte nejprve příponu UPN místních uživatelských účtů, jak je popsáno v článku Příprava nesmyšitelné domény pro synchronizaci adresářů [.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Nástroj **Run IdFix** v kroku čtyři (4) dole také bude mít jistotu, že je místní adresář Active Directory připravený k synchronizaci adresářů.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Nainstalujte a nakonfigurujte Azure AD Připojení

Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, nainstalujte Azure Active Directory Připojení a nastavte synchronizaci adresářů. 

 1. V Centru [pro správu](https://go.microsoft.com/fwlink/p/?linkid=2024339)vyberte **Nastavení** v levém navigačním panelu.

 2. V **části Přihlášení a zabezpečení** zvolte **Zobrazení** v části Synchronizovat uživatele z adresáře **vaší organizace.**

 3. Na stránce **Synchronizovat uživatele z adresáře** vaší organizace zvolte **Začínáme**.

 4. V prvním kroku spusťte nástroj IdFix a připravte se na synchronizaci adresáře.

 5. Postupujte podle pokynů průvodce a stáhněte si Azure AD Připojení a použijte ho k synchronizaci uživatelů řízených doménou a Microsoft 365.


Další [informace najdete v tématu](../enterprise/set-up-directory-synchronization.md) Nastavení synchronizace Microsoft 365 adresářů.

Při konfiguraci možností pro Azure AD Připojení doporučujeme povolit synchronizaci hesel **,** bezproblémové jednotné  přihlašování a funkci zpětného zápisu hesel, která je podporovaná také v Microsoft 365 pro firmy.

> [!NOTE]
> Za zaškrtávacím políčkam v Azure AD Připojení jsou některé další kroky pro zpětný zápis Připojení. Další informace najdete v tématu [Postupy: Konfigurace zpětného zápisu hesla](/azure/active-directory/authentication/howto-sspr-writeback). 

Pokud chcete taky spravovat zařízení připojená Windows 10 [](manage-windows-devices.md) domény, podívejte se na článku Povolení správy Windows 10 připojených k doméně Microsoft 365 Business Premium a nastavení hybridního připojení k Azure AD.