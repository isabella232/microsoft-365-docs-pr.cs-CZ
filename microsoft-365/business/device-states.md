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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Přečtěte si o různých stavech zařízení v seznamu Akce zařízení v domácnosti pro správce v Microsoft 365 Business.
ms.openlocfilehash: cb1e5172a6e2d0bfc5748fe982024ead26e8cd62
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417310"
---
# <a name="device-states"></a><span data-ttu-id="5d070-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="5d070-103">Device states</span></span>

<span data-ttu-id="5d070-104">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="5d070-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="5d070-106">**Stav**</span><span class="sxs-lookup"><span data-stu-id="5d070-106">**Status**</span></span>|<span data-ttu-id="5d070-107">**Popis**</span><span class="sxs-lookup"><span data-stu-id="5d070-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d070-108">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="5d070-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="5d070-109">Zařízení je spravované v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5d070-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="5d070-110">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="5d070-110">Retire pending</span></span>  <br/> |<span data-ttu-id="5d070-111">Microsoft 365 Business se připravuje odebrat ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="5d070-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="5d070-112">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="5d070-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="5d070-113">Microsoft 365 Business právě odebírá ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="5d070-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="5d070-114">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="5d070-114">Retire failed</span></span>  <br/> | <span data-ttu-id="5d070-115">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="5d070-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="5d070-116">Vyřazení zrušeno</span><span class="sxs-lookup"><span data-stu-id="5d070-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="5d070-117">Akce v důchodu byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="5d070-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="5d070-118">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="5d070-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="5d070-119">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="5d070-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="5d070-120">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="5d070-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="5d070-121">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="5d070-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="5d070-122">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="5d070-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="5d070-123">Nemohl jsem obnovit tovární nastavení.</span><span class="sxs-lookup"><span data-stu-id="5d070-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="5d070-124">Vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="5d070-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="5d070-125">Tovární vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="5d070-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="5d070-126">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="5d070-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="5d070-127">Akce čeká na vyřízení (nebo probíhající), ale zařízení se nepřihlásilo se změnami po dobu 30 + dnů.</span><span class="sxs-lookup"><span data-stu-id="5d070-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="5d070-128">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="5d070-128">Delete pending</span></span>  <br/> |<span data-ttu-id="5d070-129">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="5d070-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="5d070-130">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="5d070-130">Discovered</span></span>  <br/> |<span data-ttu-id="5d070-131">Služba Microsoft 365 Business zařízení rozpoznala</span><span class="sxs-lookup"><span data-stu-id="5d070-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
