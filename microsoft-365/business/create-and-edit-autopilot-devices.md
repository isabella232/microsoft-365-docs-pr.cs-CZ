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
description: Naučte se odesílat zařízení pomocí služby AutoPilot v aplikaci Microsoft 365 Business. K zařízení nebo skupině zařízení můžete přiřadit profil.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320252"
---
# <a name="create-and-edit-autopilot-devices"></a>Vytvoření a úpravy zařízení pomocí AutoPilota

## <a name="upload-a-list-of-devices"></a>Nahrání seznamu zařízení

K nahrání zařízení můžete použít [podrobný průvodce](add-autopilot-devices-and-profile.md) , ale můžete také odeslat zařízení na kartě **zařízení** . 
  
Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která nebyla součástí systému Windows,

1. V centru Microsoft 365 Business admin zvolte **zařízení** \> **autopilot**.
  
2. Na stránce **autopilot** zvolte kartu \> **zařízení** **Přidat zařízení**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Přidat zařízení** přejděte do [souboru CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) , který jste připravili \> **Uložit** \> **.**
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete vytvořit soubor CSV pomocí [skriptu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) . 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Přiřazení profilu zařízení nebo skupině zařízení

1. Na stránce **Příprava systému Windows** zvolte kartu **zařízení** a zaškrtněte políčko u jednoho nebo více zařízení. 
    
2. Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil. 
    
    Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md). 
    
