---
title: Zabezpečení zařízení s Windows 10
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Informace o výchozím nastavení a další nastavení zabezpečení zařízení Windows 10. '
ms.openlocfilehash: b56aac0c760aa0e57d48683b5f1726c9add16d20
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074414"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="3d395-103">Zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="3d395-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="3d395-p101">[] Nastavení, která tady nakonfigurujete, jsou součástí výchozí zásady zařízení pro Windows 10. Všichni uživatelé, kteří připojí zařízení s Windows 10 (včetně mobilních zařízení a počítačů) tak, že se na nich přihlásí k pracovnímu účtu, získají tato nastavení automaticky. Doporučujeme vám během instalace přijmou výchozí zásady a další zásady, které budou cílit na konkrétní skupiny uživatelů, přidat později.</span><span class="sxs-lookup"><span data-stu-id="3d395-p101">The settings that you configure here are part of the default device policy for Windows 10. All users that connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account, will automatically receive these settings. We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="3d395-107">Nastavení pro zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="3d395-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="3d395-p102">Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="3d395-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="3d395-110">Nastavení</span><span class="sxs-lookup"><span data-stu-id="3d395-110">Setting</span></span>  <br/> |<span data-ttu-id="3d395-111">Popis</span><span class="sxs-lookup"><span data-stu-id="3d395-111">Description</span></span>  <br/> |
|<span data-ttu-id="3d395-112">Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="3d395-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="3d395-113">Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.</span><span class="sxs-lookup"><span data-stu-id="3d395-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="3d395-114">Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3d395-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="3d395-115">Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.</span><span class="sxs-lookup"><span data-stu-id="3d395-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="3d395-116">Vypnout obrazovku zařízení po nečinnosti</span><span class="sxs-lookup"><span data-stu-id="3d395-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="3d395-p103">Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.</span><span class="sxs-lookup"><span data-stu-id="3d395-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="3d395-120">Povolit uživatelům stahovat aplikace z webu Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="3d395-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="3d395-p104">Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  </span><span class="sxs-lookup"><span data-stu-id="3d395-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="3d395-123">Umožnit uživatelům přístup ke Cortaně</span><span class="sxs-lookup"><span data-stu-id="3d395-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="3d395-p105">Cortana může být velice užitečná. Může vám zapínat nebo vypínat nastavení, dávat vám pokyny a postarat se o to, abyste chodili včas na schůzky. Proto jsme nastavení nechali implicitně **zapnuté**.  </span><span class="sxs-lookup"><span data-stu-id="3d395-p105">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="3d395-126">Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="3d395-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="3d395-127">Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.</span><span class="sxs-lookup"><span data-stu-id="3d395-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="3d395-128">Automaticky aktualizovat zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="3d395-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="3d395-129">Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="3d395-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

