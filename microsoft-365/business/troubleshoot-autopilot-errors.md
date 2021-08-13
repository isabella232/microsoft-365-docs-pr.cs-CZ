---
title: Odstraňování chyb zařízení AutoPilota
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Zjistěte, jak řešit chyby, které se můžou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business Premium.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809174"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Odstraňování chyb zařízení AutoPilota

## <a name="device-file-error-messages"></a>Chybové zprávy o souboru zařízení

Tady jsou informace o některých chybách, které se můžou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business Premium. 
  
|**Kód chyby**|**Oprava pokusu**|
|:-----|:-----|
|Neplatný text žádosti  <br/> |K této chybě by mělo dojít zřídka, pokud se tato chyba zobrazí, zkuste operaci znovu.  <br/> |
|Hardwarová hodnota hash zařízení není správná.  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota zadaná v souboru CSV pro hardwarovou hodnotu hash jednoho zařízení není správná. Nejdřív ověřte, jestli byla hodnota zadána správně. Pokud si myslíte, že je hodnota správná, ale tato chyba se pořád děje, požádejte dodavatele hardwaru o pomoc.  <br/> |
|Zařízení přiřazené jinému tenantovi  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota zadaná v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení není správná. Nejdřív ověřte, jestli byla hodnota zadána správně. Pokud si myslíte, že je hodnota správná, ale tato chyba se pořád děje, požádejte dodavatele hardwaru o pomoc.  <br/> |
|Soubor CSV obsahuje neplatné pořadové číslo nebo kód Product Key.  <br/> |Pokud se tato chyba zobrazí, znamená to, že zařízení, které se pokoušíte zaregistrovat, už je zaregistrované jinou organizací. Pokud chcete tuto chybu vyřešit, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Toto zařízení není pro nastavení podporované pomocí autopilota.  <br/> | Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota. Zařízení musejí splňovat tyto podmínky:  <br/>  Windows 10 verze 1703 nebo novější.  <br/>  Nová zařízení, která ještě Windows prostředí.  <br/> |
|Zařízení nebylo nalezeno.  <br/> |Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není ve vaší organizaci zaregistrované. Pokud to chcete vyřešit, požádejte o pomoc dodavatele hardwaru.  <br/> |
