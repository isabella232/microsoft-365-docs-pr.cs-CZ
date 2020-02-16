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
# <a name="create-and-edit-autopilot-devices"></a>Vytvoření a úpravy zařízení pomocí AutoPilota

## <a name="upload-a-list-of-devices"></a>Nahrání seznamu zařízení

K nahrávání zařízení můžete použít [podrobný průvodce,](add-autopilot-devices-and-profile.md) ale zařízení můžete také nahrát na kartě **Zařízení.** 
  
Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která neprošla systémem Windows, jsou v rámečku

1. V Centru pro správu microsoft365 Business zvolte **Zařízení** \> **AutoPilot**.
  
2. Na stránce **AutoPilot** zvolte \> kartu **Zařízení** **Přidat zařízení**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Přidat zařízení** přejděte na [soubor CSV seznamu zařízení,](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) který jste připravili \> **uložit** \> **zavřít**.
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete použít [skript Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) ke generování souboru CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Přiřazení profilu zařízení nebo skupině zařízení

1. Na stránce **Připravit Windows** zvolte kartu **Zařízení** a zaškrtněte políčko vedle jednoho nebo více zařízení. 
    
2. Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil. 
    
    Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md). 
    
