---
title: Začínáme s Microsoftem 365 pro firmy
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Přečtěte si o Microsoftu 365 pro firmy, o tom, jak ho nastavit a jak připravit zařízení a počítače uživatelů, abyste zajistili, že jsou chráněni Microsoftem 365 pro firmy.
ms.openlocfilehash: aedcf78f10707dbe6a1d1527effea7d56283dce0
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080037"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Začínáme s Microsoftem 365 pro firmy

## <a name="what-is-microsoft-365-for-business"></a>Co je Microsoft 365 pro firmy

Microsoft 365 pro firmy je komplexní sada nástrojů pro produktivitu a spolupráci, jako je Outlook, Word, Excel a další produkty Office, které jsou vždy aktuální. Pracovní soubory můžete chránit na všech svých zařízeních se systémy iOS, Android a Windows 10 pomocí zabezpečení na podnikové úrovni, které se snadno spravuje.

Podívejte se na toto video, kde najdete rychlý přehled Microsoftu 365 pro firmy.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 pro firmy je určen až pro 300 licencí. Pokud potřebujete více licencí, najdete další informace v dokumentaci k [Microsoftu 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986). 
  
## <a name="get-microsoft-365-for-business"></a>Získejte Microsoft 365 pro firmy

- Pokud máte partnera, získají Microsoft 365 pro firmy: [Získejte Microsoft 365 pro firmy z Microsoft Partner Center](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 pro firmy, můžete [si ho koupit zde](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Nastavení Microsoftu 365 pro firmy

 **Přehled sady Microsoft 365 pro firmy**
  
Následující diagram popisuje, jak správci nastavili Microsoft 365 pro firmy. Popisuje také postup přípravy počítačů se systémem Windows pro Microsoft 365 pro firmy. Nová zařízení můžete přidat také v Centru pro správu Microsoftu 365 pomocí [automatického panelu windows](add-autopilot-devices-and-profile.md). Pomocí funkce AutoPilot můžete nastavit a předem nakonfigurovat nová zařízení tak, aby byla připravená k produktivnímu použití, jakmile se uživatel přihlásí pomocí svých přihlašovacích údajů microsoftu 365 pro firmy.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Podívejte se na toto video, kde najdete přehled nastavení Microsoftu 365 pro firmy.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Nastavení Microsoftu 365 pro firmy (Admin)

Přihlaste se do [Centra pro správu Microsoftu 365](https://portal.office.com/adminportal/home) pomocí svých přihlašovacích údajů globálního správce a proveďte následující kroky k nastavení Microsoftu 365 pro firmy. 
  
1. [Požadavky na ochranu dat na zařízeních s Microsoft 365 pro firmy](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte požadavky, abyste se ujistili, že jsou vaše zařízení připravená pro Microsoft 365 pro firmy.
    
2. [Nastavení Microsoftu 365 pro firmy pomocí Průvodce nastavením](set-up.md)
    
    Pokud se **trvale přesouváte z místní služby Active Directory do cloudu**, můžete přejít do Centra pro správu Microsoftu 365 a pomocí průvodce nastavením přidat uživatele ručně, nebo můžete provést jednorázovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte taky server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete [pomocí minimalního hybridu rychle migrovat poštovní schránky Exchange do Microsoftu 365](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). Minimální hybridní kroky zahrnují jednorázovou synchronizaci uživatelů s Azure AD a migraci e-mailu z místního prostředí do cloudu. Po dokončení migrace e-mailu je synchronizace adresářů při použití této metody automaticky vypnuta.
    
    - Pomocí Průvodce synchronizací adresářů synchronizujte uživatele s cloudem. Tento proces dokončete podle pokynů v části [Nastavení synchronizace adresářů pro Microsoft 365.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) Po synchronizaci uživatelů do cloudu budete muset [vypnout synchronizaci adresářů pro Microsoft 365](https://docs.microsoft.com/office365/enterprise/turn-off-directory-synchronization).
    
    Budete také muset dát každému uživateli, který byl přidán tímto způsobem licenci microsoft 365 pro firmy. Můžete to udělat v [průvodci instalací](set-up.md) nebo můžete [přiřadit licence uživatelům](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů v části [Nastavení mobilních zařízení pro Microsoft 365 pro firemní uživatele](set-up-mobile-devices.md) k instalaci aplikací Office na zařízení a ujistěte se, že jsou chráněny Microsoftem 365 pro firmy. 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítačů

Správci mohou předem vybrat nastavení pro nové počítače s Windows 10 pomocí [automatického připojení systému Windows](add-autopilot-devices-and-profile.md). Uživatelé mohou nastavit svá stávající nebo nová zařízení s Windows 10 podle kroků v tomto tématu: [Nastavení počítačů s Windows pro Microsoft 365 pro firemní uživatele](set-up-windows-devices.md). U stávajících zařízení mohou uživatelé **volitelně** [přesouvat soubory na OneDrive pro firmy](move-files-to-onedrive.md). Mohou také používat nástroje třetích stran k přesunutí souborů přidružených k profilu Windows na OneDrive.
  
Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 pro firmy k ochraně vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Podle pokynů v části [Povolit zařízení s Windows 10 připojená k doméně, která budou spravována Microsoftem 365 pro firmy,](manage-windows-devices.md) aby se to nastavilo. Tato metoda je upřednostňována a zařízení v tomto stavu se nazývají **hybridní zařízení spojené Azure AD**. 
  
Pokud zachováte místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete **zařízením spojeným s Azure AD** udělit přístup k těmto prostředkům takto: Přístup k místním [prostředkům ze zařízení spojených s Azure AD v Microsoftu 365 pro firmy](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktování podpory

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako správce Microsoftu 365 pro firmy máte přístup k našemu týmu zákaznické podpory: ** [Kontaktujte podporu pro firemní produkty – nápovědu pro správce.](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Viz také

[Microsoft 365 pro obchodní dokumentaci a materiály](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoftu 365 pro firmy](manage.md)[Migrace na Microsoft 365 pro firmy](migrate-to-microsoft-365-business.md)

[Školicí videa microsoftu 365 pro firmy](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
