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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="f2d5f-103">Odstraňování chyb zařízení AutoPilota</span><span class="sxs-lookup"><span data-stu-id="f2d5f-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="f2d5f-104">Chybové zprávy souboru zařízení</span><span class="sxs-lookup"><span data-stu-id="f2d5f-104">Device file error messages</span></span>

<span data-ttu-id="f2d5f-105">Zde jsou informace o některých chybách, které se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="f2d5f-106">**Kód chyby**</span><span class="sxs-lookup"><span data-stu-id="f2d5f-106">**Error code**</span></span>|<span data-ttu-id="f2d5f-107">**Oprava vyzkoušet**</span><span class="sxs-lookup"><span data-stu-id="f2d5f-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2d5f-108">Neplatný text požadavku</span><span class="sxs-lookup"><span data-stu-id="f2d5f-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="f2d5f-109">K této chybě by mělo dojít zřídka, pokud se zobrazí tato chyba, zkuste operaci znovu.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="f2d5f-110">Hodnota hash hardwaru pro zařízení není správná.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="f2d5f-111">Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro hardwarovou hodnotu hash jednoho zařízení, není správná.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="f2d5f-112">Nejprve ověřte, zda byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="f2d5f-113">Pokud si myslíte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="f2d5f-114">Zařízení přiřazené jinému klientovi</span><span class="sxs-lookup"><span data-stu-id="f2d5f-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="f2d5f-115">Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení, není správná.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="f2d5f-116">Nejprve ověřte, zda byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="f2d5f-117">Pokud si myslíte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="f2d5f-118">Soubor CSV obsahuje neplatné sériové číslo nebo kód Product Key.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="f2d5f-119">Pokud se zobrazí tato chyba, znamená to, že zařízení, které se pokoušíte zaregistrovat, je již registrováno jinou organizací.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="f2d5f-120">Chcete-li tuto chybu vyřešit, požádejte dodavatele hardwaru o pomoc.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="f2d5f-121">Toto zařízení není podporováno pro instalaci pomocí funkce AutoPilot</span><span class="sxs-lookup"><span data-stu-id="f2d5f-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="f2d5f-122">Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="f2d5f-123">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="f2d5f-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="f2d5f-124">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="f2d5f-125">Nová zařízení, která neprošla systémem Windows, jsou v pořádku.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="f2d5f-126">Zařízení nebylo nalezeno.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-126">Device not found</span></span>  <br/> |<span data-ttu-id="f2d5f-127">Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není registrováno ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="f2d5f-128">Chcete-li tento problém vyřešit, požádejte dodavatele hardwaru o pomoc.</span><span class="sxs-lookup"><span data-stu-id="f2d5f-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
