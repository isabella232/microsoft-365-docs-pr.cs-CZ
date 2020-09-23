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
description: Přečtěte si, jak přesunout firmu z Microsoft 365 Business Premium na Microsoft 365 E3.
ms.openlocfilehash: fbd5c0710bffa92cfc17447094bb9b2683641d5f
ms.sourcegitcommit: c083602dda3cdcb5b58cb8aa070d77019075f765
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "48195513"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="b29f3-103">Migrace z aplikace Microsoft 365 Business Premium na Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="b29f3-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="b29f3-104">Microsoft 365 Business Premium obsahuje vše potřebné pro vaši malou firmu a spojuje aplikace pro práci založené na cloudu co nejlépe ve třídě s jednoduchou správou a zabezpečením zařízení, které umožní zaměstnancům co nejvýhodnější práci.</span><span class="sxs-lookup"><span data-stu-id="b29f3-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="b29f3-105">V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium na Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b29f3-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="b29f3-106">Váš podnik například vyrostl a potřebuje více než 300 licencí (blahopřejení).</span><span class="sxs-lookup"><span data-stu-id="b29f3-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="b29f3-107">Nebo potřebuje vaše firma funkce Enterprise, jako jsou aplikace Microsoft 365 pro podnik, Windows 10 Enterprise E3 nebo licence Enterprise Client Access (CAL).</span><span class="sxs-lookup"><span data-stu-id="b29f3-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="b29f3-108">Snadná inovace: můžete zahájit upgrade [z centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="b29f3-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="b29f3-109">Všechna vaše data a konfigurace ve vašem aktuálním předplatném jsou zachována.</span><span class="sxs-lookup"><span data-stu-id="b29f3-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="b29f3-110">Není nic, co byste chtěli připravit na migraci a nic nedělat, dokud nebudete moci provádět nové funkce.</span><span class="sxs-lookup"><span data-stu-id="b29f3-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="b29f3-111">Můžete také použít předplatné Microsoft 365 Business Premium pro až 300 sedadel a získat předplatné Microsoft 365 E3 pro více než 300 sedadel.</span><span class="sxs-lookup"><span data-stu-id="b29f3-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="b29f3-112">ATP Office 365 však není součástí Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b29f3-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="b29f3-113">Za účelem zachování ochrany proti hrozbám byste měli přidat další licence ATP Office 365, aby všichni uživatelé, kteří jsou v dosahu zásad Office 365 ATP, měli licenci.</span><span class="sxs-lookup"><span data-stu-id="b29f3-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="b29f3-114">Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="b29f3-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="b29f3-115">Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="b29f3-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="b29f3-116">Funkce</span><span class="sxs-lookup"><span data-stu-id="b29f3-116">Feature</span></span>    | <span data-ttu-id="b29f3-117">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b29f3-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="b29f3-118">Podpora v Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="b29f3-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="b29f3-119">**Místní**</span><span class="sxs-lookup"><span data-stu-id="b29f3-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="b29f3-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b29f3-120">Windows 10</span></span>    | <span data-ttu-id="b29f3-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="b29f3-121">Windows 10 Business</span></span>  |     <span data-ttu-id="b29f3-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b29f3-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="b29f3-123">Aplikace Office \*</span><span class="sxs-lookup"><span data-stu-id="b29f3-123">Office apps\*</span></span>    | [<span data-ttu-id="b29f3-124">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="b29f3-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="b29f3-125">Microsoft 365 Apps for enterprise</span><span class="sxs-lookup"><span data-stu-id="b29f3-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="b29f3-126">**Kancelářské aplikace**</span><span class="sxs-lookup"><span data-stu-id="b29f3-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="b29f3-127">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="b29f3-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="b29f3-128">50 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b29f3-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="b29f3-129">100 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b29f3-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="b29f3-130">Teams</span><span class="sxs-lookup"><span data-stu-id="b29f3-130">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-133">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="b29f3-133">OneDrive for Business</span></span>    | <span data-ttu-id="b29f3-134">1 TB limit úložiště na uživatele</span><span class="sxs-lookup"><span data-stu-id="b29f3-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="b29f3-135">Neomezené</span><span class="sxs-lookup"><span data-stu-id="b29f3-135">Unlimited</span></span> | 
| <span data-ttu-id="b29f3-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="b29f3-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-139">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="b29f3-139">Outlook Customer Manager, MileIQ</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="b29f3-141">**Ochrana před hrozbami**</span><span class="sxs-lookup"><span data-stu-id="b29f3-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="b29f3-142">Možnosti pro redukci pro omezení plochy</span><span class="sxs-lookup"><span data-stu-id="b29f3-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="b29f3-143">Podívejte se na tento seznam</span><span class="sxs-lookup"><span data-stu-id="b29f3-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="b29f3-144">Podniková správa izolace hardwaru pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b29f3-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="b29f3-145">Office 365 – Rozšířená ochrana před internetovými útoky (ATP) – plán 1</span><span class="sxs-lookup"><span data-stu-id="b29f3-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="b29f3-147">Není zahrnuto, ale můžete ho přidat</span><span class="sxs-lookup"><span data-stu-id="b29f3-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="b29f3-148">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="b29f3-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="b29f3-149">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), Azure Multi-Factor Authentication (MFA), podmíněný přístup, zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="b29f3-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-152">Zjišťování Cloud App, Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b29f3-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-154">Aplikace Azure AD 365 – jednotné přihlašování (SSO): 10 aplikací na uživatele (Galerie SaaS aplikací, například Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="b29f3-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-157">Jednotné přihlašování k Azure AD Premium 1: bez limitu (místní aplikace prostřednictvím proxy aplikace Azure AD a aplikací mimo galerii s použitím šablon pro samoobslužné integrace aplikací)</span><span class="sxs-lookup"><span data-stu-id="b29f3-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-159">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="b29f3-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="b29f3-160">Microsoft Intune, Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="b29f3-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b29f3-163">Přístup k virtuální ploše (VDA)</span><span class="sxs-lookup"><span data-stu-id="b29f3-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b29f3-165">Virtuální plocha systému Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="b29f3-165">Windows Virtual Desktop (WVD)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="b29f3-168">Aktivace sdíleného počítače (SCA)</span><span class="sxs-lookup"><span data-stu-id="b29f3-168">Shared Computer Activation (SCA)</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-171">Balíček Microsoft Desktop Optimization</span><span class="sxs-lookup"><span data-stu-id="b29f3-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-173">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="b29f3-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="b29f3-174">Ochrana před únikem dat v Office 365, plán Azure Information Protection 1</span><span class="sxs-lookup"><span data-stu-id="b29f3-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-177">Ochrana informací v okně pro službu DLP koncového bodu</span><span class="sxs-lookup"><span data-stu-id="b29f3-177">Window Information Protection for endpoint DLP</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-180">**Licence klientského přístupu (licence CAL)**</span><span class="sxs-lookup"><span data-stu-id="b29f3-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="b29f3-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="b29f3-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-183">**Požadavků**</span><span class="sxs-lookup"><span data-stu-id="b29f3-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="b29f3-184">Časově neomezené archivace e-mailů</span><span class="sxs-lookup"><span data-stu-id="b29f3-184">Unlimited email archiving</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-187">Správce dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="b29f3-187">Compliance Manager</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-190">Sad</span><span class="sxs-lookup"><span data-stu-id="b29f3-190">eDiscovery</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-193">Blokování pro archivaci a držení soudní pře</span><span class="sxs-lookup"><span data-stu-id="b29f3-193">In-place hold and litigation hold</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="b29f3-196">Značky uchování záznamů zpráv a zásady uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="b29f3-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="b29f3-199">\* Uživatelé, kterým byl přiřazen přístup k aplikacím SaaS, můžou získat přístup k jednotnému přihlašování k až 10 aplikacím.</span><span class="sxs-lookup"><span data-stu-id="b29f3-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="b29f3-200">Správci můžou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů na různé aplikace SaaS, ale přístup pomocí jednotného přihlašování je povolený jenom u 10 aplikací na jednoho uživatele najednou.</span><span class="sxs-lookup"><span data-stu-id="b29f3-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="b29f3-201">Všechny aplikace Office 365 se počítají jako jediná aplikace.</span><span class="sxs-lookup"><span data-stu-id="b29f3-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="b29f3-202">Migrace</span><span class="sxs-lookup"><span data-stu-id="b29f3-202">Migration</span></span>

<span data-ttu-id="b29f3-203">Pokud chcete migrovat, spolupracujte se svým partnerem a přesuňte předplatné Microsoft 365 Business Premium a licence na vhodný tarif Microsoft 365 E3 s jeho licencemi.</span><span class="sxs-lookup"><span data-stu-id="b29f3-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="b29f3-204">V následujících částech jsou popsány změny, které je třeba udělat, pokud existují, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="b29f3-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="b29f3-205">Konfigurace a data předplatného Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b29f3-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="b29f3-206">Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, což zahrnuje:</span><span class="sxs-lookup"><span data-stu-id="b29f3-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="b29f3-207">Konfigurace předplatného, třeba názvy domén DNS.</span><span class="sxs-lookup"><span data-stu-id="b29f3-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="b29f3-208">Účty uživatelů a skupin a nastavení ověřování, například vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="b29f3-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="b29f3-209">Konfigurace produktivity služeb a jejich data, například týmy, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="b29f3-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="b29f3-210">Uživatelé teď můžou využívat neomezené úložiště v poštovních schránkách Exchange Online a složkách OneDrivu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="b29f3-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="b29f3-211">Můžete začít používat vyhledávání Cloud App Appu, stav Azure AD Connect a jednotné přihlašování pro více než 10 aplikací.</span><span class="sxs-lookup"><span data-stu-id="b29f3-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="b29f3-212">Uživatelé migrace do Microsoft 365 E3 už nemůžou používat Outlook Customer Manager a MileIQ.</span><span class="sxs-lookup"><span data-stu-id="b29f3-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="b29f3-213">Ochrana před hrozbami</span><span class="sxs-lookup"><span data-stu-id="b29f3-213">Threat protection</span></span>

<span data-ttu-id="b29f3-214">Windows 10 Business zahrnuje tyto ochrany:</span><span class="sxs-lookup"><span data-stu-id="b29f3-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="b29f3-215">Vynucení integrity procesu spuštění operačního systému</span><span class="sxs-lookup"><span data-stu-id="b29f3-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="b29f3-216">Vynucení integrity citlivých provozních součástí</span><span class="sxs-lookup"><span data-stu-id="b29f3-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="b29f3-217">Zdokonalená řešení chyb a zneužití nulového počtu dnů</span><span class="sxs-lookup"><span data-stu-id="b29f3-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="b29f3-218">Ochrana sítě založená na pověsti pro Microsoft Edge, Internet Explorer a Chrome</span><span class="sxs-lookup"><span data-stu-id="b29f3-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="b29f3-219">Hostitelská brána firewall</span><span class="sxs-lookup"><span data-stu-id="b29f3-219">Host-based firewall</span></span>
- <span data-ttu-id="b29f3-220">Ransomwaru Zklidňující fakta</span><span class="sxs-lookup"><span data-stu-id="b29f3-220">Ransomware mitigations</span></span>
- <span data-ttu-id="b29f3-221">Hardwarově izolovaná izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b29f3-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="b29f3-222">Řízení aplikací poháněné grafem inteligentního zabezpečení</span><span class="sxs-lookup"><span data-stu-id="b29f3-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="b29f3-223">Ovládání zařízení (USB)</span><span class="sxs-lookup"><span data-stu-id="b29f3-223">Device control (USB)</span></span>
- <span data-ttu-id="b29f3-224">Ochrana sítě pro webové hrozby</span><span class="sxs-lookup"><span data-stu-id="b29f3-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="b29f3-225">Pravidla prevence vniknutí hostitele</span><span class="sxs-lookup"><span data-stu-id="b29f3-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="b29f3-226">Windows 10 Enterprise E3 zahrnuje také podnikovou správu izolace hardwaru pro Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b29f3-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="b29f3-227">Uživatelé, kteří jsou migrováni do Microsoft 365 E3, budou mít licenci ATP Office 365 pro pokračování ochrany před hrozbami.</span><span class="sxs-lookup"><span data-stu-id="b29f3-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="b29f3-228">Nezapomeňte si koupit další licence pro Office 365 ATP, aby všichni uživatelé, kteří jsou v dosahu zásad Office 365 ATP, měli licenci.</span><span class="sxs-lookup"><span data-stu-id="b29f3-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="b29f3-229">Správa zařízení s Intune</span><span class="sxs-lookup"><span data-stu-id="b29f3-229">Device management with Intune</span></span>

<span data-ttu-id="b29f3-230">Před migrací nemusíte dělat žádné změny v aktuální konfiguraci Intune, včetně zaregistrovaných zařízení a nastavení zařízení a aplikací.</span><span class="sxs-lookup"><span data-stu-id="b29f3-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="b29f3-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b29f3-231">Windows 10</span></span>

<span data-ttu-id="b29f3-232">Microsoft 365 Business Premium zahrnuje Windows 10 Business, který se dá nainstalovat s autopilotem Windows.</span><span class="sxs-lookup"><span data-stu-id="b29f3-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="b29f3-233">Když migrujete na Microsoft 365 E3, každá uživatelská licence obsahuje Windows 10 Enterprise E3, který se dá taky nainstalovat s autopilotem Windows.</span><span class="sxs-lookup"><span data-stu-id="b29f3-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="b29f3-234">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="b29f3-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="b29f3-235">Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních bude automaticky používat funkce aplikací Microsoft 365 pro podnik.</span><span class="sxs-lookup"><span data-stu-id="b29f3-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="b29f3-236">Po migraci můžete použít:</span><span class="sxs-lookup"><span data-stu-id="b29f3-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="b29f3-237">Aktivace multilicence prostřednictvím zásad skupiny</span><span class="sxs-lookup"><span data-stu-id="b29f3-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="b29f3-238">Telemetrie aplikací</span><span class="sxs-lookup"><span data-stu-id="b29f3-238">App telemetry</span></span>
 - <span data-ttu-id="b29f3-239">Aktualizace ovládacích prvků</span><span class="sxs-lookup"><span data-stu-id="b29f3-239">Update controls</span></span>
 - <span data-ttu-id="b29f3-240">Porovnání tabulky a dotazy</span><span class="sxs-lookup"><span data-stu-id="b29f3-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="b29f3-241">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="b29f3-241">Business intelligence</span></span>

