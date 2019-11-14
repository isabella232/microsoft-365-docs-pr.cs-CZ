---
title: Stavy zařízení
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Informace o stavech zařízení v aplikaci Microsoft 365 Business.
ms.openlocfilehash: b55e6a5d538ec28d195225e93797cea27afd2e8b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320202"
---
# <a name="device-states"></a><span data-ttu-id="1a268-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="1a268-103">Device states</span></span>

<span data-ttu-id="1a268-104">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="1a268-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="1a268-106">**Stav**</span><span class="sxs-lookup"><span data-stu-id="1a268-106">**Status**</span></span>|<span data-ttu-id="1a268-107">**Popis**</span><span class="sxs-lookup"><span data-stu-id="1a268-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a268-108">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="1a268-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="1a268-109">Zařízení je spravované v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1a268-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="1a268-110">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="1a268-110">Retire pending</span></span>  <br/> |<span data-ttu-id="1a268-111">Microsoft 365 Business se připravuje odebrat ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="1a268-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1a268-112">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="1a268-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="1a268-113">Microsoft 365 Business právě odebírá ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="1a268-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1a268-114">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="1a268-114">Retire failed</span></span>  <br/> | <span data-ttu-id="1a268-115">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="1a268-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="1a268-116">Zrušení důchodu</span><span class="sxs-lookup"><span data-stu-id="1a268-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="1a268-117">Akce odchodu do důchodu byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="1a268-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="1a268-118">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="1a268-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="1a268-119">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="1a268-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="1a268-120">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="1a268-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="1a268-121">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="1a268-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="1a268-122">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="1a268-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="1a268-123">Tovární resetování nelze.</span><span class="sxs-lookup"><span data-stu-id="1a268-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="1a268-124">Vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="1a268-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="1a268-125">Vymazání výrobního závodu bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="1a268-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="1a268-126">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="1a268-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="1a268-127">Akce čeká na vyřízení (nebo probíhá), ale zařízení se nekontroluje po dobu 30 + dní.</span><span class="sxs-lookup"><span data-stu-id="1a268-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="1a268-128">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="1a268-128">Delete pending</span></span>  <br/> |<span data-ttu-id="1a268-129">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="1a268-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="1a268-130">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="1a268-130">Discovered</span></span>  <br/> |<span data-ttu-id="1a268-131">Služba Microsoft 365 Business zařízení rozpoznala</span><span class="sxs-lookup"><span data-stu-id="1a268-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
