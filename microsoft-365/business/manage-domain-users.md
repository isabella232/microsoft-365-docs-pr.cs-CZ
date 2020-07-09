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
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="d0ca6-103">Synchronizace uživatelů domény s Microsoftem 365</span><span class="sxs-lookup"><span data-stu-id="d0ca6-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="d0ca6-104">1. Příprava na synchronizaci adresářů</span><span class="sxs-lookup"><span data-stu-id="d0ca6-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="d0ca6-105">Před synchronizací uživatelů a počítačů z místní domény služby Active Directory zkontrolujte možnost [Příprava na synchronizaci adresářů s aplikací Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d0ca6-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="d0ca6-106">Zejména:</span><span class="sxs-lookup"><span data-stu-id="d0ca6-106">In particular:</span></span>

   - <span data-ttu-id="d0ca6-107">Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **mail**, **proxyAddresses**a **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="d0ca6-108">Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="d0ca6-109">Doporučujeme nakonfigurovat **atribut userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="d0ca6-110">Například: *mary.shelley@contoso.com* spíše než *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="d0ca6-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="d0ca6-111">Pokud doména služby Active Directory končí nesměrovatelnou příponou, jako je *místní* nebo *lan*, namísto přípony směrovatelné serverem Internet, například *.com* nebo *.org*, upravte příponu hlavního názvu uživatele místních uživatelských účtů jako první, jak je popsáno v části [Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d0ca6-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="d0ca6-112">**Spustit IdFix** v kroku čtyři (4) níže, bude také ujistěte se, že místní Active Directory je připraven pro synchronizaci dir.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="d0ca6-113">2. Instalace a konfigurace služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d0ca6-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="d0ca6-114">Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte azure active directory connect a nastavte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="d0ca6-115">V Centru pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> vyberte **Nastavení** v levém navigačním panelu.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="d0ca6-116">V části **Přihlášení a zabezpečení**zvolte **Zobrazit** v části **Synchronizovat uživatele z adresáře vaší organizace**.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="d0ca6-117">Na stránce **Synchronizovat uživatele z adresáře vaší organizace** zvolte **Začínáme**.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="d0ca6-118">V prvním kroku spusťte nástroj IdFix pro přípravu na synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="d0ca6-119">Podle pokynů průvodce stáhněte Azure AD Connect a použijte ho k synchronizaci uživatelů s řízenou doménou s Microsoftem 365.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="d0ca6-120">Další informace najdete v tématu [Nastavení synchronizace adresářů pro Microsoft 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="d0ca6-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="d0ca6-121">Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporovaná v Microsoftu 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="d0ca6-122">Existují některé další kroky pro zpětný zápis hesla nad rámec zaškrtávacího políčka ve službě Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="d0ca6-123">Další informace naleznete v [tématu How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d0ca6-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="d0ca6-124">Pokud chcete spravovat i zařízení s Windows 10 připojená k doméně, přečtěte si [tématu Povolení správy zařízení s Windows 10 s doménou pomocí Microsoftu 365 Business Premium](manage-windows-devices.md) a nastavení hybridního připojení Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="d0ca6-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 