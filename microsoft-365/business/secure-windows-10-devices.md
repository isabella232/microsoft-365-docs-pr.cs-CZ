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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Informace o výchozích a dalších nastaveních pro zabezpečení zařízení systému Windows 10. '
ms.openlocfilehash: 64f20433d5a4b78fc234a4ec3bec937ec30145c6
ms.sourcegitcommit: 0ad0092d9c5cb2d69fc70c990a9b7cc03140611b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/19/2019
ms.locfileid: "40805637"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="4902c-103">Zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4902c-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="4902c-104">[] Nastavení, která tady nakonfigurujete, jsou součástí výchozí zásady zařízení pro Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4902c-104">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="4902c-105">Toto nastavení budou automaticky přijímat všichni uživatelé, kteří připojují zařízení Windows 10, včetně mobilních zařízení a počítačů, přihlášením pomocí svého pracovního účtu.</span><span class="sxs-lookup"><span data-stu-id="4902c-105">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="4902c-106">Doporučujeme vám během instalace přijmou výchozí zásady a další zásady, které budou cílit na konkrétní skupiny uživatelů, přidat později.</span><span class="sxs-lookup"><span data-stu-id="4902c-106">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="4902c-107">Nastavení pro zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4902c-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="4902c-p102">Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="4902c-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="4902c-110">Nastavení</span><span class="sxs-lookup"><span data-stu-id="4902c-110">Setting</span></span>  <br/> |<span data-ttu-id="4902c-111">Popis</span><span class="sxs-lookup"><span data-stu-id="4902c-111">Description</span></span>  <br/> |
|<span data-ttu-id="4902c-112">Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="4902c-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="4902c-113">Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.</span><span class="sxs-lookup"><span data-stu-id="4902c-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="4902c-114">Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4902c-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="4902c-115">Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.</span><span class="sxs-lookup"><span data-stu-id="4902c-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="4902c-116">Vypnout obrazovku zařízení po nečinnosti</span><span class="sxs-lookup"><span data-stu-id="4902c-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="4902c-p103">Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.</span><span class="sxs-lookup"><span data-stu-id="4902c-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="4902c-120">Povolit uživatelům stahovat aplikace z webu Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="4902c-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="4902c-p104">Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  </span><span class="sxs-lookup"><span data-stu-id="4902c-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="4902c-123">Umožnit uživatelům přístup ke Cortaně</span><span class="sxs-lookup"><span data-stu-id="4902c-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="4902c-124">Cortana může být velmi užitečný!</span><span class="sxs-lookup"><span data-stu-id="4902c-124">Cortana can be very helpful!</span></span> <span data-ttu-id="4902c-125">Cortana může zapnout nebo vypnout nastavení, poskytnout pokyny a ujistit se, že máte čas na schůzky, takže toto nastavení ponechejte ve výchozím nastavení **zapnuto** .</span><span class="sxs-lookup"><span data-stu-id="4902c-125">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="4902c-126">Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="4902c-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="4902c-127">Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.</span><span class="sxs-lookup"><span data-stu-id="4902c-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="4902c-128">Automaticky aktualizovat zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4902c-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="4902c-129">Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="4902c-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

