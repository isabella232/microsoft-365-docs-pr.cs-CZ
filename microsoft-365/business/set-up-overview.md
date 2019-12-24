---
title: Přehled nastavení
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přehled kroků nastavení pro aplikaci Microsoft 365 Business.
ms.openlocfilehash: 4aca617015cceb85ca35c8d8ada7b83d1416d959
ms.sourcegitcommit: 178ecb21cacdeaf440f3df2fe6e539e9127fcf15
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/23/2019
ms.locfileid: "40850798"
---
# <a name="overview-of-setup"></a><span data-ttu-id="89618-103">Přehled nastavení</span><span class="sxs-lookup"><span data-stu-id="89618-103">Overview of setup</span></span>

<span data-ttu-id="89618-104">Sledujte krátké video o aplikaci Microsoft 365 Business Setup.</span><span class="sxs-lookup"><span data-stu-id="89618-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="89618-105">Pokud jste toto video našli, podívejte se na [kompletní tréninkové řady pro malé firmy a ty nové do společnosti Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="89618-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="89618-106">Většinu kroků nastavení lze provést v Průvodci nastavením, ale jsou zde také uvedeny další možnosti.</span><span class="sxs-lookup"><span data-stu-id="89618-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="89618-107">Krok 1: Přidání domény a uživatelů</span><span class="sxs-lookup"><span data-stu-id="89618-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="89618-108">**[Přidejte svou doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste během [přihlášení](sign-up.md)koupili doménu, je tento krok již vykonáno.)</span><span class="sxs-lookup"><span data-stu-id="89618-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="89618-109">**Přidejte uživatele**.</span><span class="sxs-lookup"><span data-stu-id="89618-109">**Add users**.</span></span> <span data-ttu-id="89618-110">Uživatele můžete přidat některým ze tří způsobů:</span><span class="sxs-lookup"><span data-stu-id="89618-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="89618-111">V [Průvodci](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="89618-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="89618-112">Chcete-li [Přidat uživatele pomocí funkce Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) (v prostorách služby Active Directory), použijte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="89618-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="89618-113">Uživatele můžete také [přidat později](add-users-m365b.md) v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="89618-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="89618-114">Krok 2: nastavení zásad zabezpečení a konfigurace zařízení</span><span class="sxs-lookup"><span data-stu-id="89618-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="89618-115">Pomocí [Průvodce instalací](set-up.md#protect-your-organization) nakonfigurujte zásady zařízení.</span><span class="sxs-lookup"><span data-stu-id="89618-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="89618-116">Můžete je také přidat nebo upravit později v [centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="89618-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="89618-117">Průvodce instalací také nastaví základní ochranu proti ohrožení a nastavení prevence ztráty dat.</span><span class="sxs-lookup"><span data-stu-id="89618-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="89618-118">Kromě nastavení zabezpečení v Průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:</span><span class="sxs-lookup"><span data-stu-id="89618-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="89618-119">**Ochrana proti malwaru e-mailu**</span><span class="sxs-lookup"><span data-stu-id="89618-119">**Email malware protection**</span></span>
- <span data-ttu-id="89618-120">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="89618-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="89618-121">**Exchange Online - archiv**</span><span class="sxs-lookup"><span data-stu-id="89618-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="89618-122">**Ochrana informací Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="89618-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="89618-123">Chcete-li začít, přečtěte si informace v tématu [Nastavení rozšířených zásad zabezpečení](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="89618-123">To get started, see [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="89618-124">Viz také [10 nejlepších způsobů zabezpečení společnosti Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro cestovní mapu s nejlepšími bezpečnostními postupy.</span><span class="sxs-lookup"><span data-stu-id="89618-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="89618-125">Krok 3: nastavení a Správa zařízení systému Windows 10</span><span class="sxs-lookup"><span data-stu-id="89618-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="89618-126">Po spuštění Průvodce nastavením budete chtít v organizaci proctit všechny počítače společnosti Windwos 10.</span><span class="sxs-lookup"><span data-stu-id="89618-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="89618-127">Systém Windows 10 pro je [nezbytným předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale pokud používáte systém Windows 7 pro, Windows 8 pro nebo Windows 8,1 pro, vaše předplatné vás opravňuje k [inovaci na systém Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="89618-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="89618-128">Chcete-li nastavit zásady pro zařízení systému Windows 10, postupujte podle kroků v [zabezpečených počítačích se systémem Windows 10](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="89618-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="89618-129">Připojíte-li zařízení se systémem Windows 10 k Azure AD, budou na něj použity zásady nastavené pro počítače se systémem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="89618-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="89618-130">Další informace naleznete v tématu [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="89618-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="89618-131">Krok 4: instalace sady Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="89618-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="89618-132">Sadu Office lze automaticky nainstalovat do zařízení systému Windows pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="89618-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="89618-133">Umožňuje uživatelům [instalovat aplikace sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.</span><span class="sxs-lookup"><span data-stu-id="89618-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="89618-134">Pokročilé</span><span class="sxs-lookup"><span data-stu-id="89618-134">Advanced</span></span>
- <span data-ttu-id="89618-135">**Použití automatického Opilotu k nastavení nových zařízení**</span><span class="sxs-lookup"><span data-stu-id="89618-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="89618-136">Pomocí [systému Windows autopilot](add-autopilot-devices-and-profile.md) můžete automaticky nakonfigurovat **Nová** zařízení systému Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který by to mohl udělat za vás.</span><span class="sxs-lookup"><span data-stu-id="89618-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="89618-137">Můžete také přejít do [aplikace Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na technologii cloud, aby nastavil nová zařízení, která zakoupíte.</span><span class="sxs-lookup"><span data-stu-id="89618-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="89618-138">**Přístup k prostředkům na místě**</span><span class="sxs-lookup"><span data-stu-id="89618-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="89618-139">Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="89618-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="89618-140">Postupujte podle kroků, [které umožňují, aby zařízení systému Windows 10 spojená s doménou byla spravována společností Microsoft 365 Business](manage-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="89618-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="89618-141">Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají zařízení spojená s hybridním Azure.</span><span class="sxs-lookup"><span data-stu-id="89618-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="89618-142">Pokud vaše společnost disponuje místním adresářem služby Active Directory obsahujícím některé místní zdroje (například sdílené soubory a tiskárny), můžete k těmto zdrojům poskytnout přístup k těmto prostředkům pomocí zařízení Azure AD, a to následujícím postupem: [přístup k místním prostředkům z zařízení připojeném Azure AD v Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="89618-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="89618-143">Viz také</span><span class="sxs-lookup"><span data-stu-id="89618-143">See also</span></span>

[<span data-ttu-id="89618-144">Microsoft 365 Business Training video</span><span class="sxs-lookup"><span data-stu-id="89618-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
