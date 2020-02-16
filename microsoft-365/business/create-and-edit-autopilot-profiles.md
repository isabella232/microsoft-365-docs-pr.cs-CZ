---
title: Vytvoření a úpravy profilů AutoPilota
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
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Naučte se vytvářet, upravovat, odstraňovat nebo odebírat profily autopilota.
ms.openlocfilehash: 28f5b679d58711d11d9af26dffb7022024b72c79
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065877"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="6ea53-103">Vytvoření a úpravy profilů AutoPilota</span><span class="sxs-lookup"><span data-stu-id="6ea53-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="6ea53-104">Vytvoření profilu</span><span class="sxs-lookup"><span data-stu-id="6ea53-104">Create a profile</span></span>

<span data-ttu-id="6ea53-105">Profil se používá pro zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="6ea53-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="6ea53-106">V Centru pro správu microsoft365 Business zvolte **Zařízení** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="6ea53-107">Na stránce **AutoPilot** zvolte \> kartu **Profily** **Vytvořit profil**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="6ea53-108">Na stránce **Vytvořit profil** zadejte název profilu, který vám pomůže ho identifikovat, například Marketing.</span><span class="sxs-lookup"><span data-stu-id="6ea53-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="6ea53-109">Zapněte požadované nastavení a pak zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="6ea53-110">Další informace o nastavení profilu autopilota naleznete [v tématu O nastavení profilu autopilota](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="6ea53-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="6ea53-112">Použití profilu u zařízení</span><span class="sxs-lookup"><span data-stu-id="6ea53-112">Apply profile to a device</span></span>

<span data-ttu-id="6ea53-113">Po vytvoření profilu jej můžete použít na zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="6ea53-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="6ea53-114">Můžete vybrat existující profil v [podrobné příručce](add-autopilot-devices-and-profile.md) a aplikovat ho na nová zařízení nebo nahradit existující profil zařízení nebo skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="6ea53-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="6ea53-115">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="6ea53-116">Zaškrtněte políčko vedle názvu zařízení a v panelu **Zařízení** zvolte profil z \> rozevíracího seznamu **Přiřazený profil** **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="6ea53-118">Úprava, odstranění nebo odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="6ea53-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="6ea53-p103">Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="6ea53-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="6ea53-122">Úprava profilu</span><span class="sxs-lookup"><span data-stu-id="6ea53-122">Edit a profile</span></span>

1. <span data-ttu-id="6ea53-123">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="6ea53-124">Zaškrtněte políčko vedle názvu zařízení a v panelu **Profil** aktualizujte libovolné dostupné nastavení \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="6ea53-125">Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.</span><span class="sxs-lookup"><span data-stu-id="6ea53-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="6ea53-126">Odstranění profilu</span><span class="sxs-lookup"><span data-stu-id="6ea53-126">Delete a profile</span></span>

1. <span data-ttu-id="6ea53-127">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="6ea53-128">Zaškrtněte políčko vedle názvu zařízení a v panelu **Profil** vyberte **Odstranit profil** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="6ea53-129">Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.</span><span class="sxs-lookup"><span data-stu-id="6ea53-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="6ea53-130">Odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="6ea53-130">Remove a profile</span></span>

1. <span data-ttu-id="6ea53-131">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="6ea53-132">Zaškrtněte políčko vedle názvu zařízení a v panelu **Zařízení** zvolte **Žádné** z rozevíracího seznamu \> **Přiřazený profil** **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ea53-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
