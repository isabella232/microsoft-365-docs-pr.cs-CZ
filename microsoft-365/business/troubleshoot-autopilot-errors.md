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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Přečtěte si, jak řešit chyby, které se můžou zobrazit při práci se soubory zařízení AutoPilot v Microsoft u 365 Business.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547465"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Odstraňování chyb zařízení AutoPilota

## <a name="device-file-error-messages"></a>Chybové zprávy o souboru zařízení

Tady jsou informace o některých chybách, které se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoftu 365 Business. 
  
|**Kód chyby**|**Oprava vyzkoušet**|
|:-----|:-----|
|Neplatné tělo požadavku  <br/> |K této chybě by mělo dojít zřídka, pokud se zobrazí tato chyba, zkuste operaci znovu.  <br/> |
|Hodnota hash hardwaru pro zařízení není správná.  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro hodnotu hash hardwaru jednoho zařízení, není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud se domníváte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Zařízení přiřazené k jinému klientovi  <br/> |Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení, není správná. Nejprve ověřte, zda byla hodnota zadána správně. Pokud se domníváte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Soubor CSV obsahuje neplatné sériové číslo nebo kód Product Key.  <br/> |Pokud se zobrazí tato chyba, znamená to, že zařízení, které se pokoušíte zaregistrovat, je již registrováno jinou organizací. Chcete-li tuto chybu opravit, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Toto zařízení není podporováno pro nastavení pomocí funkce AutoPilot  <br/> | Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota. Zařízení musejí splňovat tyto podmínky:  <br/>  Windows 10 verze 1703 nebo novější.  <br/>  Nová zařízení, která neprošla systémem Windows ipřím pro dlužně.  <br/> |
|Zařízení nebylo nalezeno.  <br/> |Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není registrováno ve vaší organizaci. Chcete-li tento problém vyřešit, požádejte o pomoc dodavatele hardwaru.  <br/> |
