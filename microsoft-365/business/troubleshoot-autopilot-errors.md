---
title: Odstraňování chyb zařízení AutoPilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Informace o odstraňování chyb souboru zařízení AutoPilot.
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982741"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Odstraňování chyb zařízení AutoPilota

## <a name="device-file-error-messages"></a>Zařízení souboru chybových zpráv

Zde uvádíme informace o některé chyby se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business. 
  
|**Kód chyby**|**Zkuste opravit**|
|:-----|:-----|
|Neplatný požadavek subjektu  <br/> |K této chybě dojde jen zřídka, pokud se zobrazí tato chyba, zkuste operaci provést znovu.  <br/> |
|Hodnota hash hardwaru pro zařízení není správný.  <br/> |Pokud se zobrazí tato chyba, znamená to nesprávnou hodnotu, kterou jste zadali v souboru CSV pro hash hardwaru pro jedno zařízení. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správné, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Zařízení přiřazená jiného klienta  <br/> |Pokud se zobrazí tato chyba, znamená to nesprávnou hodnotu, kterou jste zadali v souboru CSV pro sériové číslo nebo kód product key z jednoho nebo více zařízení. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správné, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Soubor CSV obsahuje neplatné sériové číslo nebo kód product key  <br/> |Pokud se zobrazí tato chyba, znamená to, že zařízení, které jsou tyring registrace již registrovaných jiné organizace. Chcete-li odstranit tento problém, požádejte o pomoc dodavatele hardwaru.  <br/> |
|Toto zařízení není podporováno pro nastavení pomocí AutoPilot  <br/> | Tato chyba znamená, že zařízení nesplňuje požadavky AutoPilot nasazení. Zařízení musí splňovat tyto požadavky:  <br/>  Windows 10 verze 1703 nebo novější.  <br/>  Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.  <br/> |
|Zařízení nebylo nalezeno.  <br/> |Tato chyba znamená, že jedno nebo více zařízení ve vašem souboru CSV není registrován pro vaši organizaci. Chcete-li odstranit tento problém, požádejte o pomoc dodavatele hardwaru.  <br/> |
   
