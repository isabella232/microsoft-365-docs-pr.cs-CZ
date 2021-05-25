---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Zjistěte, jak Windows autopilota k nastavení nových Windows 10 zařízení pro vaši firmu, aby byla připravená k použití pro zaměstnance.
ms.openlocfilehash: e178e7df220e89605502d9ed400265bcd963e57e
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636100"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="541f3-103">Podrobné pokyny k přidání zařízení a profilů Autopilota</span><span class="sxs-lookup"><span data-stu-id="541f3-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="541f3-104">Pomocí Windows AutoPilot můžete nastavit nová **Windows 10** zařízení pro vaši firmu, aby byla připravená k použití, když je dáte svým zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="541f3-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="541f3-105">Požadavky na zařízení</span><span class="sxs-lookup"><span data-stu-id="541f3-105">Device requirements</span></span>

<span data-ttu-id="541f3-106">Zařízení musí splňovat tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="541f3-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="541f3-107">Windows 10 verze 1703 nebo novější</span><span class="sxs-lookup"><span data-stu-id="541f3-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="541f3-108">Nová zařízení, která ještě Windows prostředí</span><span class="sxs-lookup"><span data-stu-id="541f3-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="541f3-109">Vytvoření zařízení a profilů pomocí průvodce instalací</span><span class="sxs-lookup"><span data-stu-id="541f3-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="541f3-110">Pokud jste skupiny zařízení nebo profily ještě nevytáčili, nejlepší způsob, jak začít, je použití podrobného průvodce.</span><span class="sxs-lookup"><span data-stu-id="541f3-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="541f3-111">Můžete také [přidávat zařízení a](create-and-edit-autopilot-devices.md) [přiřazovat jim](create-and-edit-autopilot-profiles.md) profily bez použití průvodce.</span><span class="sxs-lookup"><span data-stu-id="541f3-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="541f3-112">Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="541f3-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="541f3-113">V levém navigačním podokně zvolte **Zařízení** \> **AutoPilota**.</span><span class="sxs-lookup"><span data-stu-id="541f3-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![V Centru pro správu vyberte zařízení a pak AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="541f3-115">Na stránce **AutoPilot** klikněte nebo klepněte na **Úvodní příručka**.</span><span class="sxs-lookup"><span data-stu-id="541f3-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="541f3-117">Na Upload .csv **souboru se seznamem** zařízení přejděte do umístění, kde máte připravený soubor .CSV a pak **otevřít** \> **další.**</span><span class="sxs-lookup"><span data-stu-id="541f3-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="541f3-118">Soubor musí mít tři záhlaví:</span><span class="sxs-lookup"><span data-stu-id="541f3-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="541f3-119">Sloupec A: Sériové číslo zařízení</span><span class="sxs-lookup"><span data-stu-id="541f3-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="541f3-120">Sloupec B: ID produktu Windows</span><span class="sxs-lookup"><span data-stu-id="541f3-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="541f3-121">Sloupec C: Hodnota hash hardwaru</span><span class="sxs-lookup"><span data-stu-id="541f3-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="541f3-122">Tyto informace můžete získat od dodavatele hardwaru nebo můžete ke generování souboru CSV použít skript [Get-WindowsAutoPilotInfo PowerShellu.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="541f3-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="541f3-p103">Další informace najdete v článku [Soubor CSV se seznamem zařízení](../admin/misc/device-list.md). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**.</span><span class="sxs-lookup"><span data-stu-id="541f3-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="541f3-125">Tento skript používá službu WMI k načtení vlastností potřebných k registraci zařízení u Windows Autopilota.</span><span class="sxs-lookup"><span data-stu-id="541f3-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="541f3-126">Všimněte si, že je normální, že výsledný soubor CSV neshromažďuje hodnotu ID produktu Windows (PKID), protože to není nutné k registraci zařízení a PKID je NULL ve výstupním souboru CSV je zcela v pořádku.</span><span class="sxs-lookup"><span data-stu-id="541f3-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="541f3-127">Vyplní se jenom sériové číslo a hardwarová hodnota hash.</span><span class="sxs-lookup"><span data-stu-id="541f3-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="541f3-128">Na **stránce Přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový.</span><span class="sxs-lookup"><span data-stu-id="541f3-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="541f3-129">Pokud ho ještě nemáte, zobrazí se výzva k jeho vytvoření.</span><span class="sxs-lookup"><span data-stu-id="541f3-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="541f3-130">Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="541f3-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="541f3-131">Výchozí funkce jsou povinné a automaticky se nastavují.</span><span class="sxs-lookup"><span data-stu-id="541f3-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="541f3-132">Výchozí funkce:</span><span class="sxs-lookup"><span data-stu-id="541f3-132">The default features are:</span></span>
    
    - <span data-ttu-id="541f3-133">Přeskočte cortanu, OneDrive a registraci OEM.</span><span class="sxs-lookup"><span data-stu-id="541f3-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="541f3-134">Vytvoření postupu přihlášení doplněného o značku společnosti.</span><span class="sxs-lookup"><span data-stu-id="541f3-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="541f3-135">Připojení na zařízeních Azure Active Directory účty a automaticky je zaregistrujte, aby je Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="541f3-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="541f3-136">Další informace najdete v tématu [O nastavení profilu AutoPilota](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="541f3-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="541f3-137">Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="541f3-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="541f3-138">Zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="541f3-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="541f3-139">**Hotovo znamená,** že profil, který jste vytvořili (nebo zvolili) se použije u skupiny zařízení, kterou jste vytvořili tak, že nahrajete seznam zařízení.</span><span class="sxs-lookup"><span data-stu-id="541f3-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="541f3-140">Nastavení se projeví, když se uživatelé zařízení přihlásí příště.</span><span class="sxs-lookup"><span data-stu-id="541f3-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="541f3-141">Zvolte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="541f3-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="541f3-142">Související obsah</span><span class="sxs-lookup"><span data-stu-id="541f3-142">Related content</span></span>

<span data-ttu-id="541f3-143">[Nastavení profilu AutoPilota](autopilot-profile-settings.md) (článek)</span><span class="sxs-lookup"><span data-stu-id="541f3-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="541f3-144">[Možnosti ochrany vašich zařízení a dat aplikací](../admin/devices/choose-device-security.md) (článek)</span><span class="sxs-lookup"><span data-stu-id="541f3-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>
