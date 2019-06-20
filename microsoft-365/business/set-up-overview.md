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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přehled nastavení kroky pro Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086284"
---
# <a name="overview-of-setup"></a><span data-ttu-id="8a28f-103">Přehled nastavení</span><span class="sxs-lookup"><span data-stu-id="8a28f-103">Overview of setup</span></span>

<span data-ttu-id="8a28f-104">Většina nastavení kroky lze provést v Průvodci instalací, ale jsou také uvedeny další možnosti.</span><span class="sxs-lookup"><span data-stu-id="8a28f-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="8a28f-105">Krok 1: Přidání domény a uživatelé</span><span class="sxs-lookup"><span data-stu-id="8a28f-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="8a28f-106">**[Přidat do domény](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste si koupili své domény při [přihlášení](sign-up.md), tento krok je již proveden.)</span><span class="sxs-lookup"><span data-stu-id="8a28f-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="8a28f-107">**Přidání uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="8a28f-107">**Add users**.</span></span> <span data-ttu-id="8a28f-108">Lze provést třemi způsoby:</span><span class="sxs-lookup"><span data-stu-id="8a28f-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="8a28f-109">Podle pokynů [Průvodce](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="8a28f-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="8a28f-110">Používá pro synchronizaci adresářů přidat [uživatele Azure AD připojit pomocí](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) služby Active directory v prostorách.</span><span class="sxs-lookup"><span data-stu-id="8a28f-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="8a28f-111">Můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="8a28f-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="8a28f-112">Krok 2: Nastavit zásady zabezpečení a konfigurace zařízení</span><span class="sxs-lookup"><span data-stu-id="8a28f-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="8a28f-113">[Průvodce instalací](set-up.md#set-up-security-policies-and-device-configurations) slouží ke konfiguraci zásad zabezpečení a zařízení.</span><span class="sxs-lookup"><span data-stu-id="8a28f-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="8a28f-114">Můžete také přidat více nebo je upravit později v [admin center](view-policies-and-devices.md) a do [Intune portál](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="8a28f-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="8a28f-115">Kromě nastavení zabezpečení v Průvodci instalací můžete zvýšit přidáním následující nastavení zabezpečení:</span><span class="sxs-lookup"><span data-stu-id="8a28f-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="8a28f-116">**E-mailová ochrana proti malwaru**</span><span class="sxs-lookup"><span data-stu-id="8a28f-116">**Email malware protection**</span></span>
      - <span data-ttu-id="8a28f-117">**Advanced Threat Protection (ATP) bezpečné propojení**</span><span class="sxs-lookup"><span data-stu-id="8a28f-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="8a28f-118">**ATP bezpečné přílohy**</span><span class="sxs-lookup"><span data-stu-id="8a28f-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="8a28f-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="8a28f-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="8a28f-120">**Exchange Online - archiv**</span><span class="sxs-lookup"><span data-stu-id="8a28f-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="8a28f-121">**Zabránění ztrátě dat (DLP)**</span><span class="sxs-lookup"><span data-stu-id="8a28f-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="8a28f-122">**Ochrana informací azure (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="8a28f-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="8a28f-123">Chcete-li získat spuštění naleznete v tématu [nastavení zásad pokročilé zabezpečení](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="8a28f-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="8a28f-124">Další informace naleznete v tématu [horní 10 způsobů, jak zabezpečit váš podnik 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro přehled osvědčených postupů zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="8a28f-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="8a28f-125">Krok 3: Nastavení a správa zařízení v systému Windows 10</span><span class="sxs-lookup"><span data-stu-id="8a28f-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="8a28f-126">Při připojení zařízení Windows 10 k Azure AD získat k němu použity zásady, které jste vytvořili v [kroku 2](#step-2-set-up-security-policies-and-configure-devices) .</span><span class="sxs-lookup"><span data-stu-id="8a28f-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="8a28f-127">Windows 10 Pro je [nutným předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro předplatné vás opravňuje k [upgradu na Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="8a28f-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="8a28f-128">[Průvodce instalací](set-up.md#set-up-security-policies-and-device-configurations) slouží ke konfiguraci zásad pro zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8a28f-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="8a28f-129">Stes 4: Instalace Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="8a28f-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="8a28f-130">Office v zařízení Windows může automaticky instalovat pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="8a28f-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="8a28f-131">Automaticky [nainstalovat systém Office](auto-install-or-uninstall-office.md) z středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="8a28f-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="8a28f-132">Umožní uživatelům [instalaci aplikací sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.</span><span class="sxs-lookup"><span data-stu-id="8a28f-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="8a28f-133">Upřesnit</span><span class="sxs-lookup"><span data-stu-id="8a28f-133">Advanced</span></span>
- <span data-ttu-id="8a28f-134">**Chcete-li nastavit nové zařízení pomocí Autopilot**</span><span class="sxs-lookup"><span data-stu-id="8a28f-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="8a28f-135">[Autopilot systému Windows](add-autopilot-devices-and-profile.md) lze nakonfigurovat automaticky **Nová** zařízení Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který lze provést za vás.</span><span class="sxs-lookup"><span data-stu-id="8a28f-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="8a28f-136">Můžete také přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) a zeptejte se odborníků cloud technologie nastavit nová zařízení, které zakoupíte, vám.</span><span class="sxs-lookup"><span data-stu-id="8a28f-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="8a28f-137">**Přístup k místním prostředkům**</span><span class="sxs-lookup"><span data-stu-id="8a28f-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="8a28f-138">Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních.</span><span class="sxs-lookup"><span data-stu-id="8a28f-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="8a28f-139">Postupujte podle kroků v [doméně zařízení Windows 10, které jsou spravovány Microsoft 365 Business povolit](manage-windows-devices.md) toto nastavení.</span><span class="sxs-lookup"><span data-stu-id="8a28f-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="8a28f-140">Toto je upřednostňovaný způsob a zařízení v tomto stavu se nazývají hybridní Azure AD připojené zařízení.</span><span class="sxs-lookup"><span data-stu-id="8a28f-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="8a28f-141">Pokud váš podnik má místní služby Active Directory, která obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete přidělit přístup Azure AD připojené zařízení tyto prostředky podle pokynů zde: [přístup místního zdroje z Azure AD připojené zařízení Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="8a28f-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  