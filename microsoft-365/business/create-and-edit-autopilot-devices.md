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
description: Přečtěte si, jak nahrávat zařízení pomocí autopilota v Microsoft u 365 Business Premium. Profil můžete přiřadit k zařízení nebo skupině zařízení.
ms.openlocfilehash: f2a7f801ae471352595a36b355a874b2de653326
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627388"
---
# <a name="create-and-edit-autopilot-devices"></a>Vytvoření a úpravy zařízení pomocí AutoPilota

## <a name="upload-a-list-of-devices"></a>Nahrání seznamu zařízení

Pomocí [podrobného průvodce](add-autopilot-devices-and-profile.md) můžete nahrávat zařízení, ale zařízení můžete nahrát také na kartě **Zařízení.** 
  
Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která ještě neprošla systémem Windows, jsou po vybalení

1. V Centru pro správu Microsoftu 365 zvolte **Zařízení** \> **AutoPilot**.
  
2. Na stránce **AutoPilot** zvolte \> kartu **Zařízení** **Přidat zařízení**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Na panelu **Přidat zařízení** přejděte do [souboru CSV seznamu zařízení,](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) který jste připravili \> **Uložit** \> **zavřít**.
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete použít [skript Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) ke generování souboru CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Přiřazení profilu zařízení nebo skupině zařízení

1. Na stránce **Příprava Windows** zvolte kartu **Zařízení** a zaškrtněte políčko vedle jednoho nebo více zařízení. 
    
2. Na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** některý profil. 
    
    Pokud jste profily ještě nevytvořili, přečtěte si článek [Vytvoření a úpravy profilů AutoPilota](create-and-edit-autopilot-profiles.md). 
    
