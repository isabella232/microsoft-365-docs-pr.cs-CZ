---
title: Příprava Office nasazení klienta Microsoft 365 pro firmy
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
description: Zjistěte, jak automaticky nainstalovat 32bitové aplikace Office na Windows 10 počítače a aktualizovat je.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803554"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Příprava Office nasazení klienta Microsoft 365 pro firmy

Tento článek se týká Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Pomocí funkce Microsoft 365 Business Premium můžete automaticky nainstalovat 32bitové aplikace Office na Windows 10 počítače a udržovat je aktuální v aktualizacích.
  
Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud vidíte **Office,** jak je znázorněno na následujícím obrázku, instalace byla provedena pomocí klikni a spouště. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kdo výhody této funkce**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má** Windows 10 Business licenci, aktivní Microsoft 365 pro firmy, Windows 10 Creators Update a je připojen k Azure Active Directory. 
    
- **Nemá 64bitové** aplikace Office (například Word, Excel, PowerPoint). Pokud jsou vyžadovány 64bitové Office aplikace, není tato funkce vhodná, protože neexistuje podpora pro aktivaci 64bitové verze 2016 klikni a spouštěč Office z konzoly Microsoft 365 pro firemní správce. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 pro firmy Office verzi Office 2016, která nefunguje s Office 2016 MSI. 
    
Následující tabulka ukazuje, jakou akci musí koncoví uživatelé nebo správci provést v závislosti na jejich počátečním stavu, aby z konzoly pro správu Microsoft 365 pro firmy byla úspěšná 32bitová verze nasazení Office klikni a spouštěná.<br/>


|Počáteční stav instalace Office|Akce, která se má provést před Microsoft 365 instalace Office pro firmy|Konečný stav|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádná  <br/> |Office 32bitová verze 2016 je nainstalovaná pomocí funkce Klikni a spouštět  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádná  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Stávající 32bitová verze Office a 32bitová nebo 64bitová samostatná aplikace Office klikni a spouštěná (například Visio, Project)  <br/> |Žádné  <br/> |Na samostatné aplikace se to neovlivní. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádná  <br/> |Na samostatné aplikace se to neovlivní. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalace 64bitových Office aplikací, pokud je v pořádku, nahraďte je 32bitovými Office aplikacemi  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Probíhá oprava. 
  
