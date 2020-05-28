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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Seznamte se s různými stavy zařízení v seznamu Akce zařízení v domovské stránce Správce v Microsoftu 365 pro firmy.
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400948"
---
# <a name="device-states"></a><span data-ttu-id="dfc17-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="dfc17-103">Device states</span></span>

<span data-ttu-id="dfc17-104">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="dfc17-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="dfc17-106">**Stav**</span><span class="sxs-lookup"><span data-stu-id="dfc17-106">**Status**</span></span>|<span data-ttu-id="dfc17-107">**Popis**</span><span class="sxs-lookup"><span data-stu-id="dfc17-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dfc17-108">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="dfc17-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="dfc17-109">Spravuje Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="dfc17-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="dfc17-110">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="dfc17-110">Retire pending</span></span>  <br/> |<span data-ttu-id="dfc17-111">Microsoft 365 Business Premium se chystá odebrat firemní data ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="dfc17-112">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="dfc17-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="dfc17-113">Microsoft 365 Business Premium v současné době odebírá firemní data ze zařízení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="dfc17-114">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="dfc17-114">Retire failed</span></span>  <br/> | <span data-ttu-id="dfc17-115">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="dfc17-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="dfc17-116">Vyřazení bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="dfc17-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="dfc17-117">Akce vyřazení byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="dfc17-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="dfc17-118">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="dfc17-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="dfc17-119">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="dfc17-120">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="dfc17-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="dfc17-121">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="dfc17-122">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="dfc17-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="dfc17-123">Nelze provést obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="dfc17-124">Vymazání zrušeno</span><span class="sxs-lookup"><span data-stu-id="dfc17-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="dfc17-125">Tovární vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="dfc17-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="dfc17-126">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="dfc17-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="dfc17-127">Akce čeká na vyřízení (nebo probíhá), ale zařízení se nepřihlásilo více než 30 dní.</span><span class="sxs-lookup"><span data-stu-id="dfc17-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="dfc17-128">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="dfc17-128">Delete pending</span></span>  <br/> |<span data-ttu-id="dfc17-129">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="dfc17-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="dfc17-130">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="dfc17-130">Discovered</span></span>  <br/> |<span data-ttu-id="dfc17-131">Microsoft 365 Business Premium zjistil zařízení.</span><span class="sxs-lookup"><span data-stu-id="dfc17-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
