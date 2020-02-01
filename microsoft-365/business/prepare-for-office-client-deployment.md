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
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Pomocí Microsoftu 365 Business můžete automaticky nainstalovat 32bitové aplikace Office do počítačů s Windows 10 a udržovat je aktuální s aktualizacemi.
  
Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele v systému Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se zobrazí **aktualizace Office,** jak je znázorněno na následujícím obrázku, instalace byla provedena pomocí funkce Klikněte na spouštění. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kdo má prospěch z této funkce**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má** uživatelskou licenci k Windows 10 Business, aktivní licenci k Microsoft 365 Business, Windows 10 Creators Update a je připojený k Azure Active Directory. 
    
- **Nemá** 64bitové aplikace Office (například Word, Excel, PowerPoint). Pokud jsou vyžadovány 64bitové aplikace Office, pak se tato funkce nehodí, protože neexistuje žádná podpora pro spuštění 64bitové verze Office pro kliky a spuštění z konzoly pro správu Microsoft 365 Business. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 Business upgraduje Office na verzi Pro klika a běh Office 2016 a to nefunguje se samostatnými aplikacemi Office 2016 MSI. 
    
V následující tabulce je uvedeno, jakou akci mohou koncoví uživatelé/správci v závislosti na počátečním stavu provést, aby mohli mít úspěšnou 32bitovou verzi nasazení Office pro spuštění z konzoly pro správu Microsoft 365 Business.
  
|**Počáteční stav instalace Office**|**Prováděná akce před instalací Microsoft 365 Business Office**|**Konečný stav**|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádné  <br/> |Office 2016 32bitový je nainstalován pomocí funkce Klikni na spouštění  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádné  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Existující 32bitová verze Office pro spouštění kliknutím a 32bitové nebo 64bitové samostatné aplikace Office spusťte kliknutím a spusťte 32bitové nebo 64bitové (například Visio, Project)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> ||||
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalujte 64bitové aplikace Office, pokud je v pořádku je nahradit 32bitovými aplikacemi Office  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Probíhá oprava. 
  