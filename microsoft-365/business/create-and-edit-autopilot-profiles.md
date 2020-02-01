---
title: Vytvoření a úpravy profilů AutoPilota
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Naučte se vytvářet, upravovat, odstraňovat nebo odebírat profily autopilota.
ms.openlocfilehash: 35967cb1f6e2cdeea9d7c42a529526410fa8b586
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593985"
---
# <a name="create-and-edit-autopilot-profiles"></a>Vytvoření a úpravy profilů AutoPilota

## <a name="create-a-profile"></a>Vytvoření profilu

Profil se používá pro zařízení nebo skupinu zařízení.
  
1. V Centru pro správu microsoft365 Business zvolte **Zařízení** \> **AutoPilot**.
  
2. Na stránce **AutoPilot** zvolte \> kartu **Profily** **Vytvořit profil**.
    
3. Na stránce **Vytvořit profil** zadejte název profilu, který vám pomůže ho identifikovat, například Marketing. Zapněte požadované nastavení a pak zvolte **Uložit**. Další informace o nastavení profilu autopilota naleznete [v tématu O nastavení profilu autopilota](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Použití profilu u zařízení

Po vytvoření profilu jej můžete použít na zařízení nebo skupinu zařízení. Můžete vybrat existující profil v [podrobné příručce](add-autopilot-devices-and-profile.md) a aplikovat ho na nová zařízení nebo nahradit existující profil zařízení nebo skupiny zařízení. 
  
1. Na stránce **Připravit Windows** zvolte kartu **Zařízení**. 
    
2. Zaškrtněte políčko vedle názvu zařízení a v panelu **Zařízení** zvolte profil z \> rozevíracího seznamu **Přiřazený profil** **Uložit**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Úprava, odstranění nebo odebrání profilu

Jakmile zařízení přiřadíte profil, můžete profil aktualizovat, a to i tehdy, když jste zařízení předali uživateli. Když se zařízení připojí k internetu, stáhne si v průběhu nastavení nejnovější verzi profilu. Pokud uživatel obnoví v zařízení výchozí tovární nastavení, stáhne si zařízení do profilu nejnovější aktualizace. 
  
### <a name="edit-a-profile"></a>Úprava profilu

1. Na stránce **Připravit Windows** zvolte kartu **Profily**. 
    
2. Zaškrtněte políčko vedle názvu zařízení a v panelu **Profil** aktualizujte libovolné dostupné nastavení \> **Uložit**.
    
    Pokud to uděláte předtím, než uživatel připojí zařízení k internetu, použije se profil v procesu nastavení.
    
### <a name="delete-a-profile"></a>Odstranění profilu

1. Na stránce **Připravit Windows** zvolte kartu **Profily**. 
    
2. Zaškrtněte políčko vedle názvu zařízení a v panelu **Profil** vyberte **Odstranit profil** \> **Uložit**.
    
    Pokud profil odstraníte, odebere se ze zařízení nebo skupiny zařízení, kterým byl přiřazen.
    
### <a name="remove-a-profile"></a>Odebrání profilu

1. Na stránce **Připravit Windows** zvolte kartu **Zařízení**. 
    
2. Zaškrtněte políčko vedle názvu zařízení a v panelu **Zařízení** zvolte **Žádné** z rozevíracího seznamu \> **Přiřazený profil** **Uložit**.
    
