---
title: Vytvoření a úpravy profilů AutoPilota
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Naučte se vytvářet, upravovat, odstraňovat nebo odebírat profily automatických Opilot.
ms.openlocfilehash: 4305340a2fc5df8202cf4d85f9e2541690bf9ed0
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574712"
---
# <a name="create-and-edit-autopilot-profiles"></a>Vytvoření a úpravy profilů AutoPilota

## <a name="create-a-profile"></a>Vytvoření profilu

Profil se používá pro zařízení nebo skupinu zařízení.
  
1. V centru Microsoft 365 Business admin zvolte **zařízení** \> **autopilot**.
  
2. Na stránce **autopilot** zvolte záložku \> **profily** **vytvořit profil**.
    
3. Na stránce **Vytvořit profil** zadejte název, který vám pomůže profil identifikovat, třeba Marketing, zapněte požadované nastavení (další informace najdete v článku [O nastavení profilu AutoPilota](autopilot-profile-settings.md)) a zvolte **Uložit**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Použití profilu u zařízení

Jakmile vytvoříte profil, můžete ho použít pro zařízení nebo skupinu zařízení. Stávající profil můžete vybrat v [podrobném průvodci](add-autopilot-devices-and-profile.md), můžete ho použít u nových zařízení nebo ho můžete u zařízení nebo skupiny zařízení nahradit. 
  
1. Na stránce **Připravit Windows** zvolte kartu **Zařízení**. 
    
2. Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte profil v rozevíracím seznamu **Přiřazený profil** \> **Uložit**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Úprava, odstranění nebo odebrání profilu

Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace. 
  
### <a name="edit-a-profile"></a>Úprava profilu

1. Na stránce **Připravit Windows** zvolte kartu **Profily**. 
    
2. Klikněte na zaškrtávací políčko vedle názvu zařízení. Na panelu **Profil** můžete aktualizovat dostupná nastavení \> **Uložit**.
    
    Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.
    
### <a name="delete-a-profile"></a>Odstranění profilu

1. Na stránce **Připravit Windows** zvolte kartu **Profily**. 
    
2. Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Profil** klikněte na **Odstranit profil** \> **Uložit**.
    
    Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.
    
### <a name="remove-a-profile"></a>Odebrání profilu

1. Na stránce **Připravit Windows** zvolte kartu **Zařízení**. 
    
2. Klikněte na zaškrtávací políčko vedle názvu zařízení a na panelu **Zařízení** vyberte v rozevíracím seznamu **Přiřazený profil** možnost **Žádný** \> **Uložit**.
    
