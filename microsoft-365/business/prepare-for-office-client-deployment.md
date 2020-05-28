---
title: Příprava na nasazení klienta Office microsoftem 365 pro firmy
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Přečtěte si, jak automaticky nainstalovat 32bitové aplikace Office do počítačů s Windows 10 a jak je aktualizovat.
ms.openlocfilehash: 6f3a80be9729a3818607c0f42e2cc7ece66a07ee
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401316"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="ecfca-103">Příprava na nasazení klienta Office microsoftem 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="ecfca-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="ecfca-104">Příprava k automatické instalaci aplikací Office na klientské počítače</span><span class="sxs-lookup"><span data-stu-id="ecfca-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="ecfca-105">Pomocí Microsoftu 365 pro firmy můžete automaticky instalovat 32bitové aplikace Office do počítačů s Windows 10 a udržovat je aktuální pomocí aktualizací.</span><span class="sxs-lookup"><span data-stu-id="ecfca-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="ecfca-106">Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele v systému Windows 10 Business a:</span><span class="sxs-lookup"><span data-stu-id="ecfca-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="ecfca-107">Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).</span><span class="sxs-lookup"><span data-stu-id="ecfca-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="ecfca-108">nebo</span><span class="sxs-lookup"><span data-stu-id="ecfca-108">or</span></span>
    
- <span data-ttu-id="ecfca-109">Má nainstalovanou stávající verzi Office technologií Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ecfca-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="ecfca-110">Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**).</span><span class="sxs-lookup"><span data-stu-id="ecfca-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="ecfca-111">Pokud se aktualizace **Office** zobrazují tak, jak je znázorněno na následujícím obrázku, instalace byla provedena pomocí technologie Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ecfca-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="ecfca-113">**Kdo má prospěch z této funkce**</span><span class="sxs-lookup"><span data-stu-id="ecfca-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="ecfca-114">Koncový uživatel s počítačem, který splňuje následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="ecfca-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="ecfca-115">**Má** uživatelskou licenci pro Windows 10 Business, aktivní licenci Microsoft 365 pro firmy, aktualizaci Windows 10 Creators Update a je připojená k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ecfca-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="ecfca-116">**Nemá** 64bitové aplikace Office (například Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="ecfca-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="ecfca-117">Pokud jsou vyžadovány 64bitové aplikace Office, pak se tato funkce nehodí, protože neexistuje žádná podpora pro spuštění 64bitové verze Office s funkcí Klikni a spusť z konzoly microsoftu 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="ecfca-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="ecfca-118">**Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project.</span><span class="sxs-lookup"><span data-stu-id="ecfca-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="ecfca-119">Microsoft 365 pro firmy upgraduje Office na verzi Office 2016 s klikem a spouštěním, která nefunguje se samostatnými aplikacemi MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="ecfca-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="ecfca-120">V následující tabulce je uvedeno, jakou akci mohou koncoví uživatelé nebo správci v závislosti na počátečním stavu provést, aby měli úspěšnou 32bitovou verzi office s pouštěním z konzole pro správu Microsoftu 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="ecfca-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="ecfca-121">**Počáteční stav instalace Office**</span><span class="sxs-lookup"><span data-stu-id="ecfca-121">**Starting Office install status**</span></span>|<span data-ttu-id="ecfca-122">**Akce, která má být dokončena před instalací Microsoftu 365 pro firmy, instalace Office**</span><span class="sxs-lookup"><span data-stu-id="ecfca-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="ecfca-123">**Konečný stav**</span><span class="sxs-lookup"><span data-stu-id="ecfca-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ecfca-124">Sada Office není nainstalovaná</span><span class="sxs-lookup"><span data-stu-id="ecfca-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="ecfca-125">Žádné</span><span class="sxs-lookup"><span data-stu-id="ecfca-125">None</span></span>  <br/> |<span data-ttu-id="ecfca-126">32bitový Office 2016 je nainstalovaný pomocí technologie Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ecfca-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="ecfca-127">Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací</span><span class="sxs-lookup"><span data-stu-id="ecfca-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="ecfca-128">Žádné</span><span class="sxs-lookup"><span data-stu-id="ecfca-128">None</span></span>  <br/> |<span data-ttu-id="ecfca-129">Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\***</span><span class="sxs-lookup"><span data-stu-id="ecfca-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="ecfca-130">Existující 32bitová verze 32bitových nebo 64bitových samostatných aplikací Office s 32bitovým nebo 64bitovým kliknutím (například Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="ecfca-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="ecfca-131">Žádné</span><span class="sxs-lookup"><span data-stu-id="ecfca-131">None</span></span>  <br/> |<span data-ttu-id="ecfca-132">Samostatné aplikace nejsou ovlivněny.</span><span class="sxs-lookup"><span data-stu-id="ecfca-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="ecfca-133">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ecfca-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="ecfca-134">Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)</span><span class="sxs-lookup"><span data-stu-id="ecfca-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="ecfca-135">Žádné</span><span class="sxs-lookup"><span data-stu-id="ecfca-135">None</span></span>  <br/> |<span data-ttu-id="ecfca-136">Samostatné aplikace nejsou ovlivněny.</span><span class="sxs-lookup"><span data-stu-id="ecfca-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="ecfca-137">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ecfca-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="ecfca-138">Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ecfca-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="ecfca-139">Odinstalace 64bitových aplikací Office, pokud je v pořádku je nahradit 32bitovými aplikacemi Office</span><span class="sxs-lookup"><span data-stu-id="ecfca-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="ecfca-140">Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="ecfca-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="ecfca-141">Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich</span><span class="sxs-lookup"><span data-stu-id="ecfca-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="ecfca-142">Odinstalujte Office 2016 nainstalovaný instalační službou MSI.</span><span class="sxs-lookup"><span data-stu-id="ecfca-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="ecfca-p106">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.</span><span class="sxs-lookup"><span data-stu-id="ecfca-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="ecfca-145">Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office</span><span class="sxs-lookup"><span data-stu-id="ecfca-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="ecfca-146">Žádná</span><span class="sxs-lookup"><span data-stu-id="ecfca-146">None</span></span>  <br/> |<span data-ttu-id="ecfca-147">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe</span><span class="sxs-lookup"><span data-stu-id="ecfca-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="ecfca-148">**(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="ecfca-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="ecfca-149">Probíhá oprava.</span><span class="sxs-lookup"><span data-stu-id="ecfca-149">A fix is in progress.</span></span> 
  
