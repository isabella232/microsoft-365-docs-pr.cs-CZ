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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Další informace o použití AutoPilot systému Windows k nastavení nových Windows 10 zařízení pro vaše podnikání.
ms.openlocfilehash: 9a70978156fb26ac3aad08f1758b7ee125067d38
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072144"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="54a0c-103">Podrobné pokyny k přidání zařízení a profilů Autopilota</span><span class="sxs-lookup"><span data-stu-id="54a0c-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="54a0c-104">AutoPilot systému Windows slouží k nastavení **nových** Windows 10 zařízení pro vaše podnikání tak, aby byly připraveny pro produktivní využití co nejdříve poskytnout vašim zaměstnancům.</span><span class="sxs-lookup"><span data-stu-id="54a0c-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="54a0c-105">Požadavky na zařízení</span><span class="sxs-lookup"><span data-stu-id="54a0c-105">Device requirements</span></span>

<span data-ttu-id="54a0c-106">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="54a0c-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="54a0c-107">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="54a0c-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="54a0c-108">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="54a0c-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="54a0c-109">Vytvoření zařízení a profilů pomocí průvodce instalací</span><span class="sxs-lookup"><span data-stu-id="54a0c-109">Use the setup guide to create devices and profiles</span></span>

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="54a0c-111">Pokud jste ještě nevytvořili skupiny zařízení ani jejich profily, bude nejlepší, když na začátku použijete podrobného průvodce. [Přidat zařízení](create-and-edit-autopilot-devices.md) a [přiřadit profily](create-and-edit-autopilot-profiles.md) ale můžete i bez průvodce.</span><span class="sxs-lookup"><span data-stu-id="54a0c-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="54a0c-112">Přejděte na stránku Správce na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="54a0c-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="54a0c-113">Na navigace vlevo zvolte **zařízení** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![V Centru správy vyberte zařízení a pak AutoPilot.](media/AutoPilot.png)
  
2. <span data-ttu-id="54a0c-115">Na stránce **AutoPilot** klepněte na položku nebo klepněte na tlačítko **Spustit Průvodce**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="54a0c-p101">Na stránce **Nahrát soubor .csv obsahující seznam zařízení** přejděte k místu, kde máte připravený soubor CSV, a vyberte **Otevřít** \> **Další**. Soubor musí mít tři záhlaví:</span><span class="sxs-lookup"><span data-stu-id="54a0c-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="54a0c-119">Sloupec A: Sériové číslo zařízení</span><span class="sxs-lookup"><span data-stu-id="54a0c-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="54a0c-120">Sloupec B: ID produktu Windows</span><span class="sxs-lookup"><span data-stu-id="54a0c-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="54a0c-121">Sloupec C: Hodnota hash hardwaru</span><span class="sxs-lookup"><span data-stu-id="54a0c-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="54a0c-122">Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV.</span><span class="sxs-lookup"><span data-stu-id="54a0c-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="54a0c-p102">Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="54a0c-p103">Na stránce **Přiřadit profil** můžete vybrat stávající profil nebo můžete vytvořit profil nový. Pokud ho ještě nemáte, zobrazí se výzva k vytvoření nového profilu.</span><span class="sxs-lookup"><span data-stu-id="54a0c-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="54a0c-127">Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="54a0c-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="54a0c-p104">Výchozí funkce jsou povinné a nastaví se automaticky. Výchozí funkce:</span><span class="sxs-lookup"><span data-stu-id="54a0c-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="54a0c-130">Přeskočení Cortany, OneDrivu a registrace OEM.</span><span class="sxs-lookup"><span data-stu-id="54a0c-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="54a0c-131">Vytvoření postupu přihlášení doplněného o značku společnosti.</span><span class="sxs-lookup"><span data-stu-id="54a0c-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="54a0c-132">Zařízení se připojí k účtům adresářové služby Azure Active Directory a automaticky se zaregistrují, aby je bylo možné spravovat ve službě Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="54a0c-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="54a0c-133">Další informace najdete v článku</span><span class="sxs-lookup"><span data-stu-id="54a0c-133">For more information, see</span></span>
    
    <span data-ttu-id="54a0c-134">[Informace o nastavení profilu AutoPilota](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="54a0c-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="54a0c-135">Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="54a0c-136">Zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="54a0c-p105">Stránka **Hotovo!** znamená, že vytvořený (nebo zvolený) profil se použije u skupiny zařízení vytvořené nahráním seznamu zařízení. Tato nastavení platí i při příštím přihlášení uživatelů zařízení. Zvolte **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="54a0c-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    