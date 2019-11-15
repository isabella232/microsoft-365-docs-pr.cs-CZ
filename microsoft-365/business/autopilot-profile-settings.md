---
title: Informace o nastavení profilu AutoPilota .
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profily AutoPilot vám pomohou určit, jak bude systém Windows nainstalován na uživatelských zařízeních. Profily obsahují výchozí a volitelná nastavení, jako je vynechání instalace Cortana.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321779"
---
# <a name="about-autopilot-profile-settings"></a>Informace o nastavení profilu AutoPilota .

## <a name="autopilot-profile-settings"></a>Nastavení profilu AutoPilot

Pomocí profilů automatických Opilot můžete řídit způsob instalace systému Windows na uživatelská zařízení. Profily obsahují následující nastavení.
  
 **Automaticky nastaveny výchozí funkce AutoPilot (povinné):**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit Cortana, OneDrive a registraci OEM  <br/> |Přeskočí instalaci zákaznických aplikací, jako je Cortana a Personal OneDrive. Uživatel zařízení je může nainstalovat později, dokud je uživatel místním správcem zařízení. Původní registrace výrobce je přeskočena, protože zařízení bude spravováno společností Microsoft 365 Business.  <br/> |
|Přihlášení ke zkušenostem s firemní značkou  <br/> |Pokud vaše společnost disponuje [značkou vaší společnosti na přihlašovací stránce sady Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), zobrazí se uživateli zařízení při přihlášení tato zkušenost.  <br/> |
|Automatický zápis MDM s konfigurovanými účty AAD.  <br/> |Identita uživatele bude spravována společností Azure Active Directory a uživatelé se budou přihlašovat k systému Windows a sadě Office 365 se svými pověřeními Microsoft 365 Business.  <br/> |
   
 **Volitelná nastavení:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)  <br/> |Je-li tato možnost nastavena na zapnuto, nezobrazí se uživateli zařízení licenční smlouva pro zařízení a systém Windows při prvním **přihlášení**.  <br/> |
|Nepovolit uživateli stát se místním správcem  <br/> |Pokud je tato možnost nastavena na **zapnuto**, nebude uživatel zařízení moci instalovat žádné osobní aplikace, například Cortana.<br/> |
   
