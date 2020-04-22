---
title: Odstraňování chyb zařízení AutoPilota
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Přečtěte si, jak řešit chyby, které se můžou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business Premium.
ms.openlocfilehash: 0c0742e5bf17c85cedfb421cabfd87c0e2184ba5
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635038"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="ce4ce-103">Odstraňování chyb zařízení AutoPilota</span><span class="sxs-lookup"><span data-stu-id="ce4ce-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="ce4ce-104">Chybové zprávy o souboru zařízení</span><span class="sxs-lookup"><span data-stu-id="ce4ce-104">Device file error messages</span></span>

<span data-ttu-id="ce4ce-105">Tady jsou informace o některých chybách, které se mohou zobrazit při práci se soubory zařízení AutoPilot v Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="ce4ce-106">**Kód chyby**</span><span class="sxs-lookup"><span data-stu-id="ce4ce-106">**Error code**</span></span>|<span data-ttu-id="ce4ce-107">**Oprava vyzkoušet**</span><span class="sxs-lookup"><span data-stu-id="ce4ce-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce4ce-108">Neplatné tělo požadavku</span><span class="sxs-lookup"><span data-stu-id="ce4ce-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="ce4ce-109">K této chybě by mělo dojít zřídka, pokud se zobrazí tato chyba, zkuste operaci znovu.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="ce4ce-110">Hodnota hash hardwaru pro zařízení není správná.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="ce4ce-111">Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro hodnotu hash hardwaru jednoho zařízení, není správná.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="ce4ce-112">Nejprve ověřte, zda byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ce4ce-113">Pokud se domníváte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce4ce-114">Zařízení přiřazené k jinému klientovi</span><span class="sxs-lookup"><span data-stu-id="ce4ce-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="ce4ce-115">Pokud se zobrazí tato chyba, znamená to, že hodnota, kterou jste zadali v souboru CSV pro sériové číslo nebo kód Product Key jednoho nebo více zařízení, není správná.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="ce4ce-116">Nejprve ověřte, zda byla hodnota zadána správně.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ce4ce-117">Pokud se domníváte, že hodnota je správná, ale tato chyba stále probíhá, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce4ce-118">Soubor CSV obsahuje neplatné sériové číslo nebo kód Product Key.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="ce4ce-119">Pokud se zobrazí tato chyba, znamená to, že zařízení, které se pokoušíte zaregistrovat, je již registrováno jinou organizací.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="ce4ce-120">Chcete-li tuto chybu opravit, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce4ce-121">Toto zařízení není podporováno pro nastavení pomocí funkce AutoPilot</span><span class="sxs-lookup"><span data-stu-id="ce4ce-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="ce4ce-122">Tato chyba znamená, že zařízení nesplňuje požadavky na nasazení autopilota.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="ce4ce-123">Zařízení musejí splňovat tyto podmínky:</span><span class="sxs-lookup"><span data-stu-id="ce4ce-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="ce4ce-124">Windows 10 verze 1703 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="ce4ce-125">Nová zařízení, která neprošla systémem Windows ipřím pro dlužně.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="ce4ce-126">Zařízení nebylo nalezeno.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-126">Device not found</span></span>  <br/> |<span data-ttu-id="ce4ce-127">Tato chyba znamená, že jedno nebo více zařízení v souboru CSV není registrováno ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="ce4ce-128">Chcete-li tento problém vyřešit, požádejte o pomoc dodavatele hardwaru.</span><span class="sxs-lookup"><span data-stu-id="ce4ce-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
