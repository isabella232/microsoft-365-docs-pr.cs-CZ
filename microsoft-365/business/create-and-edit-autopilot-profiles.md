---
title: Vytvoření a úpravy profilů AutoPilota
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
description: Naučte se vytvářet, upravovat, odstraňovat nebo odebírat profily automatických Opilot.
ms.openlocfilehash: f7fdc2632e93c48e043fe158842f8395d6a89e14
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320232"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="cd3d0-103">Vytvoření a úpravy profilů AutoPilota</span><span class="sxs-lookup"><span data-stu-id="cd3d0-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="cd3d0-104">Vytvoření profilu</span><span class="sxs-lookup"><span data-stu-id="cd3d0-104">Create a profile</span></span>

<span data-ttu-id="cd3d0-105">Profil se používá pro zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="cd3d0-106">V centru Microsoft 365 Business admin zvolte **zařízení** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="cd3d0-107">Na stránce **autopilot** zvolte záložku \> **profily** **vytvořit profil**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="cd3d0-108">Na stránce **vytvořit profil** zadejte název profilu, který vám pomůže jej identifikovat, například marketing.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="cd3d0-109">Zapněte požadované nastavení a pak klepněte na tlačítko **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="cd3d0-110">Další informace o nastavení profilu AutoPilot naleznete v tématu [o nastavení profilu autopilot](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="cd3d0-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="cd3d0-112">Použití profilu u zařízení</span><span class="sxs-lookup"><span data-stu-id="cd3d0-112">Apply profile to a device</span></span>

<span data-ttu-id="cd3d0-113">Vytvořený profil můžete použít na zařízení nebo skupinu zařízení.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="cd3d0-114">Můžete vybrat existující profil v [podrobných pokynech](add-autopilot-devices-and-profile.md) a použít jej na nová zařízení nebo nahradit existující profil zařízení nebo skupiny zařízení.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="cd3d0-115">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="cd3d0-116">Zaškrtněte políčko vedle názvu zařízení a v panelu **zařízení** zvolte profil z \> **rozevíracího seznamu** **přiřazený profil** .</span><span class="sxs-lookup"><span data-stu-id="cd3d0-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="cd3d0-118">Úprava, odstranění nebo odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="cd3d0-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="cd3d0-p103">Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="cd3d0-122">Úprava profilu</span><span class="sxs-lookup"><span data-stu-id="cd3d0-122">Edit a profile</span></span>

1. <span data-ttu-id="cd3d0-123">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="cd3d0-124">Zaškrtněte políčko vedle názvu zařízení a v panelu **profil** aktualizujte všechna \> **dostupná nastavení.**</span><span class="sxs-lookup"><span data-stu-id="cd3d0-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="cd3d0-125">Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="cd3d0-126">Odstranění profilu</span><span class="sxs-lookup"><span data-stu-id="cd3d0-126">Delete a profile</span></span>

1. <span data-ttu-id="cd3d0-127">Na stránce **Připravit Windows** zvolte kartu **Profily**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="cd3d0-128">Zaškrtněte políčko vedle názvu zařízení a v panelu **profil** vyberte možnost **Odstranit** \> **uložení**profilu.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="cd3d0-129">Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="cd3d0-130">Odebrání profilu</span><span class="sxs-lookup"><span data-stu-id="cd3d0-130">Remove a profile</span></span>

1. <span data-ttu-id="cd3d0-131">Na stránce **Připravit Windows** zvolte kartu **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="cd3d0-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="cd3d0-132">Zaškrtněte políčko vedle názvu zařízení a v panelu **zařízení** vyberte v \> **rozevíracím seznamu** **přiřazený profil** položku **žádný** .</span><span class="sxs-lookup"><span data-stu-id="cd3d0-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
