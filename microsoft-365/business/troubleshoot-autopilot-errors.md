---
title: Odstraňování chyb zařízení AutoPilota
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
description: Dozvíte se, jak odstraňovat chyby v souborech zařízení AutoPilot.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718693"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Odstraňování chyb zařízení AutoPilota

## <a name="device-file-error-messages"></a>Chybové zprávy souboru zařízení

Zde jsou informace o některých chybách, které se mohou zobrazit při práci se soubory zařízení AutoPilot v aplikaci Microsoft 365 Business. 
  
|**Kód chyby**|**Oprava vyzkoušet**|
|:-----|:-----|
|Neplatný text požadavku  <br/> |Tato chyba by se měla dít zřídka, pokud se zobrazí tato chyba, zkuste operaci zopakovat.  <br/> |
|Hardwarová hodnota hash pro zařízení není správná.  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste v souboru CSV poskytli pro hardwarovou hodnotu hash jednoho zařízení, není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud se domníváte, že je hodnota správná, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Zařízení přiřazené jinému nájemci  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota poskytnutá v souboru CSV buď pro sériové číslo, nebo pro kód Product Key jednoho nebo více zařízení není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud se domníváte, že je hodnota správná, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Soubor CSV obsahuje neplatné sériové číslo nebo kód Product Key.  <br/> |Pokud se zobrazí tato chyba, znamená to, že zařízení, které se pokoušíte zaregistrovat, je již registrováno jinou organizací. Chcete-li tuto chybu opravit, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Toto zařízení není podporováno pro instalaci pomocí automatického Opilot.  <br/> | Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení AutoPilot. Zařízení musejí splňovat tyto podmínky:  <br/>  Windows 10 verze 1703 nebo novější.  <br/>  Nová zařízení, která nebyla součástí systému Windows.  <br/> |
|Zařízení nebylo nalezeno.  <br/> |Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není registrováno ve vaší organizaci. Chcete-li tento problém vyřešit, požádejte o pomoc dodavatele hardwaru.  <br/> |
