---
title: Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business
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
description: Dozvíte se, jak automaticky nainstalovat 32 aplikace sady Office do počítačů se systémem Windows 10 a průběžně je aktualizovat.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640763"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Pomocí aplikace Microsoft 365 Business můžete automaticky nainstalovat 32-bitové aplikace sady Office do počítačů se systémem Windows 10 a udržovat je v aktuálním provozu s aktualizacemi.
  
Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele v systému Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se zobrazí **aktualizace sady Office** , jak je znázorněno na následujícím obrázku, byla instalace provedena pomocí klepnutí na tlačítko Spustit. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Komu je tato funkce prospěšna**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má** uživatelskou licenci k Windows 10 Business, aktivní licenci k Microsoft 365 Business, Windows 10 Creators Update a je připojený k Azure Active Directory. 
    
- **Neobsahuje** 64 aplikací sady Office (příklad: Word, Excel, PowerPoint). Jsou-li požadovány 64 aplikace sady Office, není tato funkce vhodná, protože není k dispozici podpora spuštění systému Office 64-bit 2016, který lze spustit z konzoly Microsoft 365 Business Admin Console. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 Business upgraduje sadu Office na verzi sady Office 2016 pro spouštění a nelze ji použít v samostatných aplikacích sady Office 2016 MSI. 
    
V následující tabulce je uvedeno, jakou akci mohou koncoví uživatelé/správci provést v závislosti na jejich počátečním stavu, aby mohli úspěšně 32 verzi aplikace sady Office pro spuštění z aplikace Microsoft 365 v konzole pro správu podnikových aplikací.
  
|**Počáteční stav instalace Office**|**Prováděná akce před instalací Microsoft 365 Business Office**|**Konečný stav**|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádné  <br/> |Sada Office 2016 32-bit je instalována pomocí Klikni a Run  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádné  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Existující verze pro klepnutí na 32-bit sady Office a klepnutí na 32 bitů nebo 64-bitové samostatné aplikace sady Office (například aplikace Visio, projekt)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádné  <br/> |Samostatné aplikace nejsou ovlivněny. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> ||||
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalujte 64 aplikace sady Office, pokud je v pořádku, abyste je nahradili 32-bitovým aplikacím sady Office  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Probíhá oprava. 
  