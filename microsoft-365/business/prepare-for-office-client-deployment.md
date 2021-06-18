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
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924221"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Příprava na nasazení klienta Office od Microsoftu 365 pro firmy

Tento článek se týká Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Příprava k automatické instalaci aplikací Office na klientské počítače

Microsoft 365 Business Premium můžete použít k automatické instalaci 32bitových aplikací Office na počítače s Windows 10 a k jejich aktualizaci.
  
Automatická instalace funguje nejlépe, pokud je počítač koncového uživatele ve Windows 10 Business a:
  
- Nemá stávající desktopové aplikace Office (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access a OneDrive).
    
    nebo
    
- Má nainstalovanou stávající verzi Office technologií Klikni a spusť.
    
Pokud potřebujete zjistit, jestli máte verzi Office nainstalovanou technologií Klikni a spusť, přejděte v libovolné aplikaci Office na **Soubor** \> **Účet** (v Outlooku je to **Účet Office**). Pokud se zobrazí **aktualizace Office,** jak je vidět na následujícím obrázku, instalace byla provedena pomocí klikni a spouštěče. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kdo může tuto funkci využívat**
  
Koncový uživatel s počítačem, který splňuje následující podmínky:
  
- **Má**  uživatelskou licenci pro Windows 10 Business, aktivní licenci Microsoft 365 pro firmy, Windows 10 Creators Update a je připojená k Azure Active Directory. 
    
- **Nemá 64bitové** aplikace Office (například Word, Excel, PowerPoint). Pokud jsou vyžadovány 64bitové aplikace Office, není tato funkce vhodná, protože neexistuje podpora pro aktivaci 64bitové verze Office 2016 Klikni a spouštěč z konzoly pro správu Microsoft 365 pro firmy. 
    
- **Nemá** samostatné aplikace nainstalované instalační službou Windows 2016 (MSI), jako je Visio nebo Project. Microsoft 365 pro firmy upgraduje Office na verzi Office 2016 klikni a spouštět, která nefunguje se samostatnými aplikacemi Office 2016 MSI. 
    
Následující tabulka ukazuje, jakou akci musí koncoví uživatelé/správci provést v závislosti na jejich počátečním stavu, aby z konzoly pro správu Microsoftu 365 pro firmy byla úspěšná 32bitová verze nasazení Office klikni a spouštěná.<br/>


|Počáteční stav instalace Office|Akce před instalací Office Microsoft 365 pro firmy|Konečný stav|
|:-----|:-----|:-----|
|Sada Office není nainstalovaná  <br/> |Žádná  <br/> |32bitová verze Office 2016 se instaluje pomocí klikni a spouštěče.  <br/> |
|Stávající 32bitová verze Office (2016 nebo starší) nainstalovaná technologií Klikni a spusť bez samostatných aplikací  <br/> |Žádná  <br/> |Upgrade na nejnovější 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť podle toho, co je potřeba **\*** <br/> |
|Stávající 32bitová verze Office klikni a spouštěná 32bitová nebo 64bitová samostatná aplikace Office (například Visio, Project)  <br/> |Žádné  <br/> |Na samostatné aplikace se to neovlivní. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Stávající 32 bitová verze Office nainstalovaná technologií Klikni a spusť a všechny 32bitové nebo 64bitové samostatné aplikace Office nainstalované instalační službou MSI (s výjimkou verzí 2016)  <br/> |Žádná  <br/> |Na samostatné aplikace se to neovlivní. Sada se upgraduje na 32bitovou verzi Office 2016 nainstalovanou technologií Klikni a spusť  <br/> |
|Jakákoli stávající 64bitová verze Office nainstalovaná technologií Klikni a spusť  <br/> |Odinstalace 64bitových aplikací Office, pokud je to ok, nahraďte je 32bitovou aplikací Office  <br/> |Pokud jsou odebrané 64bitové verze aplikací Office, nainstaluje se 32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť  <br/> |
|Stávající Office 2016 nainstalovaný instalační službou MSI se samostatnými aplikacemi nebo bez nich  <br/> |Odinstalujte Office 2016 nainstalovaný instalační službou MSI.  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť. Samostatné aplikace zůstávají beze změn.  <br/> |
|Stávající instalace MSI systému Office 2013 (nebo předchozích verzí) a/nebo samostatné aplikace Office  <br/> |Žádná  <br/> |32bitová verze Office 2016 nainstalovaná technologií Klikni a spusť a předchozí instalace MSI systému Office (a samostatných aplikací) existují vedle sebe  <br/> |
||||
   
 **(\*) Poznámka:** Kvůli známé chybě není možné provést upgrade na 32bitovou verzi Office 2016 využívající technologii Klikni a spusť. Probíhá oprava. 
  
