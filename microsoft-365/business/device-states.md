---
title: Stavy zařízení
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Přečtěte si o různých stavech zařízení v seznamu Akce zařízení v domovské stránce správce v Microsoftu 365 pro firmy.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578461"
---
# <a name="device-states"></a><span data-ttu-id="a5161-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="a5161-103">Device states</span></span>

<span data-ttu-id="a5161-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a5161-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a5161-105">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="a5161-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="a5161-107">**Stav**</span><span class="sxs-lookup"><span data-stu-id="a5161-107">**Status**</span></span>|<span data-ttu-id="a5161-108">**Popis**</span><span class="sxs-lookup"><span data-stu-id="a5161-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5161-109">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="a5161-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="a5161-110">Spravuje Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a5161-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="a5161-111">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="a5161-111">Retire pending</span></span>  <br/> |<span data-ttu-id="a5161-112">Microsoft 365 Business Premium se připravuje na odebrání firemních dat ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="a5161-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a5161-113">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="a5161-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="a5161-114">Microsoft 365 Business Premium momentálně odebírá data společnosti ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="a5161-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="a5161-115">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="a5161-115">Retire failed</span></span>  <br/> | <span data-ttu-id="a5161-116">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="a5161-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="a5161-117">Vyřazení zrušeno</span><span class="sxs-lookup"><span data-stu-id="a5161-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="a5161-118">Akce vyřazení byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="a5161-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="a5161-119">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="a5161-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="a5161-120">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="a5161-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="a5161-121">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="a5161-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="a5161-122">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="a5161-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="a5161-123">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="a5161-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="a5161-124">Obnovení továrního nastavení se nešlo provést.</span><span class="sxs-lookup"><span data-stu-id="a5161-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="a5161-125">Vymazání zrušeno</span><span class="sxs-lookup"><span data-stu-id="a5161-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="a5161-126">Vymazání továrního nastavení bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="a5161-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="a5161-127">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="a5161-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="a5161-128">Akce čeká na vyřízení (nebo probíhá), ale zařízení se neschová už 30+ dní.</span><span class="sxs-lookup"><span data-stu-id="a5161-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="a5161-129">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="a5161-129">Delete pending</span></span>  <br/> |<span data-ttu-id="a5161-130">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="a5161-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="a5161-131">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="a5161-131">Discovered</span></span>  <br/> |<span data-ttu-id="a5161-132">Microsoft 365 Business Premium zařízení zjistil.</span><span class="sxs-lookup"><span data-stu-id="a5161-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
