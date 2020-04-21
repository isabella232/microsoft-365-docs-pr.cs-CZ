---
title: Informace o nastavení profilu AutoPilota .
f1.keywords:
- NOCSH
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
description: Profily autopilota vám pomohou řídit, jak se systém Windows nainstaluje na uživatelská zařízení. Profily obsahují výchozí a volitelná nastavení, jako je přeskočit instalaci Cortany.
ms.openlocfilehash: 5c2ec3f4c3e0ebc4ea545d11f819c897f414ad52
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627408"
---
# <a name="about-autopilot-profile-settings"></a>Informace o nastavení profilu AutoPilota .

## <a name="autopilot-profile-settings"></a>Nastavení profilu autopilota

Pomocí profilů AutoPilot můžete určit, jak je systém Windows nainstalován na uživatelských zařízeních. Profily obsahují následující nastavení.
  
 **Výchozí funkce autopilota (povinné), které jsou nastaveny automaticky:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit registraci Cortany, OneDrivu a OEM  <br/> |Přeskočí instalaci spotřebitelských aplikací, jako je Cortana a osobní OneDrive. Uživatel zařízení můžete nainstalovat později, pokud je uživatel místní správce na zařízení. Původní registrace výrobce je přeskočena, protože zařízení bude spravovat Microsoft 365 Business Premium.  <br/> |
|Přihlaste se se svou firemní značkou  <br/> |Pokud má vaše společnost [značku Přidat firemní značku na přihlašovací stránku Microsoft 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), uživatel zařízení získá toto prostředí při přihlášení.  <br/> |
|Automatický zápis MDM s nakonfigurovanými účty AAD.  <br/> |Identitu uživatele bude spravovat služba Azure Active Directory a uživatelé se přihlásí k Windows a Microsoftu 365 pomocí svých přihlašovacích údajů k Microsoft 365 Business Premium.  <br/> |
   
 **Volitelná nastavení:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)  <br/> |Pokud je tato možnost nastavena **na Zapnuto**, uživatel zařízení neuvidí licenční smlouvu pro zařízení a systém Windows při prvním přihlášení.  <br/> |
|Nedovolte, aby se uživatel stal místním správcem  <br/> |Pokud je tato možnost nastavena **na Zapnuto**, uživatel zařízení nebude moci instalovat žádné osobní aplikace, například Cortanu.<br/> |
   
