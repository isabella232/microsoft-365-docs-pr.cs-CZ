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
description: Profily autopilota vám pomohou řídit způsob instalace systému Windows na uživatelských zařízeních. Profily obsahují výchozí a volitelná nastavení, jako je přeskočení instalace Cortany.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593327"
---
# <a name="about-autopilot-profile-settings"></a>Informace o nastavení profilu AutoPilota .

## <a name="autopilot-profile-settings"></a>Nastavení profilu autopilota

Profily AutoPilot můžete použít k řízení způsobu instalace systému Windows na uživatelských zařízeních. Profily obsahují následující nastavení.
  
 **Výchozí funkce autopilota (povinné), které jsou nastaveny automaticky:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit registraci Cortany, OneDrivu a OEM  <br/> |Přeskočí instalaci spotřebitelských aplikací, jako je Cortana a osobní OneDrive. Uživatel zařízení je může nainstalovat později, pokud je uživatel místním správcem zařízení. Původní registrace výrobce je přeskočena, protože zařízení bude spravováno společností Microsoft 365 Business.  <br/> |
|Přihlaste se ke značce vaší společnosti  <br/> |Pokud má vaše společnost na [přihlašovací stránku Office 365 značku Přidat vaši společnost](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), uživatel zařízení toto prostředí získá při přihlášení.  <br/> |
|Automatický zápis MDM s nakonfigurovanými účty AAD.  <br/> |Identitu uživatele bude spravovat služba Azure Active Directory a uživatelé se k Windows a Office 365 přihlásí pomocí přihlašovacích údajů Microsoft 365 Business.  <br/> |
   
 **Volitelné nastavení:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)  <br/> |Pokud je tato možnost nastavena na **zapnuto**, uživatel zařízení neuvidí licenční smlouvu pro zařízení a systém Windows, když se poprvé přihlásí.  <br/> |
|Nedovolte, aby se uživatel stal místním správcem  <br/> |Pokud je tato možnost nastavena na **Zapnuto**, uživatel zařízení nebude moci nainstalovat žádné osobní aplikace, jako je například Cortana.<br/> |
   
