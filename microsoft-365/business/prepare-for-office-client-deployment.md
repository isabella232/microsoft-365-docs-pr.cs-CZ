---
title: Příprava na nasazení klienta Office od Microsoftu 365 pro firmy
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Zjistěte, jak automaticky nainstalovat 32bitové aplikace Office na počítače s Windows 10 a aktualizovat je.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580048"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="9805c-103">Příprava na nasazení klienta Office od Microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="9805c-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="9805c-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9805c-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="9805c-105">Příprava k automatické instalaci aplikací Office na klientské počítače</span><span class="sxs-lookup"><span data-stu-id="9805c-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="9805c-106">Microsoft 365 Business Premium můžete použít k automatické instalaci 32bitových aplikací Office na počítače s Windows 10 a k jejich aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="9805c-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="9805c-107">Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele ve Windows 10 Business a:</span><span class="sxs-lookup"><span data-stu-id="9805c-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="9805c-108">Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).</span><span class="sxs-lookup"><span data-stu-id="9805c-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="9805c-109">nebo</span><span class="sxs-lookup"><span data-stu-id="9805c-109">or</span></span>
    
- <span data-ttu-id="9805c-110">Má nainstalovanou stávající verzi Office technologií Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="9805c-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="9805c-111">Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**).</span><span class="sxs-lookup"><span data-stu-id="9805c-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="9805c-112">Pokud se zobrazí **aktualizace Office,** jak je vidět na následujícím obrázku, instalace byla provedena pomocí klikni a spouštěče.</span><span class="sxs-lookup"><span data-stu-id="9805c-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="9805c-114">**Kdo může tuto funkci využívat**</span><span class="sxs-lookup"><span data-stu-id="9805c-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="9805c-115">Koncový uživatel s počítačem, který splňuje následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="9805c-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="9805c-116">**Má**  uživatelskou licenci pro Windows 10 Business, aktivní licenci Microsoft 365 pro firmy, Windows 10 Creators Update a je připojená k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9805c-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="9805c-117">**Nemá 64bitové** aplikace Office (například Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="9805c-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="9805c-118">Pokud jsou vyžadovány 64bitové aplikace Office, není tato funkce vhodná, protože neexistuje podpora pro aktivaci 64bitové verze Office 2016 Klikni a spouštěč z konzoly pro správu Microsoft 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="9805c-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="9805c-119">**Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project.</span><span class="sxs-lookup"><span data-stu-id="9805c-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="9805c-120">Microsoft 365 pro firmy upgraduje Office na verzi Office 2016 klikni a spouštět, která nefunguje se samostatnými aplikacemi Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="9805c-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="9805c-121">Následující tabulka ukazuje, jakou akci musí koncoví uživatelé/správci provést v závislosti na jejich počátečním stavu, aby z konzoly pro správu Microsoftu 365 pro firmy byla úspěšná 32bitová verze nasazení Office klikni a spouštěná.</span><span class="sxs-lookup"><span data-stu-id="9805c-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="9805c-122">**Počáteční stav instalace Office**</span><span class="sxs-lookup"><span data-stu-id="9805c-122">**Starting Office install status**</span></span>|<span data-ttu-id="9805c-123">**Akce před instalací Office Microsoft 365 pro firmy**</span><span class="sxs-lookup"><span data-stu-id="9805c-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="9805c-124">**Konečný stav**</span><span class="sxs-lookup"><span data-stu-id="9805c-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9805c-125">Sada Office není nainstalovaná</span><span class="sxs-lookup"><span data-stu-id="9805c-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="9805c-126">Žádná</span><span class="sxs-lookup"><span data-stu-id="9805c-126">None</span></span>  <br/> |<span data-ttu-id="9805c-127">32bitová verze Office 2016 se instaluje pomocí klikni a spouštěče.</span><span class="sxs-lookup"><span data-stu-id="9805c-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="9805c-128">Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací</span><span class="sxs-lookup"><span data-stu-id="9805c-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="9805c-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="9805c-129">None</span></span>  <br/> |<span data-ttu-id="9805c-130">Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\***</span><span class="sxs-lookup"><span data-stu-id="9805c-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="9805c-131">Stávající 32bitová verze Office klikni a spouštěná 32bitová nebo 64bitová samostatná aplikace Office (například Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="9805c-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="9805c-132">Žádné</span><span class="sxs-lookup"><span data-stu-id="9805c-132">None</span></span>  <br/> |<span data-ttu-id="9805c-133">Na samostatné aplikace se to neovlivní.</span><span class="sxs-lookup"><span data-stu-id="9805c-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="9805c-134">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="9805c-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="9805c-135">Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)</span><span class="sxs-lookup"><span data-stu-id="9805c-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="9805c-136">Žádná</span><span class="sxs-lookup"><span data-stu-id="9805c-136">None</span></span>  <br/> |<span data-ttu-id="9805c-137">Na samostatné aplikace se to neovlivní.</span><span class="sxs-lookup"><span data-stu-id="9805c-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="9805c-138">Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="9805c-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="9805c-139">Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="9805c-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="9805c-140">Odinstalace 64bitových aplikací Office, pokud je to ok, nahraďte je 32bitovou aplikací Office</span><span class="sxs-lookup"><span data-stu-id="9805c-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="9805c-141">Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť</span><span class="sxs-lookup"><span data-stu-id="9805c-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="9805c-142">Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich</span><span class="sxs-lookup"><span data-stu-id="9805c-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="9805c-143">Odinstalujte Office 2016 nainstalovaný instalační službou MSI.</span><span class="sxs-lookup"><span data-stu-id="9805c-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="9805c-p106">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.</span><span class="sxs-lookup"><span data-stu-id="9805c-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="9805c-146">Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office</span><span class="sxs-lookup"><span data-stu-id="9805c-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="9805c-147">Žádná</span><span class="sxs-lookup"><span data-stu-id="9805c-147">None</span></span>  <br/> |<span data-ttu-id="9805c-148">32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe</span><span class="sxs-lookup"><span data-stu-id="9805c-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="9805c-149">**(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="9805c-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="9805c-150">Probíhá oprava.</span><span class="sxs-lookup"><span data-stu-id="9805c-150">A fix is in progress.</span></span> 
  
