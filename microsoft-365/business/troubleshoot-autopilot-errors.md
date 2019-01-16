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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="3523c-103">Odstraňování chyb zařízení AutoPilota</span><span class="sxs-lookup"><span data-stu-id="3523c-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="3523c-104">Zařízení souboru chybových zpráv</span><span class="sxs-lookup"><span data-stu-id="3523c-104">Device file error messages</span></span>

<span data-ttu-id="3523c-105">Zde uvádíme informace o některé chyby se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3523c-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="3523c-106">**Kód chyby**</span><span class="sxs-lookup"><span data-stu-id="3523c-106">**Error code**</span></span>|<span data-ttu-id="3523c-107">**Zkuste opravit**</span><span class="sxs-lookup"><span data-stu-id="3523c-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3523c-108">Neplatný požadavek subjektu</span><span class="sxs-lookup"><span data-stu-id="3523c-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="3523c-109">K této chybě dojde jen zřídka, pokud se zobrazí tato chyba, zkuste operaci provést znovu.</span><span class="sxs-lookup"><span data-stu-id="3523c-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="3523c-110">Hodnota hash hardwaru pro zařízení není správný.</span><span class="sxs-lookup"><span data-stu-id="3523c-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="3523c-p101">Pokud se zobrazí tato chyba, znamená to nesprávnou hodnotu, kterou jste zadali v souboru CSV pro hash hardwaru pro jedno zařízení. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správné, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="3523c-p101">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3523c-114">Zařízení přiřazená jiného klienta</span><span class="sxs-lookup"><span data-stu-id="3523c-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="3523c-p102">Pokud se zobrazí tato chyba, znamená to nesprávnou hodnotu, kterou jste zadali v souboru CSV pro sériové číslo nebo kód product key z jednoho nebo více zařízení. Nejprve ověřte, zda byla hodnota zadána správně. Pokud si myslíte, že hodnota je správné, ale tato chyba se stále děje, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="3523c-p102">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3523c-118">Soubor CSV obsahuje neplatné sériové číslo nebo kód product key</span><span class="sxs-lookup"><span data-stu-id="3523c-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="3523c-p103">Pokud se zobrazí tato chyba, znamená to, že zařízení, které jsou tyring registrace již registrovaných jiné organizace. Chcete-li odstranit tento problém, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="3523c-p103">If you see this error it means that the device you are tyring to register is already registered by an other organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3523c-121">Toto zařízení není podporováno pro nastavení pomocí AutoPilot</span><span class="sxs-lookup"><span data-stu-id="3523c-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="3523c-p104">Tato chyba znamená, že zařízení nesplňuje požadavky AutoPilot nasazení. Zařízení musí splňovat tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="3523c-p104">This error means the device does not meet AutoPilot deployment requirements. Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="3523c-124">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="3523c-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="3523c-125">Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.</span><span class="sxs-lookup"><span data-stu-id="3523c-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="3523c-126">Zařízení nebylo nalezeno.</span><span class="sxs-lookup"><span data-stu-id="3523c-126">Device not found</span></span>  <br/> |<span data-ttu-id="3523c-p105">Tato chyba znamená, že jedno nebo více zařízení ve vašem souboru CSV není registrován pro vaši organizaci. Chcete-li odstranit tento problém, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="3523c-p105">This error means that one or more devices in your CSV file is not registered to your organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
