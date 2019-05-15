---
title: Začínáme s Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Naučte se nastavit Microsoft 365 Business.
ms.openlocfilehash: d309700761ee48ef66a8cd3886fd416c79463ed5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074294"
---
# <a name="get-started-with-microsoft-365-business"></a>Začínáme s Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co je Microsoft 365 Business

Microsoft 365 Business je komplexní sada nástrojů zaměřených na produktivitu firmy a spolupráci, do které například patří vždy aktuální Outlook, Word, Excel a další produkty Office. Pracovní soubory můžete chránit na všech zařízeních s iOSem, Androidem a Windows 10. Umožňuje to zabezpečení na podnikové úrovni s jednoduchou správou.
  
Microsoft 365 Business umožňuje používat maximálně 300 licencí. Pokud potřebujete více licencí, podívejte se na dokumentaci k [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986), kde získáte více informací. 
  
## <a name="get-microsoft-365-business"></a>Jak získat Microsoft 365 Business

- Pokud máte partnera, získá partner Microsoft 365 Business: [Jak získat Microsoft 365 Business z partnerského centra Microsoftu](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 Business, můžete si ho [koupit tady](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

 **Přehled Microsoft 365 Business Suite, nastavení**
  
Následující diagram popisuje, jak admins nastavit Microsoft 365 Business. Popisuje také kroky při přípravě počítačů s Windows na Microsoft 365 Business. Nová zařízení také můžete přidat v Centru pro správu Microsoft 365 Business s použitím [Windows AutoPilota](add-autopilot-devices-and-profile.md). Pomocí AutoPilota také můžete nastavit a předběžně nakonfigurovat nová zařízení, aby byla připravená k použití hned, jak se uživatel přihlásí pomocí přihlašovacích údajů služby Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: nastavit Microsoft 365 Business (Admin)

Přihlaste se do [Centra pro správu Microsoft 365 Business](https://portal.office.com/adminportal/home) pod přihlašovacími údaji globálního správce a nastavte Microsoft 365 Business podle následujících pokynů. 
  
1. [Předpoklady pro ochranu dat na zařízeních s Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte předpoklady, abyste měli jistotu, že vaše zařízení jsou na Microsoft 365 Business připravená.
    
2. [Nastavení Microsoft 365 Business pomocí průvodce nastavením](set-up.md)
    
    Pokud jste **trvale přesunout z místní služby Active Directory do cloudu**, můžete buď přidat uživatele ručně ve středisku pro správce Microsoft 365 Business pomocí Průvodce instalací nebo stačí jednorázová synchronizace s Azure AD připojit. Můžete to udělat dvěma způsoby: 
    
  - Také máte 2010 serveru Exchange, Exchange 2013 nebo Exchange 2016 server, můžete [Použít minimální hybridní rychle migrovat poštovní schránky serveru Exchange do služeb Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Kroky minimálních hybridních možností zahrnují jednorázovou synchronizaci uživatelů do Azure AD a zároveň přesun e-mailů z místního úložiště do cloudu. Po dokončení přesunu e-mailů se u této metody synchronizace adresářů automaticky vypne.
    
  - K synchronizaci uživatelů s cloudem můžete použít průvodce synchronizací adresářů Office 365. K dokončení tohoto procesu použijte postup, který je popsaný v článku [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po synchronizaci uživatelů s cloudem budete muset [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Každému uživateli přidanému tímto způsobem budete muset udělit licenci na Microsoft 365 Business. Lze provést v [Průvodci](set-up.md)nebo [přiřazení licencí uživatelům služeb Office 365 pro firmy](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů k instalaci zařízení a zkontrolujte, zda že jsou chráněny obchodní 365 Microsoft Office apps[nastavit mobilní zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md) . 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítače

Admins můžete předem vybrat nastavení pro nová zařízení počítačů se systémem Windows 10 pomocí [AutoPilot systému Windows](add-autopilot-devices-and-profile.md). Uživatelé mohou vytvořit své stávající nebo nové zařízení Windows 10 pomocí následujících kroků v tomto tématu: [Nastavení počítačů se systémem Windows Microsoft 365 Business uživatelům](set-up-windows-devices.md). Pro stávající zařízení mohou uživatelé také **Volitelně**[Přesunout soubory na OneDrive pro firmy](move-files-to-onedrive.md). Přesunout soubory, které jsou přidružené k profilu systému Windows k OneDrive lze také použít nástroje jiných výrobců.
  
Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních. Postupujte podle kroků v [doméně zařízení Windows 10, které jsou spravovány Microsoft 365 Business povolit](manage-windows-devices.md) toto nastavení. Toto je upřednostňovaný způsob a zařízení v tomto stavu se nazývají **hybridní Azure AD připojené zařízení**. 
  
Je-li zachovat místní služby Active Directory, která obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete přidělit přístup **Azure AD připojené zařízení** tyto prostředky podle pokynů zde: [přístup místního zdroje z Azure AD připojené zařízení Microsoft 365 Business](access-resources.md).
  
Po nastavení počítačů se systémem Windows 10 můžete [automaticky nainstalovat systém Office](auto-install-or-uninstall-office.md) na zařízení. 
  
## <a name="contact-support"></a>Kontaktujte podporu.

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako Microsoft 365 Business admin máte přístup k tým zákaznické podpory, [kontaktování podpory pro produkty business - Nápověda správce](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) ****
    
## <a name="related-topics"></a>Klepnutím na odkaz Příbuzná témata.
[Dokumentace a zdroje informací k Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoft 365 Business](manage.md)[Migrace na Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

