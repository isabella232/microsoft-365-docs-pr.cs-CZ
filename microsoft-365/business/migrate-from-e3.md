---
title: Migrace na Microsoft 365 Business z Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Zjistěte, jak přesunout firmu do Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: f08b054473fdd63ec2372e81c776a1b64f89fe9d
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244830"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="613c5-103">Migrace z Office 365 E3 na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="613c5-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="613c5-104">Microsoft 365 Business Premium má všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové produktivní aplikace s jednoduchou snadná správa a zabezpečení zařízení.</span><span class="sxs-lookup"><span data-stu-id="613c5-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="613c5-105">Pokud máte aktuálně předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="613c5-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="613c5-106">Migrace je snadná: Nejdřív přepnete licence a všechna data a informace o uživatelích v aktuálním předplatném se zachová.</span><span class="sxs-lookup"><span data-stu-id="613c5-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="613c5-107">Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="613c5-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="613c5-108">Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="613c5-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="613c5-109">Tato tabulka zobrazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="613c5-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="613c5-110">Funkce</span><span class="sxs-lookup"><span data-stu-id="613c5-110">Feature</span></span>    | <span data-ttu-id="613c5-111">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="613c5-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="613c5-112">Podpora v Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="613c5-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="613c5-113">**Místní**</span><span class="sxs-lookup"><span data-stu-id="613c5-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="613c5-114">Office aplikace<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="613c5-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="613c5-115">Microsoft 365 Apps pro firmy</span><span class="sxs-lookup"><span data-stu-id="613c5-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="613c5-116">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="613c5-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="613c5-117">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="613c5-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="613c5-118">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="613c5-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="613c5-119">Limit úložiště 50 GB na poštovní schránku a neomezený počet Exchange Online – archiv</span><span class="sxs-lookup"><span data-stu-id="613c5-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="613c5-120">Limit úložiště 100 GB na poštovní schránku a neomezený počet Exchange Online – archiv</span><span class="sxs-lookup"><span data-stu-id="613c5-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="613c5-121">Teams</span><span class="sxs-lookup"><span data-stu-id="613c5-121">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="613c5-124">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="613c5-124">OneDrive for Business</span></span>    | <span data-ttu-id="613c5-125">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="613c5-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="613c5-126">Neomezená</span><span class="sxs-lookup"><span data-stu-id="613c5-126">Unlimited</span></span> | 
| <span data-ttu-id="613c5-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="613c5-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="613c5-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="613c5-130">StaffHub</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="613c5-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="613c5-133">MileIQ</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="613c5-135">**Ochrana před hrozbou**</span><span class="sxs-lookup"><span data-stu-id="613c5-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="613c5-136">Defender pro Office 365 Plán 1</span><span class="sxs-lookup"><span data-stu-id="613c5-136">Defender for Office 365 Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="613c5-138">Není zahrnuto, ale může být přidáno dne</span><span class="sxs-lookup"><span data-stu-id="613c5-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="613c5-139">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="613c5-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="613c5-140">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="613c5-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="613c5-142">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="613c5-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="613c5-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="613c5-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="613c5-145">Aktivace sdíleného počítače</span><span class="sxs-lookup"><span data-stu-id="613c5-145">Shared computer activation</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="613c5-148">Upgradujte práva na Windows 10 Pro z win 7/8.1 Pro licencí</span><span class="sxs-lookup"><span data-stu-id="613c5-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="613c5-150">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="613c5-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="613c5-151">Office 365 Ochrana před únikem dat</span><span class="sxs-lookup"><span data-stu-id="613c5-151">Office 365 Data Loss Prevention</span></span>|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="613c5-154">Azure Information Protection Plan 1, nástroj BitLocker vynucení</span><span class="sxs-lookup"><span data-stu-id="613c5-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="613c5-156">Plán ochrany informací v Azure 1, popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="613c5-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="613c5-158">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="613c5-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="613c5-159">Enterprise Cal Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="613c5-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Součástí Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="613c5-161"><sup>1</sup> Microsoft 365 Business Premium aplikace Office nezahrnuje aktivaci multilicence prostřednictvím Zásady skupiny, telemetrie aplikací, ovládacích prvků aktualizace, porovnání tabulek a dotazování nebo business Intelligence.</span><span class="sxs-lookup"><span data-stu-id="613c5-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="613c5-162">Migrace</span><span class="sxs-lookup"><span data-stu-id="613c5-162">Migration</span></span>

<span data-ttu-id="613c5-163">Pokyny k migraci [](../commerce/subscriptions/change-plans-manually.md) předplatného najdete v tématu Ruční změna plánů, pokud chcete přesunout jenom několik lidí do Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="613c5-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="613c5-164">Můžete taky [upgradovat všechny automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo můžete spolupracovat s partnerem a přesunout předplatné E3 a licence na Microsoft 365 Business Premium předplatné.</span><span class="sxs-lookup"><span data-stu-id="613c5-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="613c5-165">Následující části popisují případné změny, které je potřeba udělat, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="613c5-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="613c5-166">Office 365 Konfigurace a data předplatného E3</span><span class="sxs-lookup"><span data-stu-id="613c5-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="613c5-167">Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, mezi které patří:</span><span class="sxs-lookup"><span data-stu-id="613c5-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="613c5-168">Konfigurace předplatného, jako jsou záznamy DNS a názvy domén.</span><span class="sxs-lookup"><span data-stu-id="613c5-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="613c5-169">Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="613c5-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="613c5-170">Konfigurace služeb produktivity a jejich data, jako jsou Teams, Exchange Online poštovní schránky, weby SharePoint Online, OneDrive pro firmy složky a OneNote poznámkové bloky.</span><span class="sxs-lookup"><span data-stu-id="613c5-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="613c5-171">Office aplikace se automaticky škálují.</span><span class="sxs-lookup"><span data-stu-id="613c5-171">Office applications will scale automatically.</span></span> <span data-ttu-id="613c5-172">Office 365 moderní licencování zkontroluje přiřazení licence uživatele každých 72 hodin a převede Office aplikace na verzi, která odpovídá uživatelskému předplatnému.</span><span class="sxs-lookup"><span data-stu-id="613c5-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="613c5-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="613c5-173">Windows 10</span></span>

<span data-ttu-id="613c5-174">Pokud vaše Windows ještě nejsou v aktualizaci Windows Pro creatorů, upgradujte je na [Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="613c5-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="613c5-175">Nastavení zásad pro ochranu uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="613c5-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="613c5-176">Pokud nastavíte zásady a Office 365 MDM, budou tato zařízení  uvedená na stránce Zařízení v centru Microsoft 365 správy.</span><span class="sxs-lookup"><span data-stu-id="613c5-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="613c5-177">Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="613c5-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="613c5-178">Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.</span><span class="sxs-lookup"><span data-stu-id="613c5-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="613c5-179">Pokud jste upgradovali všechny uživatele ve vaší organizaci na Microsoft 365 Business Premium, zobrazí se průvodce nastavením na domovské stránce a můžete postupovat podle pokynů průvodce nastavením nastavit [Microsoft 365 Business Premium](set-up.md) a chránit soubory a mobilní zařízení.</span><span class="sxs-lookup"><span data-stu-id="613c5-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="613c5-180">Tento postup můžete provést taky na stránce Zařízení:</span><span class="sxs-lookup"><span data-stu-id="613c5-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="613c5-181">V Centru pro správu v levém navigačním panelu přejděte na **Zásady** \> **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="613c5-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="613c5-182">Na stránce **Zásady zařízení** zvolte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="613c5-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="613c5-183">V podokně **Přidat zásadu** pojmete zásadu **a** v rozevíracím seznamu zvolte typ zásady.</span><span class="sxs-lookup"><span data-stu-id="613c5-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="613c5-184">Můžete nastavit zásady aplikace pro ochranu souborů na zařízeních s Androidem a iPhone a Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení vlastněná Windows 10 zařízeními.</span><span class="sxs-lookup"><span data-stu-id="613c5-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="613c5-185">Podrobnosti najdete v následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="613c5-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="613c5-186">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="613c5-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="613c5-187">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="613c5-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="613c5-188">Nastavení ochrany zařízení pro Windows 10 počítače</span><span class="sxs-lookup"><span data-stu-id="613c5-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="613c5-189">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="613c5-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="613c5-190">Postup [pro Windows najdete v Windows](set-up-windows-devices.md) Windows zařízení pro Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="613c5-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="613c5-191">Postup pro telefony s [Androidem a iPhony najdete v tématu](set-up-mobile-devices.md) Microsoft 365 Business Premium mobilních zařízení pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="613c5-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="613c5-192">Velikost poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="613c5-192">Mailbox Size</span></span>

<span data-ttu-id="613c5-193">Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Exchange Online Plán 1.</span><span class="sxs-lookup"><span data-stu-id="613c5-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="613c5-194">Při migraci na Microsoft 365 Business Premium, pokud některý z vašich uživatelů překročí 50 GB úložiště poštovních schránek, doporučujeme tomuto uživateli přiřadit plán Exchange Online Plán 2 a odebrat plán Exchange Online 1, protože není možné přiřadit obojí.</span><span class="sxs-lookup"><span data-stu-id="613c5-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="613c5-195">Ochrana před hrozbou</span><span class="sxs-lookup"><span data-stu-id="613c5-195">Threat protection</span></span>

<span data-ttu-id="613c5-196">Po migraci na Microsoft 365 Business Premium máte Defender pro Office 365.</span><span class="sxs-lookup"><span data-stu-id="613c5-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="613c5-197">Přehled [najdete v Office 365](../security/office-365-security/defender-for-office-365.md) Microsoft Defenderu.</span><span class="sxs-lookup"><span data-stu-id="613c5-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="613c5-198">Pokud chcete nastavit, [podívejte](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)se na nastavení bezpečných odkazů [,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nastavení bezpečných příloh a nastavení [anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)v Defenderu pro Office 365 .</span><span class="sxs-lookup"><span data-stu-id="613c5-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="613c5-199">Štítky utajení</span><span class="sxs-lookup"><span data-stu-id="613c5-199">Sensitivity labels</span></span>

<span data-ttu-id="613c5-200">Pokud chcete začít používat [](../compliance/sensitivity-labels.md) popisky citlivosti, podívejte se na téma Přehled popisků citlivosti a vytváření a správa popisků [citlivosti](../business-video/create-sensitivity-labels.md) videa.</span><span class="sxs-lookup"><span data-stu-id="613c5-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>
