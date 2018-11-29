---
title: Vytvoření a úpravy zařízení pomocí AutoPilota
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Zjistěte, jak nahrát pomocí AutoPilot v Microsoft 365 Business zařízení. Můžete přiřadit profil zařízení nebo skupiny zařízení.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982931"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="89891-104">Vytvoření a úpravy zařízení pomocí AutoPilota</span><span class="sxs-lookup"><span data-stu-id="89891-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="89891-105">Nahrání seznamu zařízení</span><span class="sxs-lookup"><span data-stu-id="89891-105">Upload a list of devices</span></span>

<span data-ttu-id="89891-106">K nahrání zařízení můžete použít [podrobného průvodce](add-autopilot-devices-and-profile.md). Zařízení také můžete nahrát na kartě **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="89891-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="89891-107">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="89891-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="89891-108">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="89891-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="89891-109">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="89891-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="89891-110">V Centru pro správu Microsoft 365 Business zvolte na kartě **Akce zařízení** možnost **Nasadit Windows pomocí Autopilota**.</span><span class="sxs-lookup"><span data-stu-id="89891-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="89891-112">Na stránce **Připravit Windows** zvolte kartu **Zařízení** \> **Přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="89891-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="89891-114">Na panelu **Přidat zařízení** vyhledejte [seznam zařízení souboru CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) mají připravené \> **Uložit** \> **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="89891-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="89891-115">Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV.</span><span class="sxs-lookup"><span data-stu-id="89891-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="89891-116">Přiřazení profilu zařízení nebo skupině zařízení</span><span class="sxs-lookup"><span data-stu-id="89891-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="89891-117">Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko u jednoho nebo více zařízení.</span><span class="sxs-lookup"><span data-stu-id="89891-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="89891-118">Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil.</span><span class="sxs-lookup"><span data-stu-id="89891-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="89891-119">Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="89891-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
