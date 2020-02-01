---
title: Odstraňování chyb zařízení AutoPilota
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Přečtěte si, jak řešit problémy s chybami souborů zařízení AutoPilot.
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594202"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Odstraňování chyb zařízení AutoPilota

## <a name="device-file-error-messages"></a>Chybové zprávy souboru zařízení

Zde jsou informace o některých chybách, které se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business. 
  
|**Kód chyby**|**Oprava vyzkoušet**|
|:-----|:-----|
|Neplatný text požadavku  <br/> |K této chybě by mělo dojít zřídka, pokud se zobrazí tato chyba, zkuste operaci znovu.  <br/> |
|Hodnota hash hardwaru pro zařízení není správná.  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro hardwarovou hodnotu hash jednoho zařízení, není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Zařízení přiřazené jinému klientovi  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení, není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Soubor CSV obsahuje neplatné sériové číslo nebo kód Product Key.  <br/> |Pokud se zobrazí tato chyba, znamená to, že zařízení, které se pokoušíte zaregistrovat, je již registrováno jinou organizací. Chcete-li tuto chybu vyřešit, požádejte dodavatele hardwaru o pomoc.  <br/> |
|Toto zařízení není podporováno pro instalaci pomocí funkce AutoPilot  <br/> | Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota. Zařízení musejí splňovat tyto podmínky:  <br/>  Windows 10 verze 1703 nebo novější.  <br/>  Nová zařízení, která neprošla systémem Windows, jsou v pořádku.  <br/> |
|Zařízení nebylo nalezeno.  <br/> |Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není registrováno ve vaší organizaci. Chcete-li tento problém vyřešit, požádejte dodavatele hardwaru o pomoc.  <br/> |
