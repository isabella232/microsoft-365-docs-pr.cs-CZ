---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Naučte se používat funkci Windows AutoPilot k nastavení nových zařízení systému Windows 10 pro váš podnik.
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323089"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="99430-103">Podrobné pokyny k přidání zařízení a profilů Autopilota</span><span class="sxs-lookup"><span data-stu-id="99430-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="99430-104">Pomocí systému Windows AutoPilot můžete nastavit **nové** systémy Windows 10 pro váš podnik, takže jsou připraveny k použití, když je dáte svým zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="99430-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="99430-105">Požadavky na zařízení</span><span class="sxs-lookup"><span data-stu-id="99430-105">Device requirements</span></span>

<span data-ttu-id="99430-106">Zařízení musí splňovat tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="99430-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="99430-107">Windows 10, verze 1703 nebo novější</span><span class="sxs-lookup"><span data-stu-id="99430-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="99430-108">Nová zařízení, která nebyla součástí systému Windows,</span><span class="sxs-lookup"><span data-stu-id="99430-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="99430-109">Vytvoření zařízení a profilů pomocí průvodce instalací</span><span class="sxs-lookup"><span data-stu-id="99430-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="99430-110">[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="99430-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="99430-111">Pokud jste ještě nevytvořili skupiny zařízení nebo profily, nejlepším způsobem, jak začít, je použití podrobných vodítek.</span><span class="sxs-lookup"><span data-stu-id="99430-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="99430-112">Můžete také [Přidat zařízení](create-and-edit-autopilot-devices.md) a [přiřadit jim profily](create-and-edit-autopilot-profiles.md) bez použití průvodce.</span><span class="sxs-lookup"><span data-stu-id="99430-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="99430-113">Přejděte do centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>adrese.</span><span class="sxs-lookup"><span data-stu-id="99430-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="99430-114">V levém navigačním podokně vyberte položku **zařízení** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="99430-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![V centru pro správu zvolte zařízení a pak položku AutoPilot.](media/AutoPilot.png)
  
2. <span data-ttu-id="99430-116">Na stránce **autopilot** klikněte na tlačítko nebo na položku **Start Guide**.</span><span class="sxs-lookup"><span data-stu-id="99430-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="99430-118">V **souboru upload. CSV se seznamem zařízení** přejděte do umístění, kde je připraven. CSV a potom **otevřete** \> **Další**.</span><span class="sxs-lookup"><span data-stu-id="99430-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="99430-119">Soubor musí obsahovat tři hlavičky:</span><span class="sxs-lookup"><span data-stu-id="99430-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="99430-120">Sloupec A: Sériové číslo zařízení</span><span class="sxs-lookup"><span data-stu-id="99430-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="99430-121">Sloupec B: ID produktu Windows</span><span class="sxs-lookup"><span data-stu-id="99430-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="99430-122">Sloupec C: Hodnota hash hardwaru</span><span class="sxs-lookup"><span data-stu-id="99430-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="99430-123">Tyto informace můžete získat od dodavatele hardwaru nebo můžete vytvořit soubor CSV pomocí [skriptu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) .</span><span class="sxs-lookup"><span data-stu-id="99430-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="99430-p103">Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**.</span><span class="sxs-lookup"><span data-stu-id="99430-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="99430-126">Na stránce **přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový.</span><span class="sxs-lookup"><span data-stu-id="99430-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="99430-127">Pokud ještě žádnou nemáte, budete vyzváni k jeho vytvoření.</span><span class="sxs-lookup"><span data-stu-id="99430-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="99430-128">Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="99430-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="99430-129">Výchozí funkce jsou vyžadovány a jsou nastaveny automaticky.</span><span class="sxs-lookup"><span data-stu-id="99430-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="99430-130">Výchozí funkce:</span><span class="sxs-lookup"><span data-stu-id="99430-130">The default features are:</span></span>
    
    - <span data-ttu-id="99430-131">Vynechejte Cortana, OneDrive a registraci OEM.</span><span class="sxs-lookup"><span data-stu-id="99430-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="99430-132">Vytvoření postupu přihlášení doplněného o značku společnosti.</span><span class="sxs-lookup"><span data-stu-id="99430-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="99430-133">Připojte zařízení k účtům služby Active Directory společnosti Azure a automaticky je zapište, aby byly spravovány společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="99430-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="99430-134">Další informace naleznete v tématu [o nastavení profilu AutoPilot](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="99430-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="99430-135">Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="99430-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="99430-136">Zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="99430-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="99430-137">**Vaše práce** znamená, že vytvořený profil (nebo zvolený) bude použit u skupiny zařízení, kterou jste vytvořili, uložením seznamu zařízení.</span><span class="sxs-lookup"><span data-stu-id="99430-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="99430-138">Nastavení bude platné po přihlášení uživatelů zařízení.</span><span class="sxs-lookup"><span data-stu-id="99430-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="99430-139">Zvolte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="99430-139">Choose **Close**.</span></span>
    