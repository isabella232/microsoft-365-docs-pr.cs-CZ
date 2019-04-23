---
title: Informace o nastavení profilu AutoPilota .
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profily umožňují určit, jak získá uživatel zařízení nainstalován systém Windows. Profily obsahují výchozí a volitelné nastavení, například Přeskočit instalaci Cortana.
ms.openlocfilehash: d43a15e5f3dc83596b5c23dd0ceb416b24810298
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276935"
---
# <a name="about-autopilot-profile-settings"></a>Informace o nastavení profilu AutoPilota .

## <a name="autopilot-profile-settings"></a>Nastavení profilu autoPilot

Můžete určit, jak získá systém Windows nainstalován na zařízení uživatele pomocí profilů AutoPilot. Profily obsahují následující nastavení.
  
 **AutoPilot výchozí funkce (povinné), které jsou automaticky nastaveny:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Vynechají registraci Cortana, OneDrive a OEM  <br/> |Přeskočí instalace aplikace spotřebitele jako Cortana a osobní OneDrive. Tak dlouho, dokud je místní správce zařízení, můžete nainstalovat tyto novější zařízení uživatele. Původní registrace výrobce je vynechán, protože zařízení bude spravovat Microsoft 365 Business.  <br/> |
|Přihlaste se zkušeností s vaší obchodní značky společnosti  <br/> |Pokud má vaše společnost [Přidat vaše společnost vlastní Office 365 přihlašovací stránku](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), dostane zařízení uživatele těchto zkušeností při přihlášení.  <br/> |
|MDM automatického zápisu s účty nakonfigurované zvukové poplašné zařízení.  <br/> |Identita uživatele budou spravovány službou Azure Active directory a uživatelé přihlášení do systému Windows a sady Office 365 pomocí svých pověření Microsoft 365 Business.  <br/> |
   
 **Volitelné nastavení:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)  <br/> |Pokud tato možnost nastavena na hodnotu **On**, zařízení uživatele při mu nejprve nezobrazí licenční smlouvy pro zařízení a Windows.  <br/> |
|Nepovolit uživateli jako místní správce  <br/> |Pokud tato možnost nastavena na hodnotu **On**, nebude moci instalovat jakékoli osobní apps, například Cortana zařízení uživatele.  <br/> |
   
