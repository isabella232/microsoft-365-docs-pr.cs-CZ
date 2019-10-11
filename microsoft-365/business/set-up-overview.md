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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přehled kroků nastavených pro aplikaci Microsoft 365 Business.
ms.openlocfilehash: 4be0a8aa1b050ee3e20a045eb2c07666765118ed
ms.sourcegitcommit: cbf117a4cd92a907115c9f10752f3c557361e586
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/10/2019
ms.locfileid: "37440531"
---
# <a name="overview-of-setup"></a><span data-ttu-id="18b4c-103">Přehled nastavení</span><span class="sxs-lookup"><span data-stu-id="18b4c-103">Overview of setup</span></span>

<span data-ttu-id="18b4c-104">Většinu kroků nastavení lze provést v Průvodci nastavením, ale jsou zde také uvedeny další možnosti.</span><span class="sxs-lookup"><span data-stu-id="18b4c-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="18b4c-105">Krok 1: Přidání domény a uživatelů</span><span class="sxs-lookup"><span data-stu-id="18b4c-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="18b4c-106">**[Přidejte svou doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste během [přihlášení](sign-up.md)koupili doménu, je tento krok již vykonáno.)</span><span class="sxs-lookup"><span data-stu-id="18b4c-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="18b4c-107">**Přidejte uživatele**.</span><span class="sxs-lookup"><span data-stu-id="18b4c-107">**Add users**.</span></span> <span data-ttu-id="18b4c-108">To lze provést některým ze tří způsobů:</span><span class="sxs-lookup"><span data-stu-id="18b4c-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="18b4c-109">V [Průvodci](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="18b4c-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="18b4c-110">Chcete-li [Přidat uživatele pomocí funkce Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) (v prostorách služby Active Directory), použijte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="18b4c-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="18b4c-111">Uživatele můžete také [přidat později](add-users-m365b.md) v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="18b4c-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="18b4c-112">Krok 2: nastavení zásad zabezpečení a konfigurace zařízení</span><span class="sxs-lookup"><span data-stu-id="18b4c-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="18b4c-113">Pomocí [Průvodce instalací](set-up.md#protect-data-and-devices) nakonfigurujte zásady zařízení a zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="18b4c-113">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies.</span></span> 
  - <span data-ttu-id="18b4c-114">Můžete je také přidat nebo upravit později v [centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="18b4c-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="18b4c-115">Kromě nastavení zabezpečení v Průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:</span><span class="sxs-lookup"><span data-stu-id="18b4c-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="18b4c-116">**Ochrana proti malwaru e-mailu**</span><span class="sxs-lookup"><span data-stu-id="18b4c-116">**Email malware protection**</span></span>
      - <span data-ttu-id="18b4c-117">**Rozšířené možnosti ochrany proti ohrožení (ATP) bezpečné odkazy**</span><span class="sxs-lookup"><span data-stu-id="18b4c-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="18b4c-118">**Bezpečné přílohy ATP**</span><span class="sxs-lookup"><span data-stu-id="18b4c-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="18b4c-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="18b4c-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="18b4c-120">**Exchange Online - archiv**</span><span class="sxs-lookup"><span data-stu-id="18b4c-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="18b4c-121">**Zabránění ztrátě dat (DLP)**</span><span class="sxs-lookup"><span data-stu-id="18b4c-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="18b4c-122">**Ochrana informací Azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="18b4c-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="18b4c-123">Chcete-li se začít podívat, [nastavte pokročilé zásady zabezpečení](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="18b4c-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="18b4c-124">Viz také [10 nejlepších způsobů zabezpečení společnosti Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro cestovní mapu s nejlepšími bezpečnostními postupy.</span><span class="sxs-lookup"><span data-stu-id="18b4c-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="18b4c-125">Krok 3: nastavení a Správa zařízení systému Windows 10</span><span class="sxs-lookup"><span data-stu-id="18b4c-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="18b4c-126">Připojíte-li zařízení se systémem Windows 10 k Azure AD, zásady nastavené v [kroku 2](#step-2-set-up-security-policies-and-configure-devices) se na něj uplatní.</span><span class="sxs-lookup"><span data-stu-id="18b4c-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="18b4c-127">Systém Windows 10 pro je [předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale pokud máte Windows 7 pro, Windows 8 pro nebo Windows 8,1 pro, vaše předplatné vás opravňuje k [inovaci na systém Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="18b4c-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="18b4c-128">Pomocí [Průvodce instalací](set-up.md#protect-data-and-devices) nakonfigurujte zásady pro zařízení systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="18b4c-128">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="18b4c-129">Stes 4: instalace sady Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="18b4c-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="18b4c-130">Sadu Office lze automaticky nainstalovat do zařízení systému Windows pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="18b4c-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="18b4c-131">Automaticky [nainstalujte sadu Office](auto-install-or-uninstall-office.md) z centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="18b4c-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="18b4c-132">Umožňuje uživatelům [instalovat aplikace sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.</span><span class="sxs-lookup"><span data-stu-id="18b4c-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="18b4c-133">Pokročilé</span><span class="sxs-lookup"><span data-stu-id="18b4c-133">Advanced</span></span>
- <span data-ttu-id="18b4c-134">**Použití automatického Opilotu k nastavení nových zařízení**</span><span class="sxs-lookup"><span data-stu-id="18b4c-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="18b4c-135">Pomocí [systému Windows autopilot](add-autopilot-devices-and-profile.md) můžete automaticky nakonfigurovat **Nová** zařízení systému Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který by to mohl udělat za vás.</span><span class="sxs-lookup"><span data-stu-id="18b4c-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="18b4c-136">Můžete také přejít do [aplikace Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) a požádat odborníka na technologii cloud, aby nastavil nová zařízení, která vám zakoupíte.</span><span class="sxs-lookup"><span data-stu-id="18b4c-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="18b4c-137">**Přístup k prostředkům na místě**</span><span class="sxs-lookup"><span data-stu-id="18b4c-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="18b4c-138">Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="18b4c-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="18b4c-139">Postupujte podle kroků, [které umožňují, aby zařízení systému Windows 10 spojená s doménou byla spravována společností Microsoft 365 Business](manage-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="18b4c-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="18b4c-140">Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají zařízení spojená s hybridním Azure.</span><span class="sxs-lookup"><span data-stu-id="18b4c-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="18b4c-141">Pokud váš podnik disponuje místním adresářem služby Active Directory obsahujícím některé místní zdroje (například sdílené soubory a tiskárny), můžete k těmto zdrojům poskytnout přístup k těmto prostředkům pomocí zařízení Azure AD, a to následujícím postupem: [přístup k místním prostředkům z Zařízení připojené k Azure v aplikaci Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="18b4c-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  