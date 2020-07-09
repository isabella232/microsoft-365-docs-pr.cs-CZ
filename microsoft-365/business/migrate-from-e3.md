---
title: Migrace na Microsoft 365 Business z Office 365 E3
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
description: Přečtěte si, jak přesunout firmu na Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081798"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="ebafd-103">Přechod z Office 365 E3 na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ebafd-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="ebafd-104">Microsoft 365 Business Premium má vše, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace na úrovni produktivity ve své třídě s jednoduchou správou a zabezpečením zařízení.</span><span class="sxs-lookup"><span data-stu-id="ebafd-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="ebafd-105">Pokud máte v současné době předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="ebafd-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="ebafd-106">Migrace je snadná: Nejprve přepnete licence a všechny vaše data a informace o uživateli v aktuálním předplatném budou zachovány.</span><span class="sxs-lookup"><span data-stu-id="ebafd-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="ebafd-107">Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ebafd-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="ebafd-108">Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ebafd-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="ebafd-109">Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="ebafd-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="ebafd-110">Funkce</span><span class="sxs-lookup"><span data-stu-id="ebafd-110">Feature</span></span>    | <span data-ttu-id="ebafd-111">Podpora v Microsoftu 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ebafd-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="ebafd-112">Podpora v Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="ebafd-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="ebafd-113">**Místní**</span><span class="sxs-lookup"><span data-stu-id="ebafd-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="ebafd-114">Aplikace Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="ebafd-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="ebafd-115">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="ebafd-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="ebafd-116">Aplikace Microsoft 365 pro podniky</span><span class="sxs-lookup"><span data-stu-id="ebafd-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="ebafd-117">**Cloudové aplikace pro zvýšení produktivity**</span><span class="sxs-lookup"><span data-stu-id="ebafd-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="ebafd-118">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="ebafd-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="ebafd-119">Limit úložiště 50 GB na poštovní schránku a neomezená archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ebafd-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="ebafd-120">Limit úložiště 100 GB na poštovní schránku a neomezený archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ebafd-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="ebafd-121">Týmy</span><span class="sxs-lookup"><span data-stu-id="ebafd-121">Teams</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="ebafd-124">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="ebafd-124">OneDrive for Business</span></span>    | <span data-ttu-id="ebafd-125">Limit úložiště 1 TB na uživatele</span><span class="sxs-lookup"><span data-stu-id="ebafd-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="ebafd-126">Neomezené</span><span class="sxs-lookup"><span data-stu-id="ebafd-126">Unlimited</span></span> | 
| <span data-ttu-id="ebafd-127">Yammer, SharePoint Online, Plánovač, Stream</span><span class="sxs-lookup"><span data-stu-id="ebafd-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="ebafd-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="ebafd-130">StaffHub</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="ebafd-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="ebafd-133">Outlook Customer Manager, MileIQ</span></span>    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="ebafd-135">**Ochrana před hrozbami**</span><span class="sxs-lookup"><span data-stu-id="ebafd-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="ebafd-136">Plán 1 pokročilé ochrany před hrozbami Office 365</span><span class="sxs-lookup"><span data-stu-id="ebafd-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="ebafd-138">Není zahrnuto, ale může být přidáno na</span><span class="sxs-lookup"><span data-stu-id="ebafd-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="ebafd-139">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="ebafd-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="ebafd-140">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure (MFA), podmíněný přístup, zpětný zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="ebafd-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="ebafd-142">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="ebafd-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="ebafd-143">Microsoft Intune, Automaticképilot systému Windows</span><span class="sxs-lookup"><span data-stu-id="ebafd-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="ebafd-145">Aktivace sdíleného počítače</span><span class="sxs-lookup"><span data-stu-id="ebafd-145">Shared computer activation</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="ebafd-148">Práva na upgrade na Windows 10 Pro z licencí Win 7/8.1 Pro</span><span class="sxs-lookup"><span data-stu-id="ebafd-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="ebafd-150">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="ebafd-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="ebafd-151">Ochrana před ztrátou dat v Office 365</span><span class="sxs-lookup"><span data-stu-id="ebafd-151">Office 365 Data Loss Prevention</span></span>|    ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="ebafd-154">Azure Information Protection Plan 1, Vynucení nástroje Bitlocker</span><span class="sxs-lookup"><span data-stu-id="ebafd-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="ebafd-156">Azure Information Protection Plan 1, popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="ebafd-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="ebafd-158">**Licence klientského přístupu (práva CAL)**</span><span class="sxs-lookup"><span data-stu-id="ebafd-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="ebafd-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="ebafd-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Součástí Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="ebafd-161"><sup>1</sup> Verze aplikací Office pro Microsoft 365 Business Premium nezahrnuje aktivaci svazku prostřednictvím zásad skupiny, telemetrie aplikací, ovládacích prvků aktualizací, porovnání tabulek a dotazování nebo business intelligence.</span><span class="sxs-lookup"><span data-stu-id="ebafd-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="ebafd-162">Migrace</span><span class="sxs-lookup"><span data-stu-id="ebafd-162">Migration</span></span>

<span data-ttu-id="ebafd-163">Pokud chcete migrovat předplatné, přečtěte si pokyny v [tématu Ruční změna plánů,](../commerce/subscriptions/change-plans-manually.md) pokud chcete do Microsoft 365 Business Premium přesunout jemnou lidi.</span><span class="sxs-lookup"><span data-stu-id="ebafd-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="ebafd-164">Můžete také [upgradovat všechny uživatele automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo spolupracovat s partnerem a přesunout předplatné e3 a licence na předplatné Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ebafd-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="ebafd-165">Následující části popisují změny, které je třeba provést, pokud existuje, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="ebafd-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="ebafd-166">Konfigurace předplatného Office 365 E3 a data</span><span class="sxs-lookup"><span data-stu-id="ebafd-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="ebafd-167">Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, což zahrnuje:</span><span class="sxs-lookup"><span data-stu-id="ebafd-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="ebafd-168">Konfigurace předplatného, například záznamy DNS a názvy domén.</span><span class="sxs-lookup"><span data-stu-id="ebafd-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="ebafd-169">Uživatelské a skupinové účty a nastavení ověřování, jako je například vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="ebafd-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="ebafd-170">Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="ebafd-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="ebafd-171">Aplikace Office se automaticky škáluje.</span><span class="sxs-lookup"><span data-stu-id="ebafd-171">Office applications will scale automatically.</span></span> <span data-ttu-id="ebafd-172">Moderní licencování Office 365 bude každých 72 hodin kontrolovat přiřazení licencí uživatele a převádí aplikace Office na verzi, která odpovídá uživatelskému předplatnému.</span><span class="sxs-lookup"><span data-stu-id="ebafd-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="ebafd-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="ebafd-173">Windows 10</span></span>

<span data-ttu-id="ebafd-174">Pokud váš Windows ještě není v aktualizaci Windows Pro Creator, upgradujte je na [aktualizaci Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="ebafd-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="ebafd-175">Nastavení zásad ochrany uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="ebafd-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="ebafd-176">Pokud nastavíte zásady a zařízení Office 365 MDM, budou tato zařízení uvedena na stránce **Zařízení** v Centru pro správu Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="ebafd-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="ebafd-177">Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="ebafd-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="ebafd-178">Po přiřazení licencí k aplikaci Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.</span><span class="sxs-lookup"><span data-stu-id="ebafd-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="ebafd-179">Pokud jste všechny uživatele ve vaší organizaci upgradovali na Microsoft 365 Business Premium, zobrazí se na domovské stránce Průvodce instalací a můžete postupovat podle [nastavení Microsoft 365 Business Premium v krocích průvodce nastavením](set-up.md) za účelem ochrany souborů a mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="ebafd-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="ebafd-180">Můžete také provést tyto kroky na stránce Zařízení:</span><span class="sxs-lookup"><span data-stu-id="ebafd-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="ebafd-181">V Centru pro správu v levém **Devices** navigačním panelu přejděte na \> **položku Zásady zařízení**.</span><span class="sxs-lookup"><span data-stu-id="ebafd-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="ebafd-182">Na stránce **Zásady zařízení** zvolte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="ebafd-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="ebafd-183">V podokně **Přidat zásady** pojmenujte zásadu a zvolte **typ zásady** z rozevíracího panelu.</span><span class="sxs-lookup"><span data-stu-id="ebafd-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="ebafd-184">Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních s Androidem a iPhonem a také na Windows 10 a nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností.</span><span class="sxs-lookup"><span data-stu-id="ebafd-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="ebafd-185">Podrobnosti naleznete v následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="ebafd-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="ebafd-186">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="ebafd-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="ebafd-187">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="ebafd-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="ebafd-188">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="ebafd-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="ebafd-189">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="ebafd-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="ebafd-190">Postup pro zařízení s Windows najdete v tématu [Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="ebafd-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="ebafd-191">Postup pro telefony a iPhony s Androidem najdete v článku [Nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="ebafd-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="ebafd-192">Ochrana před hrozbami</span><span class="sxs-lookup"><span data-stu-id="ebafd-192">Threat protection</span></span>

<span data-ttu-id="ebafd-193">Po migraci na Microsoft 365 Business Premium máte office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="ebafd-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="ebafd-194">Přehled najdete v [článku Office 365 ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="ebafd-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="ebafd-195">Nastavení naleznete v [tématu nastavení bezpečných odkazů ATP](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [nastavení bezpečných příloh ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)a [nastavení ochrany proti phishingu .](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="ebafd-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="ebafd-196">Štítky utajení</span><span class="sxs-lookup"><span data-stu-id="ebafd-196">Sensitivity labels</span></span>

<span data-ttu-id="ebafd-197">Chcete-li začít používat popisky citlivosti, přečtěte si téma [Přehled popisků citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) a vytvoření a správa videa [s popisky citlivosti.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="ebafd-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
