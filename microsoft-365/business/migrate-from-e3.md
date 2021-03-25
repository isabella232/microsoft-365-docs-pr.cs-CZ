---
title: Migrace z Office 365 E3 na Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Zjistěte, jak přesunout firmu na Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: 3f9fd70b2d31b32027981e638de249d92e98ea08
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164527"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="c541d-103">Migrace z Office 365 E3 na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c541d-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c541d-104">Microsoft 365 Business Premium nabízí všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace založené na produktivitě s jednoduchou snadná správa a zabezpečení zařízení.</span><span class="sxs-lookup"><span data-stu-id="c541d-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="c541d-105">Pokud máte momentálně předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium, abyste získali další funkce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c541d-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="c541d-106">Migrace je snadná: Nejdřív přepnete licence a všechna data a informace o uživatelích v aktuálním předplatném se zachová.</span><span class="sxs-lookup"><span data-stu-id="c541d-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="c541d-107">Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c541d-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="c541d-108">Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c541d-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c541d-109">V této tabulce jsou uvedené rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="c541d-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="c541d-110">Funkce</span><span class="sxs-lookup"><span data-stu-id="c541d-110">Feature</span></span>    | <span data-ttu-id="c541d-111">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c541d-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="c541d-112">Podpora v Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="c541d-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="c541d-113">**Místní**</span><span class="sxs-lookup"><span data-stu-id="c541d-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="c541d-114">Aplikace Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="c541d-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="c541d-115">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="c541d-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="c541d-116">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="c541d-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="c541d-117">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="c541d-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="c541d-118">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="c541d-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="c541d-119">Limit úložiště 50 GB na poštovní schránku a neomezenou archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c541d-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="c541d-120">Limit úložiště 100 GB na poštovní schránku a neomezenou archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c541d-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="c541d-121">Teams</span><span class="sxs-lookup"><span data-stu-id="c541d-121">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="c541d-124">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="c541d-124">OneDrive for Business</span></span>    | <span data-ttu-id="c541d-125">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="c541d-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="c541d-126">Neomezená</span><span class="sxs-lookup"><span data-stu-id="c541d-126">Unlimited</span></span> | 
| <span data-ttu-id="c541d-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="c541d-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="c541d-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="c541d-130">StaffHub</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="c541d-133">Outlook Customer Manager</span><span class="sxs-lookup"><span data-stu-id="c541d-133">Outlook Customer Manager</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="c541d-135">**Ochrana před hrozbou**</span><span class="sxs-lookup"><span data-stu-id="c541d-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="c541d-136">Defender pro Office 365 – plán 1</span><span class="sxs-lookup"><span data-stu-id="c541d-136">Defender for Office 365 Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="c541d-138">Není zahrnuto, ale může být přidáno dne</span><span class="sxs-lookup"><span data-stu-id="c541d-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="c541d-139">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="c541d-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="c541d-140">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesla pro místní identity</span><span class="sxs-lookup"><span data-stu-id="c541d-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="c541d-142">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="c541d-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="c541d-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c541d-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="c541d-145">Aktivace sdíleného počítače</span><span class="sxs-lookup"><span data-stu-id="c541d-145">Shared computer activation</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="c541d-148">Upgrade práv na Windows 10 Pro z licencí Win 7/8.1 Pro</span><span class="sxs-lookup"><span data-stu-id="c541d-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="c541d-150">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="c541d-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="c541d-151">Prevence ztráty dat v Office 365</span><span class="sxs-lookup"><span data-stu-id="c541d-151">Office 365 Data Loss Prevention</span></span>|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="c541d-154">Azure Information Protection Plan 1, vynucení nástroje Bitlocker</span><span class="sxs-lookup"><span data-stu-id="c541d-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="c541d-156">Plán ochrany informací v Azure 1, popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="c541d-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="c541d-158">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="c541d-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="c541d-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="c541d-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Součástí Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="c541d-161"><sup>1</sup> Verze aplikací Office pro Microsoft 365 Business Premium nezahrnuje aktivaci multilicence přes Zásady skupiny, telemetrii aplikací, ovládací prvky aktualizací, porovnání tabulek a dotazy nebo business Intelligence.</span><span class="sxs-lookup"><span data-stu-id="c541d-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="c541d-162">Migrace</span><span class="sxs-lookup"><span data-stu-id="c541d-162">Migration</span></span>

<span data-ttu-id="c541d-163">Pokud chcete do [](../commerce/subscriptions/change-plans-manually.md) Microsoftu 365 Business Premium přesunout jenom pár lidí, přečtěte si pokyny k migraci předplatného ručně.</span><span class="sxs-lookup"><span data-stu-id="c541d-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="c541d-164">Můžete také [upgradovat všechny automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo můžete spolupracovat s partnerem a přesunout předplatné E3 a licence na předplatné Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c541d-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="c541d-165">Následující části popisují případné změny, které je potřeba udělat, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="c541d-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="c541d-166">Konfigurace a data předplatného Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="c541d-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="c541d-167">Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, mezi které patří:</span><span class="sxs-lookup"><span data-stu-id="c541d-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="c541d-168">Konfigurace předplatného, jako jsou záznamy DNS a názvy domén.</span><span class="sxs-lookup"><span data-stu-id="c541d-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="c541d-169">Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="c541d-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="c541d-170">Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="c541d-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="c541d-171">Aplikace Office se automaticky zmenšují.</span><span class="sxs-lookup"><span data-stu-id="c541d-171">Office applications will scale automatically.</span></span> <span data-ttu-id="c541d-172">Moderní licencování Office 365 zkontroluje přiřazení licencí uživatele každých 72 hodin a převede aplikace Office na verzi, která odpovídá předplatnému uživatele.</span><span class="sxs-lookup"><span data-stu-id="c541d-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="c541d-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="c541d-173">Windows 10</span></span>

<span data-ttu-id="c541d-174">Pokud váš systém Windows ještě není v aktualizaci Windows Pro Creator, [upgradujte je na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="c541d-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="c541d-175">Nastavení zásad pro ochranu uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="c541d-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="c541d-176">Pokud nastavíte zásady a zařízení Office 365 MDM,  budou tato zařízení uvedená na stránce Zařízení v Centru pro správu Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="c541d-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="c541d-177">Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="c541d-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="c541d-178">Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.</span><span class="sxs-lookup"><span data-stu-id="c541d-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="c541d-179">Pokud jste upgradovali všechny uživatele ve vaší organizaci na Microsoft 365 Business Premium, zobrazí se průvodce nastavením na domovské stránce a můžete postupovat podle pokynů Průvodce nastavením nastavit [Microsoft 365 Business Premium](set-up.md) k ochraně souborů a mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="c541d-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="c541d-180">Tento postup můžete provést taky na stránce Zařízení:</span><span class="sxs-lookup"><span data-stu-id="c541d-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="c541d-181">V Centru pro správu v levém navigačním panelu přejděte na **Zásady** \> **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c541d-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="c541d-182">Na stránce **Zásady zařízení** zvolte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="c541d-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="c541d-183">V podokně **Přidat zásadu** pojmete zásadu **a** v rozevíracím seznamu zvolte typ zásady.</span><span class="sxs-lookup"><span data-stu-id="c541d-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="c541d-184">Můžete nastavit zásady aplikace pro ochranu souborů na zařízeních s Androidem a iPhonem i ve Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností.</span><span class="sxs-lookup"><span data-stu-id="c541d-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="c541d-185">Podrobnosti najdete v následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="c541d-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="c541d-186">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="c541d-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="c541d-187">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="c541d-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="c541d-188">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="c541d-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="c541d-189">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="c541d-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="c541d-190">Postup pro zařízení s Windows najdete v tématu Nastavení zařízení s Windows pro uživatele [Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c541d-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="c541d-191">Postup pro telefony s Androidem a iPhony najdete v tématu Nastavení mobilních zařízení pro uživatele [Microsoftu 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="c541d-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="c541d-192">Velikost poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="c541d-192">Mailbox Size</span></span>

<span data-ttu-id="c541d-193">Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Plán 1 Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c541d-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="c541d-194">Pokud některý z vašich uživatelů při migraci na Microsoft 365 Business Premium překročí 50 GB úložiště poštovních schránek, doporučujeme tomuto uživateli přiřadit plán 2 Exchange Online a odebrat plán 1 Exchange Online, protože není možné přiřadit obojí.</span><span class="sxs-lookup"><span data-stu-id="c541d-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="c541d-195">Ochrana před hrozbou</span><span class="sxs-lookup"><span data-stu-id="c541d-195">Threat protection</span></span>

<span data-ttu-id="c541d-196">Po migraci na Microsoft 365 Business Premium máte Defender pro Office 365.</span><span class="sxs-lookup"><span data-stu-id="c541d-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="c541d-197">Přehled [najdete v tématu Microsoft Defender pro Office 365.](../security/defender-365-security/defender-for-office-365.md)</span><span class="sxs-lookup"><span data-stu-id="c541d-197">See [Microsoft Defender for Office 365](../security/defender-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="c541d-198">Pokud chcete nastavit, podívejte se na nastavení bezpečných odkazů [,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [nastavení](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)bezpečných příloh a nastavení anti-phishing v [Defenderu pro Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="c541d-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="c541d-199">Štítky utajení</span><span class="sxs-lookup"><span data-stu-id="c541d-199">Sensitivity labels</span></span>

<span data-ttu-id="c541d-200">Pokud chcete začít používat [](../compliance/sensitivity-labels.md) popisky citlivosti, podívejte se na téma Přehled popisků citlivosti a vytváření a správa popisků [citlivosti](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videa.</span><span class="sxs-lookup"><span data-stu-id="c541d-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
