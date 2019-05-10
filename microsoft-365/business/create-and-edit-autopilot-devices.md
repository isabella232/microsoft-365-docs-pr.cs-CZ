---
title: Vytvoření a úpravy zařízení pomocí AutoPilota
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Zjistěte, jak nahrát pomocí AutoPilot v Microsoft 365 Business zařízení. Můžete přiřadit profil zařízení nebo skupiny zařízení.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660376"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="f8622-104">Vytvoření a úpravy zařízení pomocí AutoPilota</span><span class="sxs-lookup"><span data-stu-id="f8622-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="f8622-105">Nahrání seznamu zařízení</span><span class="sxs-lookup"><span data-stu-id="f8622-105">Upload a list of devices</span></span>

<span data-ttu-id="f8622-106">K nahrání zařízení můžete použít [podrobného průvodce](add-autopilot-devices-and-profile.md). Zařízení také můžete nahrát na kartě **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="f8622-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="f8622-107">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="f8622-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="f8622-108">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="f8622-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="f8622-109">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="f8622-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="f8622-110">V centru správce Business 365 Microsoft zvolte **zařízení** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="f8622-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="f8622-111">Na stránce **AutoPilot** zvolte kartu **zařízení** \> **Přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="f8622-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="f8622-113">Na panelu **Přidat zařízení** vyhledejte [seznam zařízení souboru CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) mají připravené \> **Uložit** \> **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="f8622-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="f8622-114">Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV.</span><span class="sxs-lookup"><span data-stu-id="f8622-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="f8622-115">Přiřazení profilu zařízení nebo skupině zařízení</span><span class="sxs-lookup"><span data-stu-id="f8622-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="f8622-116">Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko u jednoho nebo více zařízení.</span><span class="sxs-lookup"><span data-stu-id="f8622-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="f8622-117">Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil.</span><span class="sxs-lookup"><span data-stu-id="f8622-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="f8622-118">Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="f8622-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
