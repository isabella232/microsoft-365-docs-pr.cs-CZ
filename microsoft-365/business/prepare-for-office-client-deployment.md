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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Přečtěte si, jak automaticky nainstalovat 32bitové aplikace Office do počítačů s Windows 10 a jak je aktualizovat.
ms.openlocfilehash: b5f01bc9bb10765929f3c6bdd5908e8b48a51a11
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633093"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Příprava na nasazení klienta Office microsoftem 365 pro firmy

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Pomocí Microsoftu 365 pro firmy můžete automaticky instalovat 32bitové aplikace Office do počítačů s Windows 10 a udržovat je aktuální pomocí aktualizací.
  
Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele v systému Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se aktualizace **Office** zobrazují tak, jak je znázorněno na následujícím obrázku, instalace byla provedena pomocí technologie Klikni a spusť. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kdo má prospěch z této funkce**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má** uživatelskou licenci pro Windows 10 Business, aktivní licenci Microsoft 365 pro firmy, aktualizaci Windows 10 Creators Update a je připojená k Azure Active Directory. 
    
- **Nemá** 64bitové aplikace Office (například Word, Excel, PowerPoint). Pokud jsou vyžadovány 64bitové aplikace Office, pak se tato funkce nehodí, protože neexistuje žádná podpora pro spuštění 64bitové verze Office s funkcí Klikni a spusť z konzoly microsoftu 365 pro firmy. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 pro firmy upgraduje Office na verzi Office 2016 s klikem a spouštěním, která nefunguje se samostatnými aplikacemi MSI Office 2016. 
    
V následující tabulce je uvedeno, jakou akci mohou koncoví uživatelé nebo správci v závislosti na počátečním stavu provést, aby měli úspěšnou 32bitovou verzi office s pouštěním z konzole pro správu Microsoftu 365 pro firmy.
  
|**Počáteční stav instalace Office**|**Akce, která má být dokončena před instalací Microsoftu 365 pro firmy, instalace Office**|**Konečný stav**|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádné  <br/> |32bitový Office 2016 je nainstalovaný pomocí technologie Klikni a spusť  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádné  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Existující 32bitová verze 32bitových nebo 64bitových samostatných aplikací Office s 32bitovým nebo 64bitovým kliknutím (například Visio, Project)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> ||||
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalace 64bitových aplikací Office, pokud je v pořádku je nahradit 32bitovými aplikacemi Office  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Probíhá oprava. 
  
