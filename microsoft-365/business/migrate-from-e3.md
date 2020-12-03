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
ms.openlocfilehash: eebf78c24ed4bfd1a4fc2d843f37aebbe3d35e31
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558246"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="4a590-103">Migrace z Office 365 E3 na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="4a590-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="4a590-104">Microsoft 365 Business Premium obsahuje vše potřebné pro vaši malou firmu a spojuje aplikace pro optimální práci založené na cloudu s jednoduchou správou a zabezpečením zařízení.</span><span class="sxs-lookup"><span data-stu-id="4a590-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="4a590-105">Pokud aktuálně máte předplatné Office 365 E3, ale nepoužíváte více než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="4a590-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="4a590-106">Snadná migrace: Nejdřív si přepínáte licence a všechny vaše data a uživatelské informace jsou zachovány.</span><span class="sxs-lookup"><span data-stu-id="4a590-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="4a590-107">Po migraci budete muset nastavit funkce, které se přidají v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4a590-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="4a590-108">Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="4a590-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="4a590-109">Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="4a590-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="4a590-110">Funkce</span><span class="sxs-lookup"><span data-stu-id="4a590-110">Feature</span></span>    | <span data-ttu-id="4a590-111">Podpora v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="4a590-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="4a590-112">Podpora v Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="4a590-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="4a590-113">**Místní**</span><span class="sxs-lookup"><span data-stu-id="4a590-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="4a590-114">Aplikace Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="4a590-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="4a590-115">Aplikace Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="4a590-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="4a590-116">Microsoft 365 Apps for enterprise</span><span class="sxs-lookup"><span data-stu-id="4a590-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="4a590-117">**Kancelářské aplikace**</span><span class="sxs-lookup"><span data-stu-id="4a590-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="4a590-118">Exchange Online a Outlook</span><span class="sxs-lookup"><span data-stu-id="4a590-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="4a590-119">50 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="4a590-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="4a590-120">100 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online</span><span class="sxs-lookup"><span data-stu-id="4a590-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="4a590-121">Teams</span><span class="sxs-lookup"><span data-stu-id="4a590-121">Teams</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="4a590-124">OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="4a590-124">OneDrive for Business</span></span>    | <span data-ttu-id="4a590-125">1 TB limit úložiště na uživatele</span><span class="sxs-lookup"><span data-stu-id="4a590-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="4a590-126">Neomezené</span><span class="sxs-lookup"><span data-stu-id="4a590-126">Unlimited</span></span> | 
| <span data-ttu-id="4a590-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="4a590-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="4a590-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="4a590-130">StaffHub</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="4a590-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="4a590-133">Outlook Customer Manager, MileIQ</span></span>    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="4a590-135">**Ochrana před hrozbami**</span><span class="sxs-lookup"><span data-stu-id="4a590-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="4a590-136">Defender pro Office 365 plán 1</span><span class="sxs-lookup"><span data-stu-id="4a590-136">Defender for Office 365 Plan 1</span></span> | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="4a590-138">Není zahrnuto, ale můžete ho přidat</span><span class="sxs-lookup"><span data-stu-id="4a590-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="4a590-139">**Správa identit**</span><span class="sxs-lookup"><span data-stu-id="4a590-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="4a590-140">Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), Azure AD Multi-Factor Authentication (MFA), podmíněný přístup, zápis hesel pro místní identity</span><span class="sxs-lookup"><span data-stu-id="4a590-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="4a590-142">**Správa zařízení a aplikací**</span><span class="sxs-lookup"><span data-stu-id="4a590-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="4a590-143">Microsoft Intune, Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="4a590-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="4a590-145">Aktivace sdíleného počítače</span><span class="sxs-lookup"><span data-stu-id="4a590-145">Shared computer activation</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="4a590-148">Upgrade práv na Windows 10 pro na licence Win 7/8.1 pro</span><span class="sxs-lookup"><span data-stu-id="4a590-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="4a590-150">**Ochrana informací**</span><span class="sxs-lookup"><span data-stu-id="4a590-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="4a590-151">Ochrana před únikem dat v Office 365</span><span class="sxs-lookup"><span data-stu-id="4a590-151">Office 365 Data Loss Prevention</span></span>|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="4a590-154">Plán služby Azure Information Protection 1, vynucení nástroje BitLocker</span><span class="sxs-lookup"><span data-stu-id="4a590-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="4a590-156">Plán služby Azure Information Protection 1, popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="4a590-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="4a590-158">**Licence klientského přístupu (licence CAL)**</span><span class="sxs-lookup"><span data-stu-id="4a590-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="4a590-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="4a590-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Součástí Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="4a590-161"><sup>1</sup> verze Microsoft 365 Business Premium aplikací Office nezahrnují aktivaci multilicence prostřednictvím zásad skupiny, telemetrie aplikací, ovládacích prvků aktualizace, porovnání tabulek a dotazů nebo Business Intelligence.</span><span class="sxs-lookup"><span data-stu-id="4a590-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="4a590-162">Migrace</span><span class="sxs-lookup"><span data-stu-id="4a590-162">Migration</span></span>

<span data-ttu-id="4a590-163">Pokud chcete migrovat předplatné, přečtěte si článek [Ruční změna plánů](../commerce/subscriptions/change-plans-manually.md) , jestli chcete přesunout jenom pár lidí na Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4a590-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="4a590-164">Můžete taky [automaticky upgradovat všechny uživatele](../commerce/subscriptions/upgrade-to-different-plan.md)nebo spolupracovat s partnerem, abyste mohli přesunout předplatné E3 a licence na předplatné Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4a590-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="4a590-165">V následujících částech jsou popsány změny, které je třeba udělat, pokud existují, a co můžete udělat po migraci.</span><span class="sxs-lookup"><span data-stu-id="4a590-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="4a590-166">Konfigurace a data předplatného Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="4a590-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="4a590-167">Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, což zahrnuje:</span><span class="sxs-lookup"><span data-stu-id="4a590-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="4a590-168">Konfigurace předplatného, například záznamy DNS a názvy domén</span><span class="sxs-lookup"><span data-stu-id="4a590-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="4a590-169">Účty uživatelů a skupin a nastavení ověřování, například vícefaktorové ověřování nebo zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="4a590-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="4a590-170">Konfigurace produktivity služeb a jejich data, například týmy, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.</span><span class="sxs-lookup"><span data-stu-id="4a590-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="4a590-171">Aplikace Office se přizpůsobí automaticky.</span><span class="sxs-lookup"><span data-stu-id="4a590-171">Office applications will scale automatically.</span></span> <span data-ttu-id="4a590-172">Office 365 moderní licencování zkontroluje přiřazení licencí uživatele každých 72 hodin a převede aplikace Office na verzi, která odpovídá předplatnému uživatele.</span><span class="sxs-lookup"><span data-stu-id="4a590-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="4a590-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="4a590-173">Windows 10</span></span>

<span data-ttu-id="4a590-174">Pokud vaše okna ještě nejsou ve Windows pro Creator Update, [Upgradujte si je na Windows pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="4a590-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="4a590-175">Nastavení zásad pro ochranu uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="4a590-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="4a590-176">Pokud nastavíte zásady a zařízení Office 365 MDM, budou tato zařízení uvedená na stránce **zařízení** v centru pro správu systému Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4a590-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="4a590-177">Všechny vámi nastavené zásady se zobrazí v seznamu klasických zásad na [portálu Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="4a590-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="4a590-178">Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.</span><span class="sxs-lookup"><span data-stu-id="4a590-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="4a590-179">Pokud jste všichni v organizaci upgradovali na Microsoft 365 Business Premium, uvidíte Průvodce nastavením na domovské stránce a může se řídit [nastavením Microsoft 365 Business Premium v Průvodci nastavením](set-up.md) , abyste chránili soubory a mobilní zařízení.</span><span class="sxs-lookup"><span data-stu-id="4a590-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="4a590-180">Tyto kroky můžete provést taky na stránce zařízení:</span><span class="sxs-lookup"><span data-stu-id="4a590-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="4a590-181">V centru pro správu přejděte v levém navigačním podokně na **Devices** \> **zásady** zařízení.</span><span class="sxs-lookup"><span data-stu-id="4a590-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="4a590-182">Na stránce **zásady zařízení** zvolte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="4a590-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="4a590-183">V podokně **Přidat zásady** udělte dané zásadě název a v rozevíracím seznamu vyberte **Typ zásady** .</span><span class="sxs-lookup"><span data-stu-id="4a590-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="4a590-184">Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních s Androidem a iPhone a Windows 10 a nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností.</span><span class="sxs-lookup"><span data-stu-id="4a590-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="4a590-185">Podrobnosti najdete v následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="4a590-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="4a590-186">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="4a590-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="4a590-187">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4a590-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="4a590-188">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4a590-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="4a590-189">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="4a590-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="4a590-190">Postupy pro zařízení s Windows najdete v tématu [nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="4a590-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="4a590-191">Postup [nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md) pro telefony s Androidem a iPhone.</span><span class="sxs-lookup"><span data-stu-id="4a590-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="4a590-192">Velikost poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="4a590-192">Mailbox Size</span></span>

<span data-ttu-id="4a590-193">Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Exchange Online (plán 1).</span><span class="sxs-lookup"><span data-stu-id="4a590-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="4a590-194">Pokud některý z uživatelů přesáhne 50 GB úložiště poštovních schránek, doporučuje se při přechodu na Microsoft 365 Business Premium přiřadit tomuto uživateli tento uživatel: Exchange Online (plán 2) a odebrat plán 1 služby Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4a590-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="4a590-195">Ochrana před hrozbami</span><span class="sxs-lookup"><span data-stu-id="4a590-195">Threat protection</span></span>

<span data-ttu-id="4a590-196">Po migraci na Microsoft 365 Business Premium máte k dispozici program Defender pro Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a590-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="4a590-197">Další informace najdete v článku [Microsoft Defender pro Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) .</span><span class="sxs-lookup"><span data-stu-id="4a590-197">See [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="4a590-198">Nastavení, viz [Nastavení bezpečných odkazů](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [Nastavení bezpečných příloh](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)a [nastavení ochrany proti podvodným zprávám v programu Defender pro Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="4a590-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="4a590-199">Štítky utajení</span><span class="sxs-lookup"><span data-stu-id="4a590-199">Sensitivity labels</span></span>

<span data-ttu-id="4a590-200">Pokud chcete začít používat popisky citlivosti, přečtěte si článek Přehled popisů [citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) a [vytváření a Správa popisků](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) pro video.</span><span class="sxs-lookup"><span data-stu-id="4a590-200">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
