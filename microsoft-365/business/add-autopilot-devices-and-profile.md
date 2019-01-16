---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Další informace o použití AutoPilot systému Windows k nastavení nových Windows 10 zařízení pro vaše podnikání.
ms.openlocfilehash: 56225424125e9eed9f46867837c564aa5d1c4adc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982161"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="ddd0f-103">Podrobné pokyny k přidání zařízení a profilů Autopilota</span><span class="sxs-lookup"><span data-stu-id="ddd0f-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="ddd0f-104">Pomocí Windows AutoPilota můžete ve firmě nastavit nová zařízení s Windows 10, aby byla připravená k použití hned, jak je předáte zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="ddd0f-105">Požadavky na zařízení</span><span class="sxs-lookup"><span data-stu-id="ddd0f-105">Device requirements</span></span>

<span data-ttu-id="ddd0f-106">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="ddd0f-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="ddd0f-107">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="ddd0f-108">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="ddd0f-109">Vytvoření zařízení a profilů pomocí průvodce instalací</span><span class="sxs-lookup"><span data-stu-id="ddd0f-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="ddd0f-110">Pokud jste ještě nevytvořili skupiny zařízení ani jejich profily, bude nejlepší, když na začátku použijete podrobného průvodce. [Přidat zařízení](create-and-edit-autopilot-devices.md) a [přiřadit profily](create-and-edit-autopilot-profiles.md) ale můžete i bez průvodce.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="ddd0f-111">V Centru pro správu Microsoft 365 Business přejděte na kartu **Akce zařízení** a zvolte **Nasadit Windows pomocí Autopilota**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="ddd0f-113">Na stránce **Připravit Windows** klikněte nebo klepněte na **Úvodní příručka**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="ddd0f-p101">Na stránce **Nahrát soubor .csv obsahující seznam zařízení** přejděte k místu, kde máte připravený soubor CSV, a vyberte **Otevřít** \> **Další**. Soubor musí mít tři záhlaví:</span><span class="sxs-lookup"><span data-stu-id="ddd0f-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="ddd0f-117">Sloupec A: Sériové číslo zařízení</span><span class="sxs-lookup"><span data-stu-id="ddd0f-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="ddd0f-118">Sloupec B: ID produktu Windows</span><span class="sxs-lookup"><span data-stu-id="ddd0f-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="ddd0f-119">Sloupec C: Hodnota hash hardwaru</span><span class="sxs-lookup"><span data-stu-id="ddd0f-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="ddd0f-120">Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="ddd0f-p102">Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="ddd0f-p103">Na stránce **Přiřadit profil** můžete vybrat stávající profil nebo můžete vytvořit profil nový. Pokud ho ještě nemáte, zobrazí se výzva k vytvoření nového profilu.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="ddd0f-125">Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="ddd0f-p104">Výchozí funkce jsou povinné a nastaví se automaticky. Výchozí funkce:</span><span class="sxs-lookup"><span data-stu-id="ddd0f-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="ddd0f-128">Přeskočení Cortany, OneDrivu a registrace OEM.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="ddd0f-129">Vytvoření postupu přihlášení doplněného o značku společnosti.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="ddd0f-130">Zařízení se připojí k účtům adresářové služby Azure Active Directory a automaticky se zaregistrují, aby je bylo možné spravovat ve službě Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="ddd0f-131">Další informace najdete v článku</span><span class="sxs-lookup"><span data-stu-id="ddd0f-131">For more information, see</span></span>
    
    <span data-ttu-id="ddd0f-132">[Informace o nastavení profilu AutoPilota](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="ddd0f-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="ddd0f-133">Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="ddd0f-134">Zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="ddd0f-p105">Stránka **Hotovo!** znamená, že vytvořený (nebo zvolený) profil se použije u skupiny zařízení vytvořené nahráním seznamu zařízení. Tato nastavení platí i při příštím přihlášení uživatelů zařízení. Zvolte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="ddd0f-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    