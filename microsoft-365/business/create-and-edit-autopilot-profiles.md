---
title: Vytvoření a úpravy profilů AutoPilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Zjistěte, jak můžete vytvořit, upravit, odstranit nebo odebrat profily AutoPilot. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277084"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="f4dfe-103">Vytvoření a úpravy profilů AutoPilota</span><span class="sxs-lookup"><span data-stu-id="f4dfe-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="f4dfe-104">Vytvoření profilu</span><span class="sxs-lookup"><span data-stu-id="f4dfe-104">Create a profile</span></span>

<span data-ttu-id="f4dfe-105">Profil se používá pro zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="f4dfe-106">V centru správce Business 365 Microsoft zvolte **zařízení** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="f4dfe-107">Na stránce **AutoPilot** zvolte kartu **profily** \> **vytvořit profil**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="f4dfe-108">Na stránce **Vytvořit profil** zadejte název, který vám pomůže profil identifikovat, třeba Marketing, zapněte požadované nastavení (další informace najdete v článku [O nastavení profilu AutoPilota](autopilot-profile-settings.md)) a zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="f4dfe-110">Použití profilu u zařízení</span><span class="sxs-lookup"><span data-stu-id="f4dfe-110">Apply profile to a device</span></span>

<span data-ttu-id="f4dfe-p101">Jakmile vytvoříte profil, můžete ho použít pro zařízení nebo skupinu zařízení. Stávající profil můžete vybrat v [podrobném průvodci](add-autopilot-devices-and-profile.md), můžete ho použít u nových zařízení nebo ho můžete u zařízení nebo skupiny zařízení nahradit.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="f4dfe-113">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="f4dfe-114">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte profil v rozevíracím seznamu **Přiřazený profil** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="f4dfe-116">Úprava, odstranění nebo odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="f4dfe-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="f4dfe-p102">Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="f4dfe-120">Úprava profilu</span><span class="sxs-lookup"><span data-stu-id="f4dfe-120">Edit a profile</span></span>

1. <span data-ttu-id="f4dfe-121">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="f4dfe-122">Klikněte na zaškrtávací políčko vedle názvu zařízení. Na panelu **Profil** můžete aktualizovat dostupná nastavení \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="f4dfe-123">Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="f4dfe-124">Odstranění profilu</span><span class="sxs-lookup"><span data-stu-id="f4dfe-124">Delete a profile</span></span>

1. <span data-ttu-id="f4dfe-125">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="f4dfe-126">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Profil** klikněte na **Odstranit profil** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="f4dfe-127">Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="f4dfe-128">Odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="f4dfe-128">Remove a profile</span></span>

1. <span data-ttu-id="f4dfe-129">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="f4dfe-130">Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** možnost **Žádný** \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f4dfe-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
