---
title: Migrace z Microsoftu 365 Business do Microsoftu 365 E3
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
description: Přečtěte si, jak přesunout svou firmu z Microsoft 365 Business Premium do Microsoftu 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081795"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="5237c-103">Migrace z Microsoftu 365 Business Premium do Microsoftu 365 E3</span><span class="sxs-lookup"><span data-stu-id="5237c-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="5237c-104">Microsoft 365 Business Premium má vše, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace ve své třídě s jednoduchou správou zařízení a zabezpečením, které vašim zaměstnancům umožní odváděli nejlepší práci.</span><span class="sxs-lookup"><span data-stu-id="5237c-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="5237c-105">V některých případech však může být nutné migrovat předplatné Microsoft 365 Business Premium do Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5237c-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="5237c-106">Vaše firma se například rozrostla a potřebuje více než 300 licencí (mimochodem blahopřejeme).</span><span class="sxs-lookup"><span data-stu-id="5237c-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="5237c-107">Nebo vaše firma potřebuje podnikové funkce, jako jsou aplikace Microsoft 365 pro podniky, Windows 10 Enterprise E3 nebo licence enterprise client access (CAL).</span><span class="sxs-lookup"><span data-stu-id="5237c-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="5237c-108">Upgrade je snadný: upgrade můžete spustit [z Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="5237c-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="5237c-109">Všechna vaše data a konfigurace v aktuálním předplatném jsou zachována.</span><span class="sxs-lookup"><span data-stu-id="5237c-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="5237c-110">Není nic, co byste měli udělat, abyste se připravili na migraci, a nic dělat později, kromě využití nových funkcí.</span><span class="sxs-lookup"><span data-stu-id="5237c-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="5237c-111">Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí.</span><span class="sxs-lookup"><span data-stu-id="5237c-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="5237c-112">Však Office 365 ATP není součástí Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5237c-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="5237c-113">Chcete-li pokračovat v ochraně před hrozbami, měli byste přidat další licence office 365 ATP, aby měli licenci všichni uživatelé v rozsahu vašich policistů ochrany ATP Office 365.</span><span class="sxs-lookup"><span data-stu-id="5237c-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="5237c-114">Rozdíly mezi Microsoftem 365 Business Premium a Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="5237c-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="5237c-115">Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5237c-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="5237c-116">Funkce</span><span class="sxs-lookup"><span data-stu-id="5237c-116">Feature</span></span>    | <span data-ttu-id="5237c-117">Podpora v Microsoftu 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5237c-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="5237c-118">Podpora v Microsoftu 365 E3</span><span class="sxs-lookup"><span data-stu-id="5237c-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="5237c-119">**Místní**</span><span class="sxs-lookup"><span data-stu-id="5237c-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="5237c-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5237c-120">Windows 10</span></span>    | <span data-ttu-id="5237c-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="5237c-121">Windows 10 Business</span></span>  |     <span data-ttu-id="5237c-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="5237c-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="5237c-123">Aplikace Office\*</span><span class="sxs-lookup"><span data-stu-id="5237c-123">Office apps\*</span></span>    | [<span data-ttu-id="5237c-124">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="5237c-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="5237c-125">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="5237c-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="5237c-126">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="5237c-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="5237c-127">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="5237c-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="5237c-128">Limit úložiště 50 GB na poštovní schránku a neomezená archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5237c-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="5237c-129">Limit úložiště 100 GB na poštovní schránku a neomezená archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5237c-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="5237c-130">Týmy</span><span class="sxs-lookup"><span data-stu-id="5237c-130">Teams</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-133">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="5237c-133">OneDrive for Business</span></span>    | <span data-ttu-id="5237c-134">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="5237c-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="5237c-135">Neomezené</span><span class="sxs-lookup"><span data-stu-id="5237c-135">Unlimited</span></span> | 
| <span data-ttu-id="5237c-136">Yammer, SharePoint Online, Plánovač, Stream</span><span class="sxs-lookup"><span data-stu-id="5237c-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-139">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="5237c-139">Outlook Customer Manager, MileIQ</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="5237c-141">**Ochrana před hrozbami**</span><span class="sxs-lookup"><span data-stu-id="5237c-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="5237c-142">Možnosti redukce povrchu útoku</span><span class="sxs-lookup"><span data-stu-id="5237c-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="5237c-143">Podívejte se na tento seznam</span><span class="sxs-lookup"><span data-stu-id="5237c-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="5237c-144">Podniková správa hardwarové izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5237c-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="5237c-145">Plán 1 pokročilé ochrany před hrozbami Office 365</span><span class="sxs-lookup"><span data-stu-id="5237c-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="5237c-147">Není zahrnuto, ale může být přidáno na</span><span class="sxs-lookup"><span data-stu-id="5237c-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="5237c-148">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="5237c-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="5237c-149">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure (MFA), podmíněný přístup, zpětný zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="5237c-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-152">Zjišťování cloudových aplikací, azure ad connect stav</span><span class="sxs-lookup"><span data-stu-id="5237c-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-154">Jednotné přihlašení aplikací Azure AD Office 365 (jednotné přihlašení): 10 aplikací na uživatele (aplikace Galerie SaaS, jako je Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="5237c-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-157">Azure AD Premium 1 SSO: bez omezení (místní aplikace prostřednictvím azure ad application proxy a non-galerie aplikace pomocí samoobslužné šablony integrace aplikací)</span><span class="sxs-lookup"><span data-stu-id="5237c-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-159">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="5237c-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="5237c-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="5237c-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5237c-163">Přístup k virtuální ploše (VDA)</span><span class="sxs-lookup"><span data-stu-id="5237c-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5237c-165">Virtuální plocha systému Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="5237c-165">Windows Virtual Desktop (WVD)</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5237c-168">Aktivace sdíleného počítače (SCA)</span><span class="sxs-lookup"><span data-stu-id="5237c-168">Shared Computer Activation (SCA)</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-171">Balíček optimalizace pro stolní počítače společnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="5237c-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-173">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="5237c-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="5237c-174">Office 365 Ochrana před ztrátou dat, Plán ochrany informací Azure 1</span><span class="sxs-lookup"><span data-stu-id="5237c-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-177">Ochrana informací o okně pro dlp koncového bodu</span><span class="sxs-lookup"><span data-stu-id="5237c-177">Window Information Protection for endpoint DLP</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-180">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="5237c-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="5237c-181">Sada Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Správa práv systému Windows)</span><span class="sxs-lookup"><span data-stu-id="5237c-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-183">**Dodržování**</span><span class="sxs-lookup"><span data-stu-id="5237c-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="5237c-184">Neomezená archivace e-mailů</span><span class="sxs-lookup"><span data-stu-id="5237c-184">Unlimited email archiving</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-187">Skóre dodržování předpisů/Správce dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="5237c-187">Compliance Score/Compliance Manager</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-190">Ediscovery</span><span class="sxs-lookup"><span data-stu-id="5237c-190">eDiscovery</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-193">Blokování na místě a blokování ze soudních sporů</span><span class="sxs-lookup"><span data-stu-id="5237c-193">In-place hold and litigation hold</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5237c-196">Retenční značky a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM) a zásady uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="5237c-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="5237c-199">\*Uživatelé, kterým byl přiřazen přístup k aplikacím SaaS, mohou získat přístup k návěsům až pro 10 aplikací.</span><span class="sxs-lookup"><span data-stu-id="5237c-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="5237c-200">Správci můžou konfigurovat jednosadové služby a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednoodvolům je povolen jenom pro 10 aplikací na uživatele najednou.</span><span class="sxs-lookup"><span data-stu-id="5237c-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="5237c-201">Všechny aplikace Office 365 se počítají jako jedna aplikace.</span><span class="sxs-lookup"><span data-stu-id="5237c-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="5237c-202">Migrace</span><span class="sxs-lookup"><span data-stu-id="5237c-202">Migration</span></span>

<span data-ttu-id="5237c-203">Chcete-li migrovat, spolupracujte se svým partnerem na přesunutí předplatného a licencí Microsoft 365 Business Premium do vhodného předplatného Microsoft 365 E3 s jeho licencemi.</span><span class="sxs-lookup"><span data-stu-id="5237c-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="5237c-204">Následující části popisují, jaké změny je třeba provést, pokud existuje, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="5237c-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="5237c-205">Konfigurace předplatného Microsoftu 365 a data</span><span class="sxs-lookup"><span data-stu-id="5237c-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="5237c-206">Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, což zahrnuje:</span><span class="sxs-lookup"><span data-stu-id="5237c-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="5237c-207">Konfigurace předplatného, například názvy domén DNS.</span><span class="sxs-lookup"><span data-stu-id="5237c-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="5237c-208">Uživatelské a skupinové účty a nastavení ověřování, jako je například vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="5237c-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="5237c-209">Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="5237c-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="5237c-210">Vaši uživatelé teď můžou využívat neomezené úložiště v poštovních schránkách Exchange Online a ve složkách OneDrivu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="5237c-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="5237c-211">Můžete začít používat Cloud App Discovery, Azure AD Connect Health a SSO pro více než 10 aplikací.</span><span class="sxs-lookup"><span data-stu-id="5237c-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="5237c-212">Uživatelé migrovaní na Microsoft 365 E3 již nemohou používat Správce zákazníků aplikace Outlook a MileIQ.</span><span class="sxs-lookup"><span data-stu-id="5237c-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="5237c-213">Ochrana před hrozbami</span><span class="sxs-lookup"><span data-stu-id="5237c-213">Threat protection</span></span>

<span data-ttu-id="5237c-214">Windows 10 Business zahrnuje tyto ochrany:</span><span class="sxs-lookup"><span data-stu-id="5237c-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="5237c-215">Vynucení integrity procesu spouštění operačního systému</span><span class="sxs-lookup"><span data-stu-id="5237c-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="5237c-216">Prosazování integrity citlivých provozních součástí</span><span class="sxs-lookup"><span data-stu-id="5237c-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="5237c-217">Pokročilá chyba zabezpečení a skutečnosti snižující závažnost rizika zneužití nultého dne</span><span class="sxs-lookup"><span data-stu-id="5237c-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="5237c-218">Ochrana sítě založená na reputaci pro Microsoft Edge, Internet Explorer a Chrome</span><span class="sxs-lookup"><span data-stu-id="5237c-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="5237c-219">Brána firewall založená na hostiteli</span><span class="sxs-lookup"><span data-stu-id="5237c-219">Host-based firewall</span></span>
- <span data-ttu-id="5237c-220">Skutečnosti snižující závažnost rizika ransomwaru</span><span class="sxs-lookup"><span data-stu-id="5237c-220">Ransomware mitigations</span></span>
- <span data-ttu-id="5237c-221">Hardwarová izolace pro Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5237c-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="5237c-222">Řízení aplikací poháněné grafem inteligentního zabezpečení</span><span class="sxs-lookup"><span data-stu-id="5237c-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="5237c-223">Ovládání zařízení (USB)</span><span class="sxs-lookup"><span data-stu-id="5237c-223">Device control (USB)</span></span>
- <span data-ttu-id="5237c-224">Ochrana sítě před webovými hrozbami</span><span class="sxs-lookup"><span data-stu-id="5237c-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="5237c-225">Pravidla prevence narušení hostitele</span><span class="sxs-lookup"><span data-stu-id="5237c-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="5237c-226">Windows 10 Enterprise E3 také zahrnuje podnikovou správu hardwarové izolace pro Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5237c-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="5237c-227">Uživatelé migrované na Microsoft 365 E3 budou potřebovat licenci Office 365 ATP pro trvalou ochranu před hrozbami.</span><span class="sxs-lookup"><span data-stu-id="5237c-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="5237c-228">Nezapomeňte zakoupit další licence Office 365 ATP, aby všichni uživatelé v rozsahu vašich policistů office 365 ATP získali licenci.</span><span class="sxs-lookup"><span data-stu-id="5237c-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="5237c-229">Správa zařízení s Intune</span><span class="sxs-lookup"><span data-stu-id="5237c-229">Device management with Intune</span></span>

<span data-ttu-id="5237c-230">Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.</span><span class="sxs-lookup"><span data-stu-id="5237c-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="5237c-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5237c-231">Windows 10</span></span>

<span data-ttu-id="5237c-232">Microsoft 365 Business Premium obsahuje Windows 10 Business, který můžete nainstalovat pomocí Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5237c-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="5237c-233">Při migraci na Microsoft 365 E3 obsahuje každá uživatelská licence Windows 10 Enterprise E3, který můžete nainstalovat také pomocí programu Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5237c-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="5237c-234">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="5237c-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="5237c-235">Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních začne automaticky používat funkce Aplikací Microsoft 365 pro podniky.</span><span class="sxs-lookup"><span data-stu-id="5237c-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="5237c-236">Po migraci můžete nyní použít:</span><span class="sxs-lookup"><span data-stu-id="5237c-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="5237c-237">Aktivace svazku prostřednictvím zásad skupiny</span><span class="sxs-lookup"><span data-stu-id="5237c-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="5237c-238">Telemetrie aplikací</span><span class="sxs-lookup"><span data-stu-id="5237c-238">App telemetry</span></span>
 - <span data-ttu-id="5237c-239">Aktualizovat ovládací prvky</span><span class="sxs-lookup"><span data-stu-id="5237c-239">Update controls</span></span>
 - <span data-ttu-id="5237c-240">Porovnání a dotazování v tabulkovém procesoru</span><span class="sxs-lookup"><span data-stu-id="5237c-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="5237c-241">Business intelligence</span><span class="sxs-lookup"><span data-stu-id="5237c-241">Business intelligence</span></span>

