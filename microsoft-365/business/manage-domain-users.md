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
description: Synchronizujte uživatele řízené doménou s Microsoftem 365 pro firmy.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913248"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="7650b-103">Synchronizace uživatelů domény s Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7650b-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="7650b-104">1. Příprava na synchronizaci adresářů</span><span class="sxs-lookup"><span data-stu-id="7650b-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="7650b-105">Před synchronizací uživatelů a počítačů z místní domény služby Active Directory si prohlédněte článek Příprava synchronizace [adresářů s Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="7650b-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="7650b-106">Konkrétně:</span><span class="sxs-lookup"><span data-stu-id="7650b-106">In particular:</span></span>

   - <span data-ttu-id="7650b-107">Ujistěte se, že v adresáři nejsou žádné duplicitní položky pro následující atributy: **pošta**, **proxyAddresses** a **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="7650b-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="7650b-108">Tyto hodnoty musí být jedinečné a všechny duplicitní položky musí být odebrány.</span><span class="sxs-lookup"><span data-stu-id="7650b-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="7650b-109">Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="7650b-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="7650b-110">Příklad: *mary.shelley@contoso.com* místo *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="7650b-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="7650b-111">Pokud doména služby Active Directory končí nesmyšitelnou příponou, jako je *.local* nebo *.lan*, místo internetové směrovatelné přípony, jako je *.com* nebo *.org,* upravte nejprve příponu UPN místních uživatelských účtů, jak je popsáno v článku Příprava nesmyšitelné domény pro synchronizaci adresářů [.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="7650b-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="7650b-112">Nástroj **Run IdFix** v kroku čtyři (4) dole také bude mít jistotu, že je místní adresář Active Directory připravený k synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="7650b-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="7650b-113">2. Instalace a konfigurace Služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7650b-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="7650b-114">Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, nainstalujte Azure Active Directory Connect a nastavte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="7650b-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="7650b-115">V Centru [pro správu](https://go.microsoft.com/fwlink/p/?linkid=2024339)vyberte **Nastavení** v levém navigačním panelu.</span><span class="sxs-lookup"><span data-stu-id="7650b-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="7650b-116">V **části Přihlášení a zabezpečení** zvolte **Zobrazení** v části Synchronizovat uživatele z adresáře **vaší organizace.**</span><span class="sxs-lookup"><span data-stu-id="7650b-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="7650b-117">Na stránce **Synchronizovat uživatele z adresáře** vaší organizace zvolte **Začínáme**.</span><span class="sxs-lookup"><span data-stu-id="7650b-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="7650b-118">V prvním kroku spusťte nástroj IdFix a připravte se na synchronizaci adresáře.</span><span class="sxs-lookup"><span data-stu-id="7650b-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="7650b-119">Postupujte podle pokynů průvodce a stáhněte si Azure AD Connect a použijte ho k synchronizaci uživatelů řízených doménou s Microsoftem 365.</span><span class="sxs-lookup"><span data-stu-id="7650b-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="7650b-120">Další informace najdete v tématu Nastavení synchronizace adresářů [pro Microsoft 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="7650b-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="7650b-121">Při konfiguraci možností pro Azure AD Connect doporučujeme povolit synchronizaci hesel **,** bezproblémové jednotné přihlašování a funkci zpětného zápisu hesel, která je podporovaná také v Microsoftu 365 pro firmy. </span><span class="sxs-lookup"><span data-stu-id="7650b-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="7650b-122">Existuje několik dalších kroků pro zpětný zápis hesel za zaškrtávací políčko v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7650b-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="7650b-123">Další informace najdete v tématu [Postupy: Konfigurace zpětného zápisu hesla](/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="7650b-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="7650b-124">Pokud chcete taky spravovat zařízení s Windows 10 připojená k doméně, podívejte se na článek Povolení správy zařízení s Windows 10 připojených k doméně [microsoftem 365 Business Premium](manage-windows-devices.md) a nastavení hybridního připojení k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7650b-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>