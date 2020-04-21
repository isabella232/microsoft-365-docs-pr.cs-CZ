---
title: Stavy zařízení
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Seznamte se s různými stavy zařízení v seznamu Akce zařízení v domovské stránce Správce v Microsoftu 365 pro firmy.
ms.openlocfilehash: 1a66e76dd3a74428923292427b01551db2449e48
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627240"
---
# <a name="device-states"></a><span data-ttu-id="f9361-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="f9361-103">Device states</span></span>

<span data-ttu-id="f9361-104">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="f9361-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="f9361-106">**Stav**</span><span class="sxs-lookup"><span data-stu-id="f9361-106">**Status**</span></span>|<span data-ttu-id="f9361-107">**Popis**</span><span class="sxs-lookup"><span data-stu-id="f9361-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9361-108">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="f9361-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="f9361-109">Spravuje Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f9361-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="f9361-110">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="f9361-110">Retire pending</span></span>  <br/> |<span data-ttu-id="f9361-111">Microsoft 365 Business Premium se chystá odebrat firemní data ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="f9361-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f9361-112">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="f9361-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="f9361-113">Microsoft 365 Business Premium v současné době odebírá firemní data ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="f9361-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f9361-114">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="f9361-114">Retire failed</span></span>  <br/> | <span data-ttu-id="f9361-115">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="f9361-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="f9361-116">Vyřazení bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="f9361-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="f9361-117">Akce vyřazení byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="f9361-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="f9361-118">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="f9361-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="f9361-119">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="f9361-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="f9361-120">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="f9361-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="f9361-121">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="f9361-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="f9361-122">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="f9361-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="f9361-123">Nelze provést obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="f9361-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="f9361-124">Vymazání zrušeno</span><span class="sxs-lookup"><span data-stu-id="f9361-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="f9361-125">Tovární vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="f9361-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="f9361-126">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="f9361-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="f9361-127">Akce čeká na vyřízení (nebo probíhá), ale zařízení se nepřihlásilo více než 30 dní.</span><span class="sxs-lookup"><span data-stu-id="f9361-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="f9361-128">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="f9361-128">Delete pending</span></span>  <br/> |<span data-ttu-id="f9361-129">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="f9361-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="f9361-130">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="f9361-130">Discovered</span></span>  <br/> |<span data-ttu-id="f9361-131">Microsoft 365 Business Premium zjistil zařízení.</span><span class="sxs-lookup"><span data-stu-id="f9361-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
