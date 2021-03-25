---
title: Migrace z Microsoftu 365 Business na Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Zjistěte, jak přesunout svou firmu z Microsoft 365 Business Premium na Microsoft 365 E3.
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164507"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="b4f5e-103">Migrace z Microsoft 365 Business Premium na Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="b4f5e-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="b4f5e-104">Microsoft 365 Business Premium má všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace založené na produktivitě s jednoduchou snadná správa zařízení a zabezpečení, které vašim zaměstnancům umožňují dělat nejlepší práci.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="b4f5e-105">V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium na Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="b4f5e-106">Vaše firma například roste a potřebuje víc než 300 licencí (mimochodem blahopřejeme).</span><span class="sxs-lookup"><span data-stu-id="b4f5e-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="b4f5e-107">Nebo vaše firma potřebuje podnikové funkce, jako jsou Aplikace Microsoft 365 pro podniky, Windows 10 Enterprise E3 nebo Licence klientského přístupu enterprise (CAL).</span><span class="sxs-lookup"><span data-stu-id="b4f5e-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="b4f5e-108">Upgrade je snadný: Upgrade můžete spustit z [Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="b4f5e-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="b4f5e-109">Všechna vaše data a konfigurace v aktuálním předplatném se zachová.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="b4f5e-110">Není nic, co byste měli udělat, abyste se připravili na migraci a potom nic dělat, kromě využití nových funkcí.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="b4f5e-111">Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="b4f5e-112">Microsoft Defender pro Office 365 ale není součástí Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="b4f5e-113">Pokud chcete pokračovat v ochraně před hrozbami, měli byste přidat další licence Defenderu pro Office 365, aby měli licenci všichni uživatelé, kteří mají v rámci vašeho programu Defender for Office 365 licenci.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="b4f5e-114">Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="b4f5e-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="b4f5e-115">V této tabulce jsou uvedené rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="b4f5e-116">Funkce</span><span class="sxs-lookup"><span data-stu-id="b4f5e-116">Feature</span></span>    | <span data-ttu-id="b4f5e-117">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b4f5e-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="b4f5e-118">Podpora v Microsoftu 365 E3</span><span class="sxs-lookup"><span data-stu-id="b4f5e-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="b4f5e-119">**Místní**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="b4f5e-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b4f5e-120">Windows 10</span></span>    | <span data-ttu-id="b4f5e-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="b4f5e-121">Windows 10 Business</span></span>  |     <span data-ttu-id="b4f5e-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b4f5e-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="b4f5e-123">Aplikace Office\*</span><span class="sxs-lookup"><span data-stu-id="b4f5e-123">Office apps\*</span></span>    | [<span data-ttu-id="b4f5e-124">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="b4f5e-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="b4f5e-125">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="b4f5e-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="b4f5e-126">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="b4f5e-127">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="b4f5e-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="b4f5e-128">Limit úložiště 50 GB na poštovní schránku a neomezenou archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b4f5e-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="b4f5e-129">Limit úložiště 100 GB na poštovní schránku a neomezenou archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b4f5e-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="b4f5e-130">Teams</span><span class="sxs-lookup"><span data-stu-id="b4f5e-130">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-133">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="b4f5e-133">OneDrive for Business</span></span>    | <span data-ttu-id="b4f5e-134">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="b4f5e-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="b4f5e-135">Neomezená</span><span class="sxs-lookup"><span data-stu-id="b4f5e-135">Unlimited</span></span> | 
| <span data-ttu-id="b4f5e-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="b4f5e-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-139">**Ochrana před hrozbou**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-139">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="b4f5e-140">Možnosti omezení útoku na povrch</span><span class="sxs-lookup"><span data-stu-id="b4f5e-140">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="b4f5e-141">Zobrazit tento seznam</span><span class="sxs-lookup"><span data-stu-id="b4f5e-141">See this list</span></span>](#threat-protection) | <span data-ttu-id="b4f5e-142">Enterprise management of hardware-based isolation for Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b4f5e-142">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="b4f5e-143">Defender pro Office 365 – plán 1</span><span class="sxs-lookup"><span data-stu-id="b4f5e-143">Defender for Office 365 Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="b4f5e-145">Není zahrnuto, ale může být přidáno dne</span><span class="sxs-lookup"><span data-stu-id="b4f5e-145">Not included, but can be added on</span></span> | 
| <span data-ttu-id="b4f5e-146">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-146">**Identity management**</span></span>        | | | 
| <span data-ttu-id="b4f5e-147">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesla pro místní identity</span><span class="sxs-lookup"><span data-stu-id="b4f5e-147">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-150">Cloud App Discovery, Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="b4f5e-150">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-152">Aplikace Azure AD Office 365 Single Sign-On (SSO): 10 aplikací na uživatele (aplikace SaaS galerie, jako je Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="b4f5e-152">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-155">Jednotné přihlašování k Azure AD Premium 1: bez omezení (místní aplikace prostřednictvím proxy aplikací Azure AD a aplikací mimo galerii pomocí šablon Self-Service Integrace aplikací)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-155">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-157">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-157">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="b4f5e-158">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="b4f5e-158">Microsoft Intune, Windows Autopilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b4f5e-161">Přístup k virtuální ploše (VDA)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-161">Virtual Desktop Access (VDA)</span></span>    |  |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b4f5e-163">Virtuální plocha Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-163">Windows Virtual Desktop (WVD)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b4f5e-166">Aktivace sdíleného počítače (SCA)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-166">Shared Computer Activation (SCA)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-169">Microsoft Desktop Optimization Package</span><span class="sxs-lookup"><span data-stu-id="b4f5e-169">Microsoft Desktop Optimization Package</span></span>    | |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-171">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-171">**Information protection**</span></span>        | | | 
| <span data-ttu-id="b4f5e-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span><span class="sxs-lookup"><span data-stu-id="b4f5e-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-175">Ochrana informací v okně pro koncový bod DLP</span><span class="sxs-lookup"><span data-stu-id="b4f5e-175">Window Information Protection for endpoint DLP</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-178">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-178">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="b4f5e-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Správce konfigurace, Správa přístupových práv k Windows)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-181">**Dodržování předpisů**</span><span class="sxs-lookup"><span data-stu-id="b4f5e-181">**Compliance**</span></span>        | | | 
| <span data-ttu-id="b4f5e-182">Neomezená archivace e-mailů</span><span class="sxs-lookup"><span data-stu-id="b4f5e-182">Unlimited email archiving</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-185">Správce dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="b4f5e-185">Compliance Manager</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-188">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="b4f5e-188">eDiscovery</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-191">Blokování a blokování soudních sporů na místě</span><span class="sxs-lookup"><span data-stu-id="b4f5e-191">In-place hold and litigation hold</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b4f5e-194">Značky uchovávání informací a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-194">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="b4f5e-197">\* Uživatelé, kteří mají přiřazený přístup k aplikacím SaaS, mohou získat přístup k jednotnému přihlašování až k 10 aplikacím.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-197">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="b4f5e-198">Správci mohou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednotnému přihlašování je povolený jenom pro 10 aplikací na uživatele najednou.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-198">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="b4f5e-199">Všechny aplikace Office 365 se počítají jako jedna aplikace.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-199">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="b4f5e-200">Migrace</span><span class="sxs-lookup"><span data-stu-id="b4f5e-200">Migration</span></span>

<span data-ttu-id="b4f5e-201">Pokud chcete migrovat, přesuňte předplatné a licence Microsoft 365 Business Premium na vhodné předplatné Microsoft 365 E3 s jeho licencemi.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-201">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="b4f5e-202">Následující části popisují, jaké změny je potřeba udělat, pokud nějaké jsou, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-202">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="b4f5e-203">Konfigurace a data předplatného Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b4f5e-203">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="b4f5e-204">Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, které zahrnují:</span><span class="sxs-lookup"><span data-stu-id="b4f5e-204">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="b4f5e-205">Konfigurace předplatného, například názvy domén DNS.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-205">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="b4f5e-206">Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-206">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="b4f5e-207">Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-207">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="b4f5e-208">Vaši uživatelé teď mohou využívat neomezené úložiště v poštovních schránkách Exchange Online a ve složkách OneDrivu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-208">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="b4f5e-209">Pro více než 10 aplikací můžete začít používat Cloud App Discovery, Azure AD Connect Health a jednotné přihlašování.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-209">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="b4f5e-210">Ochrana před hrozbou</span><span class="sxs-lookup"><span data-stu-id="b4f5e-210">Threat protection</span></span>

<span data-ttu-id="b4f5e-211">Windows 10 Business zahrnuje tyto ochrany:</span><span class="sxs-lookup"><span data-stu-id="b4f5e-211">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="b4f5e-212">Vynucení integrity procesu spouštění operačního systému</span><span class="sxs-lookup"><span data-stu-id="b4f5e-212">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="b4f5e-213">Vynucení integrity citlivých operačních komponent</span><span class="sxs-lookup"><span data-stu-id="b4f5e-213">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="b4f5e-214">Pokročilá zranitelnost a omezení zneužití po nulu</span><span class="sxs-lookup"><span data-stu-id="b4f5e-214">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="b4f5e-215">Ochrana sítě založená na reputaci pro Microsoft Edge, Internet Explorer a Chrome</span><span class="sxs-lookup"><span data-stu-id="b4f5e-215">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="b4f5e-216">Brána firewall založená na hostiteli</span><span class="sxs-lookup"><span data-stu-id="b4f5e-216">Host-based firewall</span></span>
- <span data-ttu-id="b4f5e-217">Zmírnění rizik ransomwaru</span><span class="sxs-lookup"><span data-stu-id="b4f5e-217">Ransomware mitigations</span></span>
- <span data-ttu-id="b4f5e-218">Hardwarová izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b4f5e-218">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="b4f5e-219">Řízení aplikací využívající inteligentní graf zabezpečení</span><span class="sxs-lookup"><span data-stu-id="b4f5e-219">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="b4f5e-220">Řízení zařízení (USB)</span><span class="sxs-lookup"><span data-stu-id="b4f5e-220">Device control (USB)</span></span>
- <span data-ttu-id="b4f5e-221">Ochrana sítě pro webové hrozby</span><span class="sxs-lookup"><span data-stu-id="b4f5e-221">Network protection for web-based threats</span></span>
- <span data-ttu-id="b4f5e-222">Pravidla prevence vniknutí hostitele</span><span class="sxs-lookup"><span data-stu-id="b4f5e-222">Host intrusion prevention rules</span></span>

<span data-ttu-id="b4f5e-223">Windows 10 Enterprise E3 zahrnuje také podnikovou správu hardwarové izolace pro Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-223">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="b4f5e-224">Uživatelé, kteří migrují na Microsoft 365 E3, budou každý z nich vyžadovat licenci Microsoft Defender pro Office 365, aby bylo možné pokračovat v ochraně před hrozbou.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-224">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="b4f5e-225">Nezapomeňte si koupit další licence Defenderu pro Office 365, aby všichni uživatelé, kteří mají v rámci vašeho programu Defender for Office 365 oprávnění, mají licenci.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-225">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="b4f5e-226">Správa zařízení pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="b4f5e-226">Device management with Intune</span></span>

<span data-ttu-id="b4f5e-227">Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-227">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="b4f5e-228">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b4f5e-228">Windows 10</span></span>

<span data-ttu-id="b4f5e-229">Microsoft 365 Business Premium zahrnuje Windows 10 Business, který si můžete nainstalovat pomocí Windows AutoPilota.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-229">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="b4f5e-230">Když migrujete na Microsoft 365 E3, každá uživatelská licence zahrnuje Windows 10 Enterprise E3, který můžete nainstalovat také pomocí Windows Autopilota.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-230">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="b4f5e-231">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="b4f5e-231">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="b4f5e-232">Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních automaticky začne používat funkce aplikací Microsoft 365 pro podniky.</span><span class="sxs-lookup"><span data-stu-id="b4f5e-232">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="b4f5e-233">Po migraci teď můžete použít:</span><span class="sxs-lookup"><span data-stu-id="b4f5e-233">After migration, you can now use:</span></span>

 - <span data-ttu-id="b4f5e-234">Zásady skupiny podpora</span><span class="sxs-lookup"><span data-stu-id="b4f5e-234">Group Policy support</span></span>
 - <span data-ttu-id="b4f5e-235">Porovnání tabulek a dotazování</span><span class="sxs-lookup"><span data-stu-id="b4f5e-235">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="b4f5e-236">Business intelligence</span><span class="sxs-lookup"><span data-stu-id="b4f5e-236">Business intelligence</span></span>

