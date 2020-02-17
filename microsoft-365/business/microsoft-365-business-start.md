---
title: Začínáme s Microsoft 365 Business
f1.keywords:
- NOCSH
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Naučte se nastavit Microsoft 365 Business.
ms.openlocfilehash: 5491486c2bf8da1ee38fcd986d5ecd682d57c82e
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065599"
---
# <a name="get-started-with-microsoft-365-business"></a>Začínáme s Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co je Microsoft 365 Business

Microsoft 365 Business je komplexní sada nástrojů pro produktivitu a spolupráci v podnikání, jako je Outlook, Word, Excel a další produkty Office, které jsou vždy aktuální. Pracovní soubory můžete chránit na všech svých zařízeních se systémem iOS, Android a Windows 10 pomocí podnikového zabezpečení, které se snadno spravuje.

Podívejte se na toto video pro rychlý přehled microsoft 365 business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business je určen až pro 300 licencí. Další informace naleznete v dokumentaci [k Microsoftu 365 Enterprise.](https://go.microsoft.com/fwlink/p/?linkid=860986) 
  
## <a name="get-microsoft-365-business"></a>Jak získat Microsoft 365 Business

- Pokud máte partnera, dostanou Microsoft 365 Business: [Získejte Microsoft 365 Business od Centra microsoft partnerů](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 Business, můžete si ho [koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

 **Přehled nastavení sady Microsoft 365 Business Suite**
  
Následující diagram popisuje, jak správci nastavují Microsoft 365 Business. Popisuje také kroky při přípravě počítačů s Windows na Microsoft 365 Business. Můžete také přidat nová zařízení v Centru pro správu Microsoft 365 Business pomocí [programu Windows AutoPilot](add-autopilot-devices-and-profile.md). Pomocí programu AutoPilot můžete nastavit a předkonfigurovat nová zařízení tak, aby byla připravena k produktivnímu použití, jakmile se uživatel přihlásí pomocí svých přihlašovacích údajů microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Podívejte se na toto video, kde najdete přehled nastavení Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Nastavení Microsoft 365 Business (Admin)

Přihlaste se do [Centra pro správu Microsoftu 365 Business](https://portal.office.com/adminportal/home) pomocí globálních přihlašovacích údajů pro správce a proveďte následující kroky k nastavení Microsoft365 Business. 
  
1. [Předpoklady pro ochranu dat na zařízeních s Microsoft em 365 Business](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte požadavky, abyste se ujistili, že jsou vaše zařízení připravena pro Microsoft 365 Business.
    
2. [Nastavení microsoftu 365 business pomocí Průvodce instalací](set-up.md)
    
    Pokud se **trvale stěhujete z místní služby Active Directory do cloudu**, můžete přejít do Centra pro správu Microsoft 365 Business a pomocí Průvodce nastavením přidat uživatele ručně, nebo můžete provést jednorázovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte také server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete [pomocí minimálního hybridního serveru rychle migrovat poštovní schránky Exchange do Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Minimální hybridní kroky zahrnují jednorázovou synchronizaci uživatelů s Azure AD a migraci e-mailů z místního do cloudu. Po dokončení migrace e-mailu je synchronizace adresářů při použití této metody automaticky vypnuta.
    
    - K synchronizaci uživatelů s cloudem použijte Průvodce synchronizací adresářů Office 365. K dokončení tohoto procesu použijte postup, který je popsaný v článku [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po synchronizaci uživatelů do cloudu budete muset [vypnout synchronizaci adresářů pro Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Budete také muset dát každému uživateli, který byl přidán tímto způsobem licenci microsoft 365 business. Můžete to provést v [Průvodci nastavením](set-up.md) nebo můžete [přiřadit licence uživatelům v Office 365 pro firmy](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Podle pokynů v [části Nastavení mobilních zařízení pro uživatele Microsoft 365 Business nainstalujte](set-up-mobile-devices.md) aplikace Office na zařízení a ujistěte se, že jsou chráněny Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítačů

Správci mohou předem vybrat nastavení pro nové počítače s Windows 10 pomocí [systému Windows AutoPilot](add-autopilot-devices-and-profile.md). Uživatelé mohou nastavit stávající nebo nová zařízení s Windows 10 podle kroků v tomto tématu: [Nastavení počítačů se systémem Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md). U stávajících zařízení mohou uživatelé **volitelně** [přesouvat soubory na OneDrive pro firmy](move-files-to-onedrive.md). Mohou také používat nástroje jiných výrobců k přesunutí souborů přidružených k profilu systému Windows na OneDrive.
  
Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business k ochraně zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Podle pokynů v [části Povolit zařízení windows 10 připojená k doméně, která má spravovat Microsoft 365 Business,](manage-windows-devices.md) a nastavte tak to. Tato metoda je upřednostňovaná a zařízení v tomto stavu se nazývají **hybridní zařízení připojená ke službě Azure AD**. 
  
Pokud si ponecháte místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete k těmto prostředkům udělit přístup k těmto prostředkům **se službou Azure AD** takto podle kroků: [Přístup k místním prostředkům ze zařízení se službou Azure AD v Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktujte podporu.

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako správce Microsoft 365 Business máte přístup k našemu týmu zákaznické podpory: ** [Kontaktní podpora pro firemní produkty – nápověda pro správce](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Viz také

[Dokumentace a zdroje informací k Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoft 365 Business](manage.md)[Migrace na Microsoft 365 Business](migrate-to-microsoft-365-business.md)

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
