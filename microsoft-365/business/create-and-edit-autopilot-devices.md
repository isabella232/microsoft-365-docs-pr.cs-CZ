---
title: Vytvoření a úpravy zařízení pomocí AutoPilota
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Zjistěte, jak nahrávat zařízení pomocí AutoPilota v Microsoft 365 Business Premium. Profil můžete přiřadit zařízení nebo skupině zařízení.
ms.openlocfilehash: 910abb98b94b749177b04cd12c766f82d348e379
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913392"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="b7851-104">Vytvoření a úpravy zařízení pomocí AutoPilota</span><span class="sxs-lookup"><span data-stu-id="b7851-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="b7851-105">Nahrání seznamu zařízení</span><span class="sxs-lookup"><span data-stu-id="b7851-105">Upload a list of devices</span></span>

<span data-ttu-id="b7851-106">K [nahrání](add-autopilot-devices-and-profile.md) zařízení můžete použít podrobný průvodce, ale zařízení můžete nahrát taky na **kartě** Zařízení.</span><span class="sxs-lookup"><span data-stu-id="b7851-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="b7851-107">Zařízení musí splňovat tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="b7851-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="b7851-108">Windows 10, verze 1703 nebo novější</span><span class="sxs-lookup"><span data-stu-id="b7851-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="b7851-109">Nová zařízení, která ještě nevyužíla prostředí Windows</span><span class="sxs-lookup"><span data-stu-id="b7851-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="b7851-110">V Centru pro správu Microsoftu 365 zvolte **Zařízení** \> **AutoPilota**.</span><span class="sxs-lookup"><span data-stu-id="b7851-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="b7851-111">Na stránce **AutoPilot** zvolte kartu **Zařízení –** \> **přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="b7851-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="b7851-113">Na panelu **Přidat zařízení** přejděte na soubor CSV [se seznamem](../admin/misc/device-list.md) zařízení, který jste připravili \> **Pro uložení** \> **zavřít.**</span><span class="sxs-lookup"><span data-stu-id="b7851-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="b7851-114">Tyto informace můžete získat od dodavatele hardwaru nebo můžete ke generování souboru CSV použít skript [Get-WindowsAutoPilotInfo PowerShellu.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo)</span><span class="sxs-lookup"><span data-stu-id="b7851-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="b7851-115">Přiřazení profilu zařízení nebo skupině zařízení</span><span class="sxs-lookup"><span data-stu-id="b7851-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="b7851-116">Na stránce **Příprava Windows**  zvolte kartu Zařízení a zaškrtněte políčko vedle jednoho nebo více zařízení.</span><span class="sxs-lookup"><span data-stu-id="b7851-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="b7851-117">Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil.</span><span class="sxs-lookup"><span data-stu-id="b7851-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="b7851-118">Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="b7851-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
