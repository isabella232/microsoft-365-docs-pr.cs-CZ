---
title: Zabezpečení zařízení s Windows 10
f1.keywords:
- CSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Přečtěte si o konfiguraci nastavení výchozích zásad zařízení, která každé zařízení s Windows 10 obdrží po přihlášení ke svému pracovnímu nebo školnímu účtu.
ms.openlocfilehash: 03ae86861ddb0cb83cd39b7834f19e01bf3e99e2
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470621"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="8d1a2-103">Zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="8d1a2-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="8d1a2-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="8d1a2-105">[] Nastavení, která tady nakonfigurujete, jsou součástí výchozí zásady zařízení pro Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="8d1a2-106">Všechna uživatelé, kteří se přihlásí pomocí svého pracovního účtu, se přihlásí pomocí svého pracovního účtu, včetně mobilních zařízení a počítačů.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="8d1a2-107">Doporučujeme vám během instalace přijmou výchozí zásady a další zásady, které budou cílit na konkrétní skupiny uživatelů, přidat později.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="8d1a2-108">Nastavení pro zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="8d1a2-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="8d1a2-p102">Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="8d1a2-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="8d1a2-111">Nastavení</span><span class="sxs-lookup"><span data-stu-id="8d1a2-111">Setting</span></span>  <br/> |<span data-ttu-id="8d1a2-112">Popis</span><span class="sxs-lookup"><span data-stu-id="8d1a2-112">Description</span></span>  <br/> |
|<span data-ttu-id="8d1a2-113">Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="8d1a2-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="8d1a2-114">Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="8d1a2-115">Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8d1a2-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="8d1a2-116">Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="8d1a2-117">Vypnout obrazovku zařízení po nečinnosti</span><span class="sxs-lookup"><span data-stu-id="8d1a2-117">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="8d1a2-p103">Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="8d1a2-121">Povolit uživatelům stahovat aplikace z webu Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="8d1a2-121">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="8d1a2-p104">Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  </span><span class="sxs-lookup"><span data-stu-id="8d1a2-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="8d1a2-124">Umožnit uživatelům přístup ke Cortaně</span><span class="sxs-lookup"><span data-stu-id="8d1a2-124">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="8d1a2-125">Cortana může být velmi užitečná!</span><span class="sxs-lookup"><span data-stu-id="8d1a2-125">Cortana can be very helpful!</span></span> <span data-ttu-id="8d1a2-126">Cortana může zapíná nebo vypíná nastavení, dávat pokyny a ujistit se, že jste na schůzky včas, takže toto **nastavení** ve výchozím nastavení zapínáme.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-126">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="8d1a2-127">Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="8d1a2-127">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="8d1a2-128">Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-128">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="8d1a2-129">Automaticky aktualizovat zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="8d1a2-129">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="8d1a2-130">Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="8d1a2-130">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

