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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Přečtěte si, jak nahrávat zařízení pomocí automatického pilotního projektu v Microsoft 365 Business. Můžete přiřadit profil zařízení nebo skupině zařízení.
ms.openlocfilehash: 640e4af7cccde83c87d90a875c1d44dead7255ca
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065970"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="fb4ac-104">Vytvoření a úpravy zařízení pomocí AutoPilota</span><span class="sxs-lookup"><span data-stu-id="fb4ac-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="fb4ac-105">Nahrání seznamu zařízení</span><span class="sxs-lookup"><span data-stu-id="fb4ac-105">Upload a list of devices</span></span>

<span data-ttu-id="fb4ac-106">K nahrávání zařízení můžete použít [podrobný průvodce,](add-autopilot-devices-and-profile.md) ale zařízení můžete také nahrát na kartě **Zařízení.**</span><span class="sxs-lookup"><span data-stu-id="fb4ac-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="fb4ac-107">Zařízení musí splňovat tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="fb4ac-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="fb4ac-108">Windows 10, verze 1703 nebo novější</span><span class="sxs-lookup"><span data-stu-id="fb4ac-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="fb4ac-109">Nová zařízení, která neprošla systémem Windows, jsou v rámečku</span><span class="sxs-lookup"><span data-stu-id="fb4ac-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="fb4ac-110">V Centru pro správu microsoft365 Business zvolte **Zařízení** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="fb4ac-111">Na stránce **AutoPilot** zvolte \> kartu **Zařízení** **Přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="fb4ac-113">Na panelu **Přidat zařízení** přejděte na [soubor CSV seznamu zařízení,](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) který jste připravili \> **uložit** \> **zavřít**.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="fb4ac-114">Tyto informace můžete získat od dodavatele hardwaru nebo můžete použít [skript Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) ke generování souboru CSV.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="fb4ac-115">Přiřazení profilu zařízení nebo skupině zařízení</span><span class="sxs-lookup"><span data-stu-id="fb4ac-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="fb4ac-116">Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko vedle jednoho nebo více zařízení.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="fb4ac-117">Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil.</span><span class="sxs-lookup"><span data-stu-id="fb4ac-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="fb4ac-118">Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="fb4ac-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
