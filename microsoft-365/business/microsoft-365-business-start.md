---
title: Začínáme s Microsoft 365 pro firmy
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
description: Informace o aplikaci Microsoft 365 pro firmy, o tom, jak ji nastavit, a o tom, jak připravit zařízení a počítače uživatelů, aby byla chráněna Microsoft 365 pro firmy.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306483"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Začínáme s Microsoft 365 pro firmy

## <a name="what-is-microsoft-365-for-business"></a>Co je Microsoft 365 pro firmy

Microsoft 365 pro firmy je komplexní sada kancelářských nástrojů pro zvýšení produktivity a spolupráce, jako je Outlook, Word, Excel a další produkty Office, které jsou vždycky aktuální. Svoje pracovní soubory můžete chránit na zařízeních s iOS, Androidem a Windows 10 se zabezpečením rozlehlých sítí, které můžete spravovat.

V tomto videu najdete rychlý přehled o Microsoft 365 pro firmy.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 pro firmy je určen až pro 300 licencí. Pokud potřebujete více licencí, najdete další informace v dokumentaci k [Microsoftu 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986). 
  
## <a name="get-microsoft-365-for-business"></a>Získejte Microsoft 365 pro firmy

- Pokud máte partnera, získá Microsoft 365 pro firmy: [Získejte microsoft 365 pro firmy z partnerského centra Microsoftu](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 pro firmy, můžete si [ho koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Nastavení Microsoft 365 pro firmy

 **Základní informace o nastavení Microsoft 365 pro firmy**
  
Následující diagram popisuje, jak správci nastavují Microsoft 365 pro firmy. Popisuje také postup pro přípravu počítačů s Windows pro Microsoft 365 pro firmy. V centru pro správu Microsoft 365 můžete přidat nová zařízení taky pomocí [autopilota pro Windows](add-autopilot-devices-and-profile.md). Pomocí autopilotního nasazení můžete nastavit a předem nakonfigurovat nová zařízení, aby je bylo možné používat, jakmile se uživatel přihlásí pomocí svých přihlašovacích údajů Microsoft 365 pro firmy.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

V tomto videu najdete přehled nastavení Microsoft 365 pro firmy.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: nastavení Microsoft 365 pro firmy (správce)

Přihlaste se do [centra pro správu Microsoft 365](https://portal.office.com/adminportal/home) s přihlašovacími údaji globálního správce a nainstalujte Microsoft 365 pro firmy provedením následujících kroků. 
  
1. [Předpoklady pro ochranu dat na zařízeních s Microsoft 365 pro firmy](pre-requisites-for-data-protection.md)
    
    Nejdřív si přečtěte předpoklady, abyste měli jistotu, že vaše zařízení jsou připravená pro Microsoft 365 pro firmy.
    
2. [Nastavení Microsoft 365 pro firmy pomocí Průvodce nastavením](set-up.md)
    
    Pokud **trvale přesouváte z místního adresáře Active Directory do cloudu**, můžete přejít do centra pro správu Microsoft 365 a pomocí Průvodce nastavením ručně přidat uživatele nebo můžete provést jednorázovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte taky Exchange 2010, Exchange 2013 nebo Exchange 2016 Server, můžete [pomocí minimálního hybridu rychle migrovat poštovní schránky Exchange do microsoftu 365](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). Minimální hybridní kroky zahrnují jednorázovou synchronizaci uživatelů s Azure AD a migraci e-mailů z místního do cloudu. Po dokončení migrace e-mailu se synchronizace adresářů automaticky vypne, když tuto metodu použijete.
    
    - Pomocí Průvodce synchronizací adresářů synchronizujte uživatele s cloudem. Postupujte podle pokynů v tématu [Nastavení synchronizace adresářů pro Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) k dokončení tohoto procesu. Po synchronizaci uživatelů s cloudem musíte vypnout [synchronizaci adresářů pro Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization).
    
    Musíte také udělit každému uživateli, který tento způsob přidal, licenci na Microsoft 365 pro firmy. To můžete udělat v [Průvodci nastavením](set-up.md) nebo můžete [přiřazovat licence uživatelům](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů v tématu [nastavení mobilních zařízení pro uživatele Microsoft 365 pro firmy](set-up-mobile-devices.md) pro instalaci aplikací Office na zařízení a ujistěte se, že jsou chráněné Microsoft 365 pro firmy. 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítačů

Správci můžou pro nové počítače s Windows 10 vybrat nastavení pomocí [autopilota Windows](add-autopilot-devices-and-profile.md). Uživatelé můžou nastavit svoje stávající nebo nová zařízení s Windows 10 Podle pokynů v tomto tématu: [Nastavení počítačů s Windows pro uživatele Microsoft 365 pro firmy](set-up-windows-devices.md). V případě existujících zařízení můžou uživatelé **volitelně** [přesunout soubory na OneDrive pro firmy](move-files-to-onedrive.md). Mohou také pomocí nástrojů třetích stran přesouvat soubory spojené s profilem systému Windows na OneDrive.
  
Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 pro firmy tak, aby chránil vaše zařízení s Windows 10, a přitom pořád udržuje přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle kroků uvedených v tématu [Povolení zařízení s Windows 10 připojenými k doméně, která budou spravována Microsoft 365 pro firmy](manage-windows-devices.md) . Tato metoda je upřednostňovaná a zařízení v tomto stavu se nazývají **hybridní zařízení připojení Azure AD**. 
  
Pokud zachováte místní službu Active Directory, která obsahuje některé místní prostředky (jako jsou například sdílené soubory a tiskárny), můžete přístup k těmto prostředkům v **zařízení Azure AD – spojené s AD-joinovat** takto: [přístup k místním prostředkům ze zařízení Azure AD-připojeno v Microsoft 365 pro firmy](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktování podpory

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako správce Microsoft 365 pro firmy máte přístup k naší týmu zákaznické podpory: ** [kontaktujte podporu pro firemní produkty – Nápověda pro správce](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Viz také

[Dokumentace a zdroje informací o Microsoft 365 pro firmy](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa microsoft 365 pro firmy](manage.md)[migrace do systému Microsoft 365 pro firmy](migrate-to-microsoft-365-business.md)

[Školicí kurzy pro Microsoft 365 for Business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
