---
title: Vytvoření a úpravy profilů AutoPilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Zjistěte, jak můžete vytvořit, upravit, odstranit nebo odebrat profily AutoPilot. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983131"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="c29b4-103">Vytvoření a úpravy profilů AutoPilota</span><span class="sxs-lookup"><span data-stu-id="c29b4-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="c29b4-104">Vytvoření profilu</span><span class="sxs-lookup"><span data-stu-id="c29b4-104">Create a profile</span></span>

<span data-ttu-id="c29b4-105">Profil se používá pro zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="c29b4-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="c29b4-106">V Centru pro správu Microsoft 365 Business zvolte na kartě **Akce zařízení** možnost **Nasadit Windows pomocí Autopilota**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="c29b4-108">Na stránce **Připravit Windows** zvolte kartu **Profily** \> **Vytvořit profil**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="c29b4-109">Na stránce **Vytvořit profil** zadejte název, který vám pomůže profil identifikovat, třeba Marketing, zapněte požadované nastavení (další informace najdete v článku [O nastavení profilu AutoPilota](autopilot-profile-settings.md)) a zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="c29b4-111">Použití profilu u zařízení</span><span class="sxs-lookup"><span data-stu-id="c29b4-111">Apply profile to a device</span></span>

<span data-ttu-id="c29b4-p101">Jakmile vytvoříte profil, můžete ho použít pro zařízení nebo skupinu zařízení. Stávající profil můžete vybrat v [podrobném průvodci](add-autopilot-devices-and-profile.md), můžete ho použít u nových zařízení nebo ho můžete u zařízení nebo skupiny zařízení nahradit.</span><span class="sxs-lookup"><span data-stu-id="c29b4-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="c29b4-114">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c29b4-115">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte profil v rozevíracím seznamu **Přiřazený profil** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="c29b4-117">Úprava, odstranění nebo odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="c29b4-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="c29b4-p102">Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="c29b4-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="c29b4-121">Úprava profilu</span><span class="sxs-lookup"><span data-stu-id="c29b4-121">Edit a profile</span></span>

1. <span data-ttu-id="c29b4-122">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c29b4-123">Klikněte na zaškrtávací políčko vedle názvu zařízení. Na panelu **Profil** můžete aktualizovat dostupná nastavení \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="c29b4-124">Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.</span><span class="sxs-lookup"><span data-stu-id="c29b4-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="c29b4-125">Odstranění profilu</span><span class="sxs-lookup"><span data-stu-id="c29b4-125">Delete a profile</span></span>

1. <span data-ttu-id="c29b4-126">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c29b4-127">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Profil** klikněte na **Odstranit profil** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="c29b4-128">Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.</span><span class="sxs-lookup"><span data-stu-id="c29b4-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="c29b4-129">Odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="c29b4-129">Remove a profile</span></span>

1. <span data-ttu-id="c29b4-130">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c29b4-131">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** možnost **Žádný** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c29b4-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
