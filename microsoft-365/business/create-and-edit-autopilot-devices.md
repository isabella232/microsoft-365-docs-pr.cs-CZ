---
title: Vytvoření a úpravy zařízení pomocí AutoPilota
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Naučte se odesílat zařízení pomocí služby AutoPilot v aplikaci Microsoft 365 Business. K zařízení nebo skupině zařízení můžete přiřadit profil.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288009"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="26552-104">Vytvoření a úpravy zařízení pomocí AutoPilota</span><span class="sxs-lookup"><span data-stu-id="26552-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="26552-105">Nahrání seznamu zařízení</span><span class="sxs-lookup"><span data-stu-id="26552-105">Upload a list of devices</span></span>

<span data-ttu-id="26552-106">K nahrání zařízení můžete použít [podrobného průvodce](add-autopilot-devices-and-profile.md). Zařízení také můžete nahrát na kartě **Zařízení**.</span><span class="sxs-lookup"><span data-stu-id="26552-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="26552-107">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="26552-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="26552-108">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="26552-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="26552-109">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="26552-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="26552-110">V centru Microsoft 365 Business admin zvolte **zařízení** \> **autopilot**.</span><span class="sxs-lookup"><span data-stu-id="26552-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="26552-111">Na stránce **autopilot** zvolte kartu \> **zařízení** **Přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="26552-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="26552-113">V panelu **Přidat zařízení** přejděte do [souboru CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , který jste připravili \> pro **uložení** \> **.**</span><span class="sxs-lookup"><span data-stu-id="26552-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="26552-114">Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV.</span><span class="sxs-lookup"><span data-stu-id="26552-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="26552-115">Přiřazení profilu zařízení nebo skupině zařízení</span><span class="sxs-lookup"><span data-stu-id="26552-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="26552-116">Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko u jednoho nebo více zařízení.</span><span class="sxs-lookup"><span data-stu-id="26552-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="26552-117">Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil.</span><span class="sxs-lookup"><span data-stu-id="26552-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="26552-118">Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="26552-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
