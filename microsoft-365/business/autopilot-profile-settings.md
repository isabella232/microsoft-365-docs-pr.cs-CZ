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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profily autopilota vám pomůžou řídit, jak se windows instaluje na uživatelských zařízeních. Profily obsahují výchozí a nepovinná nastavení, jako je přeskočení instalace Cortany.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913372"
---
# <a name="about-autopilot-profile-settings"></a>Informace o nastavení profilu AutoPilota .

## <a name="autopilot-profile-settings"></a>Nastavení profilu AutoPilota

Profily AutoPilota můžete použít k řízení instalace Windows na uživatelských zařízeních. Profily obsahují následující nastavení.
  
 **Výchozí funkce AutoPilota (povinné), které jsou nastavené automaticky:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit registraci Cortany, OneDrivu a OEM  <br/> |Přeskočí instalaci spotřebitelských aplikací, jako je Cortana a osobní OneDrive. Uživatel zařízení si je může nainstalovat později, pokud je na zařízení místním správcem. Registrace původního výrobce se přeskočí, protože zařízení bude spravovat Microsoft 365 Business Premium.  <br/> |
|Přihlašovací prostředí se značkou vaší společnosti  <br/> |Pokud má vaše společnost stránku Přidat značku vaší společnosti na přihlašovací stránku [Microsoftu 365](../admin/setup/customize-sign-in-page.md), uživatel zařízení bude mít toto prostředí při přihlašování.  <br/> |
|Automatická registrace MDM s nakonfigurované účty AAD  <br/> |Identitu uživatele spravuje Azure Active Directory a uživatelé se přihlásí k Windows a Microsoftu 365 pomocí přihlašovacích údajů Microsoftu 365 Business Premium.  <br/> |
   
 **Volitelné nastavení:**
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení je vypnuté)  <br/> |Pokud je tato možnost nastavená na **Hodnotu Za,** uživatel zařízení neuvidí při prvním přihlášení licenční smlouvu pro zařízení a Windows.  <br/> |
|Nepovolit uživateli stát se místním správcem  <br/> |Pokud je tato možnost nastavená na **Hodnotu Na**, uživatel zařízení nebude moct instalovat žádné osobní aplikace, jako je Cortana.<br/> |
