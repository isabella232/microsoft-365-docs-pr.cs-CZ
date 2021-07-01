---
title: Migrace z Microsoft 365 Business na Microsoft 365 E3
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
description: Zjistěte, jak přesunout svou firmu z Microsoft 365 Business Premium do Microsoft 365 E3.
ms.openlocfilehash: 6502d79dbb283db37b00e4fccf89b15ab4291ce5
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227613"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="43dad-103">Migrace z Microsoft 365 Business Premium na Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="43dad-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="43dad-104">Microsoft 365 Business Premium má všechno, co potřebujete pro svoji malou firmu, a kombinuje nejlepší cloudové aplikace na bázi produktivity ve své třídě s jednoduchou snadná správa zařízení a zabezpečení, které vašim zaměstnancům umožňují dělat svou nejlepší práci.</span><span class="sxs-lookup"><span data-stu-id="43dad-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="43dad-105">V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium do Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="43dad-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span>

<span data-ttu-id="43dad-106">Vaše firma například roste a potřebuje víc než 300 licencí (mimochodem blahopřejeme).</span><span class="sxs-lookup"><span data-stu-id="43dad-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="43dad-107">Nebo vaše firma potřebuje podnikové funkce, jako jsou Microsoft 365 Apps pro velké organizace, Windows 10 Enterprise E3 nebo Enterprise klientského přístupu (CAL).</span><span class="sxs-lookup"><span data-stu-id="43dad-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="43dad-108">Upgrade je snadný: Upgrade můžete spustit z [Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="43dad-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="43dad-109">Všechna vaše data a konfigurace v aktuálním předplatném se zachová.</span><span class="sxs-lookup"><span data-stu-id="43dad-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="43dad-110">Není nic, co byste měli udělat, abyste se připravili na migraci a potom nic dělat, kromě využití nových funkcí.</span><span class="sxs-lookup"><span data-stu-id="43dad-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

> [!NOTE]
> <span data-ttu-id="43dad-111">Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí.</span><span class="sxs-lookup"><span data-stu-id="43dad-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="43dad-112">Program Microsoft Defender pro Office 365 ale není součástí Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="43dad-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="43dad-113">Pokud chcete pokračovat v ochraně před hrozbami, měli byste přidat další defender pro Office 365, aby všichni uživatelé v rozsahu vašeho Defenderu pro Office 365 měli licenci.</span><span class="sxs-lookup"><span data-stu-id="43dad-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="43dad-114">Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="43dad-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="43dad-115">Tato tabulka zobrazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="43dad-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="43dad-116">Funkce</span><span class="sxs-lookup"><span data-stu-id="43dad-116">Feature</span></span>    | <span data-ttu-id="43dad-117">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="43dad-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="43dad-118">Podpora v Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="43dad-118">Support in Microsoft 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="43dad-119">**Místní**</span><span class="sxs-lookup"><span data-stu-id="43dad-119">**On-premises**</span></span>        | | |
| <span data-ttu-id="43dad-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="43dad-120">Windows 10</span></span>    | <span data-ttu-id="43dad-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="43dad-121">Windows 10 Business</span></span>  |     <span data-ttu-id="43dad-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="43dad-122">Windows 10 Enterprise E3</span></span>|
| <span data-ttu-id="43dad-123">Office aplikace\*</span><span class="sxs-lookup"><span data-stu-id="43dad-123">Office apps\*</span></span>    | [<span data-ttu-id="43dad-124">Microsoft 365 Apps pro firmy</span><span class="sxs-lookup"><span data-stu-id="43dad-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="43dad-125">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="43dad-125">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="43dad-126">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="43dad-126">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="43dad-127">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="43dad-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="43dad-128">Limit úložiště 50 GB na poštovní schránku a neomezená Exchange Online archivace</span><span class="sxs-lookup"><span data-stu-id="43dad-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="43dad-129">Limit úložiště 100 GB na poštovní schránku a neomezená Exchange Online archivace</span><span class="sxs-lookup"><span data-stu-id="43dad-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> |
| <span data-ttu-id="43dad-130">Teams</span><span class="sxs-lookup"><span data-stu-id="43dad-130">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-133">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="43dad-133">OneDrive for Business</span></span>    | <span data-ttu-id="43dad-134">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="43dad-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="43dad-135">Neomezená</span><span class="sxs-lookup"><span data-stu-id="43dad-135">Unlimited</span></span> |
| <span data-ttu-id="43dad-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="43dad-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-139">**Ochrana před hrozbou**</span><span class="sxs-lookup"><span data-stu-id="43dad-139">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="43dad-140">Možnosti omezení útoku na povrch</span><span class="sxs-lookup"><span data-stu-id="43dad-140">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="43dad-141">Zobrazit tento seznam</span><span class="sxs-lookup"><span data-stu-id="43dad-141">See this list</span></span>](#threat-protection) | <span data-ttu-id="43dad-142">Enterprise správy hardwarové izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="43dad-142">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> |
| <span data-ttu-id="43dad-143">Defender pro Office 365 Plán 1</span><span class="sxs-lookup"><span data-stu-id="43dad-143">Defender for Office 365 Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="43dad-145">Není zahrnuto, ale může být přidáno dne</span><span class="sxs-lookup"><span data-stu-id="43dad-145">Not included, but can be added on</span></span> |
| <span data-ttu-id="43dad-146">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="43dad-146">**Identity management**</span></span>        | | |
| <span data-ttu-id="43dad-147">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="43dad-147">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-150">Zjišťování cloudových aplikací, Azure AD Připojení Health</span><span class="sxs-lookup"><span data-stu-id="43dad-150">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-152">Aplikace Azure AD Office 365 Sign-On jednotné přihlašování (SSO): 10 aplikací na uživatele (aplikace Gallery SaaS, jako je Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="43dad-152">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-155">Azure AD Premium 1 jednotné přihlašování: bez omezení (místní aplikace prostřednictvím Proxy aplikací Azure AD a aplikací mimo galerii pomocí šablon Self-Service Integrace aplikací)</span><span class="sxs-lookup"><span data-stu-id="43dad-155">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-157">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="43dad-157">**Device and app management**</span></span>        | | |
| <span data-ttu-id="43dad-158">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="43dad-158">Microsoft Intune, Windows Autopilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="43dad-161">Přístup k virtuální ploše (VDA)</span><span class="sxs-lookup"><span data-stu-id="43dad-161">Virtual Desktop Access (VDA)</span></span>    |  |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="43dad-163">Windows Virtuální plocha (WVD)</span><span class="sxs-lookup"><span data-stu-id="43dad-163">Windows Virtual Desktop (WVD)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="43dad-166">Aktivace sdíleného počítače (SCA)</span><span class="sxs-lookup"><span data-stu-id="43dad-166">Shared Computer Activation (SCA)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-169">Microsoft Desktop Optimization Package</span><span class="sxs-lookup"><span data-stu-id="43dad-169">Microsoft Desktop Optimization Package</span></span>    | |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-171">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="43dad-171">**Information protection**</span></span>        | | |
| <span data-ttu-id="43dad-172">Office 365 Ochrana před únikem dat, Plán ochrany informací v Azure 1</span><span class="sxs-lookup"><span data-stu-id="43dad-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-175">Ochrana informací v okně pro koncový bod DLP</span><span class="sxs-lookup"><span data-stu-id="43dad-175">Window Information Protection for endpoint DLP</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-178">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="43dad-178">**Client Access License (CAL rights)**</span></span>    | | |
| <span data-ttu-id="43dad-179">Enterprise Cal Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="43dad-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-181">**Dodržování předpisů**</span><span class="sxs-lookup"><span data-stu-id="43dad-181">**Compliance**</span></span>        | | |
| <span data-ttu-id="43dad-182">Neomezená archivace e-mailů</span><span class="sxs-lookup"><span data-stu-id="43dad-182">Unlimited email archiving</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-185">Správce dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="43dad-185">Compliance Manager</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-188">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="43dad-188">eDiscovery</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-191">Blokování a blokování soudních sporů na místě</span><span class="sxs-lookup"><span data-stu-id="43dad-191">In-place hold and litigation hold</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="43dad-194">Značky uchovávání informací a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM)</span><span class="sxs-lookup"><span data-stu-id="43dad-194">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
||||

<span data-ttu-id="43dad-197">\* Uživatelé, kteří mají přiřazený přístup k aplikacím SaaS, mohou získat přístup k jednotnému přihlašování až k 10 aplikacím.</span><span class="sxs-lookup"><span data-stu-id="43dad-197">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="43dad-198">Správci mohou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednotnému přihlašování je povolený jenom pro 10 aplikací na uživatele najednou.</span><span class="sxs-lookup"><span data-stu-id="43dad-198">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="43dad-199">Všechny Office 365 aplikace se počítají jako jedna aplikace.</span><span class="sxs-lookup"><span data-stu-id="43dad-199">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="43dad-200">Migrace</span><span class="sxs-lookup"><span data-stu-id="43dad-200">Migration</span></span>

<span data-ttu-id="43dad-201">Pokud chcete migrovat, můžete spolupracovat se svým partnerem a přesunout Microsoft 365 Business Premium předplatné a licence na vhodné předplatné Microsoft 365 E3 s jeho licencemi.</span><span class="sxs-lookup"><span data-stu-id="43dad-201">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="43dad-202">Následující části popisují, jaké změny je potřeba udělat, pokud nějaké jsou, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="43dad-202">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="43dad-203">Microsoft 365 a data předplatného</span><span class="sxs-lookup"><span data-stu-id="43dad-203">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="43dad-204">Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, které zahrnují:</span><span class="sxs-lookup"><span data-stu-id="43dad-204">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="43dad-205">Konfigurace předplatného, například názvy domén DNS.</span><span class="sxs-lookup"><span data-stu-id="43dad-205">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="43dad-206">Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="43dad-206">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="43dad-207">Konfigurace služeb produktivity a jejich data, jako jsou Teams, Exchange Online poštovní schránky, weby SharePoint Online, OneDrive pro firmy složky a OneNote poznámkové bloky.</span><span class="sxs-lookup"><span data-stu-id="43dad-207">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="43dad-208">Vaši uživatelé teď mohou využívat neomezené úložiště v Exchange Online poštovních schránkách a OneDrive pro firmy složkách.</span><span class="sxs-lookup"><span data-stu-id="43dad-208">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="43dad-209">Pro více než 10 aplikací můžete začít používat Cloud App Discovery, Azure AD Připojení Health a jednotné přihlašování.</span><span class="sxs-lookup"><span data-stu-id="43dad-209">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="43dad-210">Ochrana před hrozbou</span><span class="sxs-lookup"><span data-stu-id="43dad-210">Threat protection</span></span>

<span data-ttu-id="43dad-211">Windows 10 Business zahrnuje tyto ochrany:</span><span class="sxs-lookup"><span data-stu-id="43dad-211">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="43dad-212">Vynucení integrity procesu spouštění operačního systému</span><span class="sxs-lookup"><span data-stu-id="43dad-212">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="43dad-213">Vynucení integrity citlivých operačních komponent</span><span class="sxs-lookup"><span data-stu-id="43dad-213">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="43dad-214">Pokročilá zranitelnost a omezení zneužití po nulu</span><span class="sxs-lookup"><span data-stu-id="43dad-214">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="43dad-215">Ochrana sítě založená na reputaci pro Microsoft Edge, Internet Explorer a Chrome</span><span class="sxs-lookup"><span data-stu-id="43dad-215">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="43dad-216">Brána firewall založená na hostiteli</span><span class="sxs-lookup"><span data-stu-id="43dad-216">Host-based firewall</span></span>
- <span data-ttu-id="43dad-217">Zmírnění rizik ransomwaru</span><span class="sxs-lookup"><span data-stu-id="43dad-217">Ransomware mitigations</span></span>
- <span data-ttu-id="43dad-218">Hardwarová izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="43dad-218">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="43dad-219">Řízení aplikací využívající inteligentní zabezpečení Graph</span><span class="sxs-lookup"><span data-stu-id="43dad-219">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="43dad-220">Řízení zařízení (USB)</span><span class="sxs-lookup"><span data-stu-id="43dad-220">Device control (USB)</span></span>
- <span data-ttu-id="43dad-221">Ochrana sítě pro webové hrozby</span><span class="sxs-lookup"><span data-stu-id="43dad-221">Network protection for web-based threats</span></span>
- <span data-ttu-id="43dad-222">Pravidla prevence vniknutí hostitele</span><span class="sxs-lookup"><span data-stu-id="43dad-222">Host intrusion prevention rules</span></span>

<span data-ttu-id="43dad-223">Windows 10 Enterprise E3 zahrnuje také podnikovou správu hardwarové izolace pro Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="43dad-223">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

> [!NOTE]
> <span data-ttu-id="43dad-224">Uživatelé migrované do Microsoft 365 E3 budou pro další ochranu před hrozbou vyžadovat licenci Microsoft Defender Office 365 ochranu před internetovou hrozbou.</span><span class="sxs-lookup"><span data-stu-id="43dad-224">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="43dad-225">Nezapomeňte si koupit další defender pro Office 365 licencí, aby všichni uživatelé v rozsahu vašeho Defenderu pro Office 365 licencí.</span><span class="sxs-lookup"><span data-stu-id="43dad-225">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

### <a name="device-management-with-intune"></a><span data-ttu-id="43dad-226">Správa zařízení pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="43dad-226">Device management with Intune</span></span>

<span data-ttu-id="43dad-227">Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.</span><span class="sxs-lookup"><span data-stu-id="43dad-227">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="43dad-228">Windows 10</span><span class="sxs-lookup"><span data-stu-id="43dad-228">Windows 10</span></span>

<span data-ttu-id="43dad-229">Microsoft 365 Business Premium obsahuje Windows 10 Business, které můžete nainstalovat pomocí Windows AutoPilota.</span><span class="sxs-lookup"><span data-stu-id="43dad-229">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="43dad-230">Když migrujete na Microsoft 365 E3, každá uživatelská licence obsahuje Windows 10 Enterprise E3, kterou můžete nainstalovat také pomocí Windows Autopilota.</span><span class="sxs-lookup"><span data-stu-id="43dad-230">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="43dad-231">Microsoft 365 Apps pro firmy</span><span class="sxs-lookup"><span data-stu-id="43dad-231">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="43dad-232">Váš Microsoft 365 Apps pro firmy klient nainstalovaný na vašich zařízeních automaticky začne používat funkce Microsoft 365 Apps pro velké organizace.</span><span class="sxs-lookup"><span data-stu-id="43dad-232">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="43dad-233">Po migraci teď můžete použít:</span><span class="sxs-lookup"><span data-stu-id="43dad-233">After migration, you can now use:</span></span>

- <span data-ttu-id="43dad-234">Zásady skupiny podpora</span><span class="sxs-lookup"><span data-stu-id="43dad-234">Group Policy support</span></span>
- <span data-ttu-id="43dad-235">Porovnání tabulek a dotazování</span><span class="sxs-lookup"><span data-stu-id="43dad-235">Spreadsheet compare and inquire</span></span>
- <span data-ttu-id="43dad-236">Business intelligence</span><span class="sxs-lookup"><span data-stu-id="43dad-236">Business intelligence</span></span>
