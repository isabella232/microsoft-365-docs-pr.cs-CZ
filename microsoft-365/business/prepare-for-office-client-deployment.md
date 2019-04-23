---
title: Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Zjistěte, jak na automatickou instalaci aplikací Office 32-bit Windows 10 počítačů a jejich aktualizaci.
ms.openlocfilehash: c8e93746b89925d6b6a928a474fe5736e2834987
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286639"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="ccce6-103">Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="ccce6-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="ccce6-104">Příprava k automatické instalaci aplikací Office na klientské počítače</span><span class="sxs-lookup"><span data-stu-id="ccce6-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="ccce6-105">Microsoft 365 Business můžete použít k instalaci 32bitových aplikací Office na počítače s Windows 10 a k jejich udržování v aktuálním stavu prostřednictvím aktualizací.</span><span class="sxs-lookup"><span data-stu-id="ccce6-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="ccce6-106">Nejlépe to funguje, pokud počítač koncového uživatele používá Windows 10 Business a:</span><span class="sxs-lookup"><span data-stu-id="ccce6-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="ccce6-107">Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).</span><span class="sxs-lookup"><span data-stu-id="ccce6-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="ccce6-108">nebo</span><span class="sxs-lookup"><span data-stu-id="ccce6-108">or</span></span>
    
- <span data-ttu-id="ccce6-109">Má nainstalovanou stávající verzi Office technologií Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ccce6-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="ccce6-p101">Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se zobrazí stejné aktualizace Office jako na následujícím obrázku, byla k instalaci použita technologie Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ccce6-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="ccce6-113">**Pro koho je tato funkce užitečná?**</span><span class="sxs-lookup"><span data-stu-id="ccce6-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="ccce6-114">Koncový uživatel s počítačem, který splňuje následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="ccce6-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="ccce6-115">**Má** uživatelskou licenci k Windows 10 Business, aktivní licenci k Microsoft 365 Business, Windows 10 Creators Update a je připojený k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ccce6-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="ccce6-p102">**Nemá** 64bitové aplikace Office (např. Word, Excel, PowerPoint). Pokud potřebujete 64bitové aplikace Office, není tato funkce vhodná, protože nepodporuje spuštění 64bitové verze Office 2016 technologií Klikni a spusť z konzoly pro správu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ccce6-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="ccce6-p103">**Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 Business upgraduje Office na verzi Office 2016 nainstalovanou technologií Klikni a spusť, která ale nefunguje se samostatnými aplikacemi Office 2016 nainstalovanými instalační službou MSI.</span><span class="sxs-lookup"><span data-stu-id="ccce6-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="ccce6-120">Následující tabulka podrobně popisuje, jakou akci musí koncoví uživatelé / správci provést podle toho, jaký je počáteční stav, aby mohli z konzoly pro správce Microsoft 365 Business úspěšně nasadit 32bitovou verzi Office nainstalovanou technologií Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ccce6-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="ccce6-121">**Počáteční stav instalace Office**</span><span class="sxs-lookup"><span data-stu-id="ccce6-121">**Starting Office install status**</span></span>|<span data-ttu-id="ccce6-122">**Prováděná akce před instalací Microsoft 365 Business Office**</span><span class="sxs-lookup"><span data-stu-id="ccce6-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="ccce6-123">**Konečný stav**</span><span class="sxs-lookup"><span data-stu-id="ccce6-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ccce6-124">Sada Office není nainstalovaná</span><span class="sxs-lookup"><span data-stu-id="ccce6-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="ccce6-125">Žádná</span><span class="sxs-lookup"><span data-stu-id="ccce6-125">None</span></span>  <br/> |<span data-ttu-id="ccce6-126">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="ccce6-127">Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací</span><span class="sxs-lookup"><span data-stu-id="ccce6-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="ccce6-128">Žádná</span><span class="sxs-lookup"><span data-stu-id="ccce6-128">None</span></span>  <br/> |<span data-ttu-id="ccce6-129">Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\***</span><span class="sxs-lookup"><span data-stu-id="ccce6-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="ccce6-130">Stávající 32bitová verze Office nainstalovaná technologií Klikni a spusť a 32bitové nebo 64bitové samostatné aplikace Office (například Visio nebo Project) nainstalované technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="ccce6-131">Žádná</span><span class="sxs-lookup"><span data-stu-id="ccce6-131">None</span></span>  <br/> |<span data-ttu-id="ccce6-p104">Samostatné aplikace se nezmění. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="ccce6-134">Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)</span><span class="sxs-lookup"><span data-stu-id="ccce6-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="ccce6-135">Žádná</span><span class="sxs-lookup"><span data-stu-id="ccce6-135">None</span></span>  <br/> |<span data-ttu-id="ccce6-p105">Samostatné aplikace se nezmění. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="ccce6-138">Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="ccce6-139">Odinstalujte 64bitové aplikace Office, pokud je možné je nahradit 32bitovými aplikacemi Office.</span><span class="sxs-lookup"><span data-stu-id="ccce6-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="ccce6-140">Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ccce6-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="ccce6-141">Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich</span><span class="sxs-lookup"><span data-stu-id="ccce6-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="ccce6-142">Odinstalujte Office 2016 nainstalovaný instalační službou MSI.</span><span class="sxs-lookup"><span data-stu-id="ccce6-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="ccce6-p106">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.</span><span class="sxs-lookup"><span data-stu-id="ccce6-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="ccce6-145">Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office</span><span class="sxs-lookup"><span data-stu-id="ccce6-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="ccce6-146">Žádná</span><span class="sxs-lookup"><span data-stu-id="ccce6-146">None</span></span>  <br/> |<span data-ttu-id="ccce6-147">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe</span><span class="sxs-lookup"><span data-stu-id="ccce6-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="ccce6-p107">**(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Na opravě se pracuje.</span><span class="sxs-lookup"><span data-stu-id="ccce6-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


