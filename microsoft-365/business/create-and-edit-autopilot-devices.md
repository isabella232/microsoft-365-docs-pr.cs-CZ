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
# <a name="create-and-edit-autopilot-devices"></a>Vytvoření a úpravy zařízení pomocí AutoPilota

## <a name="upload-a-list-of-devices"></a>Nahrání seznamu zařízení

K nahrání zařízení můžete použít [podrobného průvodce](add-autopilot-devices-and-profile.md). Zařízení také můžete nahrát na kartě **Zařízení**. 
  
Zařízení musejí splňovat tyto podmínky:
  
- Windows 10 verze 1703 nebo novější.
    
- Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.

1. V centru správce Business 365 Microsoft zvolte **zařízení** \> **AutoPilot**.
  
2. Na stránce **AutoPilot** zvolte kartu **zařízení** \> **Přidat zařízení**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Přidat zařízení** vyhledejte [seznam zařízení souboru CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) mají připravené \> **Uložit** \> **Zavřít**.
    
    Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Přiřazení profilu zařízení nebo skupině zařízení

1. Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko u jednoho nebo více zařízení. 
    
2. Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil. 
    
    Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md). 
    
