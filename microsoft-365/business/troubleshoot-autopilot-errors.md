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
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578081"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="e293e-103">Odstraňování chyb zařízení AutoPilota</span><span class="sxs-lookup"><span data-stu-id="e293e-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="e293e-104">Chybové zprávy o souboru zařízení</span><span class="sxs-lookup"><span data-stu-id="e293e-104">Device file error messages</span></span>

<span data-ttu-id="e293e-105">Tady jsou informace o některých chybách, které se můžou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e293e-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="e293e-106">**Kód chyby**</span><span class="sxs-lookup"><span data-stu-id="e293e-106">**Error code**</span></span>|<span data-ttu-id="e293e-107">**Oprava pokusu**</span><span class="sxs-lookup"><span data-stu-id="e293e-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e293e-108">Neplatný text žádosti</span><span class="sxs-lookup"><span data-stu-id="e293e-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="e293e-109">K této chybě by mělo dojít zřídka, pokud se tato chyba zobrazí, zkuste operaci znovu.</span><span class="sxs-lookup"><span data-stu-id="e293e-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="e293e-110">Hardwarová hodnota hash zařízení není správná.</span><span class="sxs-lookup"><span data-stu-id="e293e-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="e293e-111">Pokud se zobrazí tato chyba, znamená to, že hodnota zadaná v souboru CSV pro hardwarovou hodnotu hash jednoho zařízení není správná.</span><span class="sxs-lookup"><span data-stu-id="e293e-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="e293e-112">Nejdřív ověřte, jestli byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="e293e-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="e293e-113">Pokud si myslíte, že je hodnota správná, ale tato chyba se pořád děje, požádejte dodavatele hardwaru o pomoc.</span><span class="sxs-lookup"><span data-stu-id="e293e-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="e293e-114">Zařízení přiřazené jinému tenantovi</span><span class="sxs-lookup"><span data-stu-id="e293e-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="e293e-115">Pokud se zobrazí tato chyba, znamená to, že hodnota zadaná v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení není správná.</span><span class="sxs-lookup"><span data-stu-id="e293e-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="e293e-116">Nejdřív ověřte, jestli byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="e293e-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="e293e-117">Pokud si myslíte, že je hodnota správná, ale tato chyba se pořád děje, požádejte dodavatele hardwaru o pomoc.</span><span class="sxs-lookup"><span data-stu-id="e293e-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="e293e-118">Soubor CSV obsahuje neplatné pořadové číslo nebo kód Product Key.</span><span class="sxs-lookup"><span data-stu-id="e293e-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="e293e-119">Pokud se tato chyba zobrazí, znamená to, že zařízení, které se pokoušíte zaregistrovat, už je zaregistrované jinou organizací.</span><span class="sxs-lookup"><span data-stu-id="e293e-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="e293e-120">Pokud chcete tuto chybu vyřešit, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="e293e-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="e293e-121">Toto zařízení není pro nastavení podporované pomocí autopilota.</span><span class="sxs-lookup"><span data-stu-id="e293e-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="e293e-122">Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota.</span><span class="sxs-lookup"><span data-stu-id="e293e-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="e293e-123">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="e293e-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="e293e-124">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="e293e-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="e293e-125">Nová zařízení, která ještě nevyužíla prostředí Windows.</span><span class="sxs-lookup"><span data-stu-id="e293e-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="e293e-126">Zařízení nebylo nalezeno.</span><span class="sxs-lookup"><span data-stu-id="e293e-126">Device not found</span></span>  <br/> |<span data-ttu-id="e293e-127">Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není ve vaší organizaci zaregistrované.</span><span class="sxs-lookup"><span data-stu-id="e293e-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="e293e-128">Pokud to chcete vyřešit, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="e293e-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
