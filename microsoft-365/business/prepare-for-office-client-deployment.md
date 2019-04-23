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
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Příprava nasazení klienta Office prostřednictvím plánu Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Microsoft 365 Business můžete použít k instalaci 32bitových aplikací Office na počítače s Windows 10 a k jejich udržování v aktuálním stavu prostřednictvím aktualizací.
  
Nejlépe to funguje, pokud počítač koncového uživatele používá Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se zobrazí stejné aktualizace Office jako na následujícím obrázku, byla k instalaci použita technologie Klikni a spusť. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Pro koho je tato funkce užitečná?**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má** uživatelskou licenci k Windows 10 Business, aktivní licenci k Microsoft 365 Business, Windows 10 Creators Update a je připojený k Azure Active Directory. 
    
- **Nemá** 64bitové aplikace Office (např. Word, Excel, PowerPoint). Pokud potřebujete 64bitové aplikace Office, není tato funkce vhodná, protože nepodporuje spuštění 64bitové verze Office 2016 technologií Klikni a spusť z konzoly pro správu Microsoft 365 Business. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 Business upgraduje Office na verzi Office 2016 nainstalovanou technologií Klikni a spusť, která ale nefunguje se samostatnými aplikacemi Office 2016 nainstalovanými instalační službou MSI. 
    
Následující tabulka podrobně popisuje, jakou akci musí koncoví uživatelé / správci provést podle toho, jaký je počáteční stav, aby mohli z konzoly pro správce Microsoft 365 Business úspěšně nasadit 32bitovou verzi Office nainstalovanou technologií Klikni a spusť.
  
|**Počáteční stav instalace Office**|**Prováděná akce před instalací Microsoft 365 Business Office**|**Konečný stav**|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádná  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Stávající 32bitová verze Office nainstalovaná technologií Klikni a spusť a 32bitové nebo 64bitové samostatné aplikace Office (například Visio nebo Project) nainstalované technologií Klikni a spusť  <br/> |Žádná  <br/> |Samostatné aplikace se nezmění. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádná  <br/> |Samostatné aplikace se nezmění. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> ||||
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalujte 64bitové aplikace Office, pokud je možné je nahradit 32bitovými aplikacemi Office.  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Na opravě se pracuje. 
  


