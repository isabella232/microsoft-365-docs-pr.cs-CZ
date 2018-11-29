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
# <a name="create-and-edit-autopilot-devices"></a>Vytvoření a úpravy zařízení pomocí AutoPilota

## <a name="upload-a-list-of-devices"></a>Nahrání seznamu zařízení

K nahrání zařízení můžete použít [podrobného průvodce](add-autopilot-devices-and-profile.md). Zařízení také můžete nahrát na kartě **Zařízení**. 
  
Zařízení musejí splňovat tyto podmínky:
  
- Windows 10 verze 1703 nebo novější.
    
- Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.
    
1. V Centru pro správu Microsoft 365 Business zvolte na kartě **Akce zařízení** možnost **Nasadit Windows pomocí Autopilota**. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Na stránce **Připravit Windows** zvolte kartu **Zařízení** \> **Přidat zařízení**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Přidat zařízení** vyhledejte [seznam zařízení souboru CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) mají připravené \> **Uložit** \> **Zavřít**.
    
    Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Přiřazení profilu zařízení nebo skupině zařízení

1. Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko u jednoho nebo více zařízení. 
    
2. Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil. 
    
    Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md). 
    
