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
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="907cb-103">Synchronizace uživatelů domény s Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="907cb-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="907cb-104">1. Příprava na synchronizaci adresářů</span><span class="sxs-lookup"><span data-stu-id="907cb-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="907cb-105">Než synchronizujete uživatele a počítače z místní domény Active Directory, přečtěte si téma [Příprava synchronizace adresářů do Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="907cb-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="907cb-106">Zejména:</span><span class="sxs-lookup"><span data-stu-id="907cb-106">In particular:</span></span>

   - <span data-ttu-id="907cb-107">Zkontrolujte, že v adresáři neexistují žádné duplicity pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="907cb-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="907cb-108">Tyto hodnoty musí být jedinečné a všechny duplicitní položky musí být odebrány.</span><span class="sxs-lookup"><span data-stu-id="907cb-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="907cb-109">Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá Licencovanému uživateli aplikace Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="907cb-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="907cb-110">Třeba: *Mary.Shelley@contoso.com* místo *Mary@contoso. Local*</span><span class="sxs-lookup"><span data-stu-id="907cb-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="907cb-111">Pokud doména služby Active Directory končí v Nesměrovatelné příponě, *jako je třeba. com nebo.* org, místo internetové přihlášené *přípony, jako*je třeba *. com* nebo *. org*, upravte příponu UPN místních uživatelských účtů, jak je popsáno v části [Příprava domény, která není směrovatelný](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="907cb-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="907cb-112">Pomocí **příkazu Spustit IdFix** v kroku čtyři (4) níže se také ujistěte, že je váš místní adresář Active Directory připravený na synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="907cb-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="907cb-113">2. instalace a konfigurace Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="907cb-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="907cb-114">Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte Azure Active Directory Connect a nastavte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="907cb-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="907cb-115">V centru pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vyberte v levém navigačním podokně možnost **Nastavení** .</span><span class="sxs-lookup"><span data-stu-id="907cb-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="907cb-116">V části **přihlášení a zabezpečení**zvolte **Zobrazit**  v části **synchronizace uživatelů z adresáře vaší organizace**.</span><span class="sxs-lookup"><span data-stu-id="907cb-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="907cb-117">Na stránce **synchronizovat uživatele z adresáře organizace** zvolte **Začínáme**.</span><span class="sxs-lookup"><span data-stu-id="907cb-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="907cb-118">V prvním kroku spusťte nástroj IdFix (příprava synchronizace adresářů).</span><span class="sxs-lookup"><span data-stu-id="907cb-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="907cb-119">Postupujte podle pokynů průvodce a Stáhněte si Azure AD Connect a použijte ho k synchronizaci uživatelů, kteří řídí vaši doménu, na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="907cb-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="907cb-120">Další informace najdete v tématu [Nastavení synchronizace adresářů pro Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .</span><span class="sxs-lookup"><span data-stu-id="907cb-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="907cb-121">Když nakonfigurujete možnosti pro Azure AD Connect, doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesel** , která je taky podporovaná v Microsoft 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="907cb-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="907cb-122">Za zaškrtávacím políčkem služby Azure AD Connect je k dispozici několik dalších kroků.</span><span class="sxs-lookup"><span data-stu-id="907cb-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="907cb-123">Další informace najdete v tématu [Postupy: Konfigurace zpětného zápisu hesel](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="907cb-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="907cb-124">Pokud chcete spravovat zařízení s Windows 10 připojená k doméně taky, přečtěte si článek Povolení hybridního připojení Azure AD [pro správu zařízení s Windows 10 připojenými k doméně v Microsoft 365 Business Premium](manage-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="907cb-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 