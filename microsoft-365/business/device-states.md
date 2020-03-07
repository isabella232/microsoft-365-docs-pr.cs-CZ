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
description: Seznamte se s různými stavy zařízení v seznamu Akce zařízení v domovské stránce Správce v Microsoftu 365 Business.
ms.openlocfilehash: bed1610814ca0d60adb4b4b3d0018e3e7e6d763f
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560814"
---
# <a name="device-states"></a><span data-ttu-id="ed02d-103">Stavy zařízení</span><span class="sxs-lookup"><span data-stu-id="ed02d-103">Device states</span></span>

<span data-ttu-id="ed02d-104">Zařízení v seznamu **Akce zařízení** (domovská stránka správce \> **Akce zařízení**) můžou mít následující stavy.</span><span class="sxs-lookup"><span data-stu-id="ed02d-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="ed02d-106">**Stav**</span><span class="sxs-lookup"><span data-stu-id="ed02d-106">**Status**</span></span>|<span data-ttu-id="ed02d-107">**Popis**</span><span class="sxs-lookup"><span data-stu-id="ed02d-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed02d-108">Spravováno službami Intune</span><span class="sxs-lookup"><span data-stu-id="ed02d-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="ed02d-109">Zařízení je spravované v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ed02d-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="ed02d-110">Čeká se na vyřízení</span><span class="sxs-lookup"><span data-stu-id="ed02d-110">Retire pending</span></span>  <br/> |<span data-ttu-id="ed02d-111">Microsoft 365 Business se připravuje odebrat ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="ed02d-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ed02d-112">Probíhá vyřazování</span><span class="sxs-lookup"><span data-stu-id="ed02d-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="ed02d-113">Microsoft 365 Business právě odebírá ze zařízení data společnosti.</span><span class="sxs-lookup"><span data-stu-id="ed02d-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ed02d-114">Vyřazení selhalo</span><span class="sxs-lookup"><span data-stu-id="ed02d-114">Retire failed</span></span>  <br/> | <span data-ttu-id="ed02d-115">Akce spočívající v odebrání dat společnosti se nezdařila.</span><span class="sxs-lookup"><span data-stu-id="ed02d-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="ed02d-116">Vyřazení bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="ed02d-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="ed02d-117">Akce vyřazení byla zrušena.</span><span class="sxs-lookup"><span data-stu-id="ed02d-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="ed02d-118">Čeká se na vymazání</span><span class="sxs-lookup"><span data-stu-id="ed02d-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="ed02d-119">Čeká se na spuštění obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="ed02d-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="ed02d-120">Probíhá mazání</span><span class="sxs-lookup"><span data-stu-id="ed02d-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="ed02d-121">Byl vydán příkaz k obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="ed02d-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="ed02d-122">Vymazání selhalo</span><span class="sxs-lookup"><span data-stu-id="ed02d-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="ed02d-123">Nelze provést obnovení továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="ed02d-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="ed02d-124">Vymazání zrušeno</span><span class="sxs-lookup"><span data-stu-id="ed02d-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="ed02d-125">Tovární vymazání bylo zrušeno.</span><span class="sxs-lookup"><span data-stu-id="ed02d-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="ed02d-126">Není v pořádku</span><span class="sxs-lookup"><span data-stu-id="ed02d-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="ed02d-127">Akce čeká na vyřízení (nebo probíhá), ale zařízení se nepřihlásilo více než 30 dní.</span><span class="sxs-lookup"><span data-stu-id="ed02d-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="ed02d-128">Čeká se na odstranění</span><span class="sxs-lookup"><span data-stu-id="ed02d-128">Delete pending</span></span>  <br/> |<span data-ttu-id="ed02d-129">Čeká se na provedení akce odstranění.</span><span class="sxs-lookup"><span data-stu-id="ed02d-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="ed02d-130">Zjištěné</span><span class="sxs-lookup"><span data-stu-id="ed02d-130">Discovered</span></span>  <br/> |<span data-ttu-id="ed02d-131">Služba Microsoft 365 Business zařízení rozpoznala</span><span class="sxs-lookup"><span data-stu-id="ed02d-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
