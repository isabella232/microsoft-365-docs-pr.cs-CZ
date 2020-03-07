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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Přečtěte si o Microsoft 365 Business, jak ho nastavit a jak připravit zařízení a počítače uživatelů, abyste zajistili, že jsou chráněni Microsoftem 365 Business.
ms.openlocfilehash: 220fb747e2bc501f3f6d46d967b30d2e5fd79a4a
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561434"
---
# <a name="get-started-with-microsoft-365-business"></a>Začínáme s Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co je Microsoft 365 Business

Microsoft 365 Business je komplexní sada nástrojů pro produktivitu a spolupráci firem, jako jsou Outlook, Word, Excel a další produkty Office, které jsou vždy aktuální. Pracovní soubory můžete chránit na všech zařízeních se systémem iOS, Android a Windows 10 pomocí zabezpečení na podnikové úrovni, které se snadno spravuje.

Podívejte se na toto video, kde najdete rychlý přehled microsoftu 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business je určen až pro 300 licencí. Pokud potřebujete další licence, další informace najdete v dokumentaci k [Microsoft 365 Enterprise.](https://go.microsoft.com/fwlink/p/?linkid=860986) 
  
## <a name="get-microsoft-365-business"></a>Jak získat Microsoft 365 Business

- Pokud máte partnera, získá Microsoft 365 Business: [Získejte Microsoft 365 Business z Microsoft Partner Center](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 Business, můžete si ho [koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

 **Přehled nastavení sady Microsoft 365 Business Suite**
  
Následující diagram popisuje, jak správci nastavili Microsoft 365 Business. Popisuje také kroky při přípravě počítačů s Windows na Microsoft 365 Business. Nová zařízení můžete přidat také v Centru pro správu Microsoft 365 Business pomocí [systému Windows AutoPilot](add-autopilot-devices-and-profile.md). Pomocí funkce AutoPilot můžete nastavit a předem nakonfigurovat nová zařízení tak, aby byla připravena k produktivnímu použití, jakmile se uživatel přihlásí pomocí přihlašovacích údajů k Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Podívejte se na toto video s přehledem nastavení Microsoftu 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Nastavení Microsoft 365 Business (Správce)

Přihlaste se k [Centru pro správu Microsoft 365 Business](https://portal.office.com/adminportal/home) pomocí přihlašovacích údajů pro globálního správce a proveďte následující kroky k nastavení Microsoftu 365 Business. 
  
1. [Požadavky na ochranu dat na zařízeních s Microsoftem 365 Business](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte požadavky a ujistěte se, že jsou vaše zařízení připravená pro Microsoft 365 Business.
    
2. [Nastavení Microsoft 365 Business pomocí průvodce instalací](set-up.md)
    
    Pokud trvale **přecházíte z místní služby Active Directory do cloudu**, můžete přejít do Centra pro správu Microsoft 365 Business a pomocí průvodce nastavením přidat uživatele ručně, nebo můžete provést jednorázovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte taky server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete [pomocí minimálního hybridu rychle migrovat poštovní schránky Exchange do Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Mezi minimální hybridní kroky patří jednorázová synchronizace uživatelů s Azure AD a migrace e-mailu z místního do cloudu. Po dokončení migrace e-mailu je synchronizace adresáře automaticky vypnuta při použití této metody.
    
    - Pomocí Průvodce synchronizací adresářů Office 365 synchronizujte uživatele s cloudem. K dokončení tohoto procesu použijte postup, který je popsaný v článku [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po synchronizaci uživatelů s cloudem budete muset [vypnout synchronizaci adresářů pro Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Budete také muset dát každému uživateli, který byl přidán tímto způsobem licenci k Microsoft 365 Business. Můžete to provést v [průvodci nastavením](set-up.md) nebo můžete [přiřadit licence uživatelům v Office 365 pro firmy](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů v části [Nastavení mobilních zařízení pro uživatele Microsoft365 Business,](set-up-mobile-devices.md) nainstalujte aplikace Office na zařízení a ujistěte se, že jsou chráněné Microsoftem 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítačů

Správci mohou předem vybrat nastavení pro nové počítače s Windows 10 pomocí [windows autopilota](add-autopilot-devices-and-profile.md). Uživatelé mohou nastavit svá stávající nebo nová zařízení s Windows 10 podle kroků v tomto tématu: [Nastavení počítačů s Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md). U stávajících zařízení **můžou** uživatelé volitelně [přesouvat soubory na OneDrive pro firmy](move-files-to-onedrive.md). Pomocí nástrojů jiných výrobců mohou také přesouvat soubory přidružené k profilu Windows na OneDrive.
  
Pokud vaše organizace používá službu Windows Server Active Directory místně, můžete nastavit Microsoft 365 Business tak, aby chránila vaše zařízení s Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle pokynů v [části Povolit, aby zařízení s Windows 10 připojená k doméně byla spravována microsoftem 365 Business,](manage-windows-devices.md) abyste to nastavili. Tato metoda je upřednostňována a zařízení v tomto stavu se nazývají **hybridní zařízení azure ad připojená**. 
  
Pokud si ponecháte místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízením **s azure ad připojit** k těmto prostředkům poskytnout přístup k těmto prostředkům podle následujících kroků: Přístup k místním [prostředkům ze zařízení pro připojení K OnD v Microsoftu 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktování podpory

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako správce Microsoft 365 Business máte přístup k našemu týmu zákaznické podpory: ** [Obraťte se na podporu pro firemní produkty – nápověda pro správce](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Viz také

[Dokumentace a zdroje informací k Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoft 365 Business](manage.md)[Migrace na Microsoft 365 Business](migrate-to-microsoft-365-business.md)

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
