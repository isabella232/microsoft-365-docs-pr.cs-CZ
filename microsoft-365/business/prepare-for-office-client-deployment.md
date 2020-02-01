---
title: Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Přečtěte si, jak automaticky nainstalovat 32bitové aplikace Office do počítačů s Windows 10 a aktualizovat je.
ms.openlocfilehash: fa5b2ce1852ebdb1e76c1fa844793fee56af3d68
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593613"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="f48f5-103">Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="f48f5-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="f48f5-104">Příprava k automatické instalaci aplikací Office na klientské počítače</span><span class="sxs-lookup"><span data-stu-id="f48f5-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="f48f5-105">Pomocí Microsoftu 365 Business můžete automaticky nainstalovat 32bitové aplikace Office do počítačů s Windows 10 a udržovat je aktuální s aktualizacemi.</span><span class="sxs-lookup"><span data-stu-id="f48f5-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="f48f5-106">Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele v systému Windows 10 Business a:</span><span class="sxs-lookup"><span data-stu-id="f48f5-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="f48f5-107">Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).</span><span class="sxs-lookup"><span data-stu-id="f48f5-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="f48f5-108">nebo</span><span class="sxs-lookup"><span data-stu-id="f48f5-108">or</span></span>
    
- <span data-ttu-id="f48f5-109">Má nainstalovanou stávající verzi Office technologií Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="f48f5-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="f48f5-110">Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**).</span><span class="sxs-lookup"><span data-stu-id="f48f5-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="f48f5-111">Pokud se zobrazí **aktualizace Office,** jak je znázorněno na následujícím obrázku, instalace byla provedena pomocí funkce Klikněte na spouštění.</span><span class="sxs-lookup"><span data-stu-id="f48f5-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="f48f5-113">**Kdo má prospěch z této funkce**</span><span class="sxs-lookup"><span data-stu-id="f48f5-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="f48f5-114">Koncový uživatel s počítačem, který splňuje následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="f48f5-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="f48f5-115">**Má** uživatelskou licenci k Windows 10 Business, aktivní licenci k Microsoft 365 Business, Windows 10 Creators Update a je připojený k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f48f5-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="f48f5-116">**Nemá** 64bitové aplikace Office (například Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="f48f5-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="f48f5-117">Pokud jsou vyžadovány 64bitové aplikace Office, pak se tato funkce nehodí, protože neexistuje žádná podpora pro spuštění 64bitové verze Office pro kliky a spuštění z konzoly pro správu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f48f5-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="f48f5-118">**Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project.</span><span class="sxs-lookup"><span data-stu-id="f48f5-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="f48f5-119">Microsoft 365 Business upgraduje Office na verzi Pro klika a běh Office 2016 a to nefunguje se samostatnými aplikacemi Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="f48f5-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="f48f5-120">V následující tabulce je uvedeno, jakou akci mohou koncoví uživatelé/správci v závislosti na počátečním stavu provést, aby mohli mít úspěšnou 32bitovou verzi nasazení Office pro spuštění z konzoly pro správu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f48f5-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="f48f5-121">**Počáteční stav instalace Office**</span><span class="sxs-lookup"><span data-stu-id="f48f5-121">**Starting Office install status**</span></span>|<span data-ttu-id="f48f5-122">**Prováděná akce před instalací Microsoft 365 Business Office**</span><span class="sxs-lookup"><span data-stu-id="f48f5-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="f48f5-123">**Konečný stav**</span><span class="sxs-lookup"><span data-stu-id="f48f5-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f48f5-124">Sada Office není nainstalovaná</span><span class="sxs-lookup"><span data-stu-id="f48f5-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="f48f5-125">Žádné</span><span class="sxs-lookup"><span data-stu-id="f48f5-125">None</span></span>  <br/> |<span data-ttu-id="f48f5-126">Office 2016 32bitový je nainstalován pomocí funkce Klikni na spouštění</span><span class="sxs-lookup"><span data-stu-id="f48f5-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="f48f5-127">Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací</span><span class="sxs-lookup"><span data-stu-id="f48f5-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="f48f5-128">Žádné</span><span class="sxs-lookup"><span data-stu-id="f48f5-128">None</span></span>  <br/> |<span data-ttu-id="f48f5-129">Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\***</span><span class="sxs-lookup"><span data-stu-id="f48f5-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="f48f5-130">Existující 32bitová verze Office pro spouštění kliknutím a 32bitové nebo 64bitové samostatné aplikace Office spusťte kliknutím a spusťte 32bitové nebo 64bitové (například Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="f48f5-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="f48f5-131">Žádné</span><span class="sxs-lookup"><span data-stu-id="f48f5-131">None</span></span>  <br/> |<span data-ttu-id="f48f5-132">Samostatné aplikace nejsou ovlivněny.</span><span class="sxs-lookup"><span data-stu-id="f48f5-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="f48f5-133">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="f48f5-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="f48f5-134">Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)</span><span class="sxs-lookup"><span data-stu-id="f48f5-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="f48f5-135">Žádné</span><span class="sxs-lookup"><span data-stu-id="f48f5-135">None</span></span>  <br/> |<span data-ttu-id="f48f5-136">Samostatné aplikace nejsou ovlivněny.</span><span class="sxs-lookup"><span data-stu-id="f48f5-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="f48f5-137">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="f48f5-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="f48f5-138">Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="f48f5-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="f48f5-139">Odinstalujte 64bitové aplikace Office, pokud je v pořádku je nahradit 32bitovými aplikacemi Office</span><span class="sxs-lookup"><span data-stu-id="f48f5-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="f48f5-140">Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="f48f5-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="f48f5-141">Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich</span><span class="sxs-lookup"><span data-stu-id="f48f5-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="f48f5-142">Odinstalujte Office 2016 nainstalovaný instalační službou MSI.</span><span class="sxs-lookup"><span data-stu-id="f48f5-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="f48f5-p106">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.</span><span class="sxs-lookup"><span data-stu-id="f48f5-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="f48f5-145">Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office</span><span class="sxs-lookup"><span data-stu-id="f48f5-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="f48f5-146">Žádná</span><span class="sxs-lookup"><span data-stu-id="f48f5-146">None</span></span>  <br/> |<span data-ttu-id="f48f5-147">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe</span><span class="sxs-lookup"><span data-stu-id="f48f5-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="f48f5-148">**(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="f48f5-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="f48f5-149">Probíhá oprava.</span><span class="sxs-lookup"><span data-stu-id="f48f5-149">A fix is in progress.</span></span> 
  