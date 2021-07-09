---
title: Začínáme s Microsoft 365 pro firmy
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Přečtěte si Microsoft 365 pro firmy, jak ho nastavit a jak připravit zařízení a počítače uživatelů, aby se zajistilo, že jsou chráněná Microsoft 365 pro firmy.
ms.openlocfilehash: 2ab0079da7a8f30d481cdb3d3dc6d165b4a19e99
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339284"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Začínáme s Microsoft 365 pro firmy

## <a name="what-is-microsoft-365-for-business"></a>Co je Microsoft 365 pro firmy

Microsoft 365 pro firmy je komplexní sada nástrojů pro firemní produktivitu a spolupráci, jako jsou Outlook, Word, Excel a další produkty Office, které jsou vždy aktuální. Pracovní soubory můžete chránit na všech svých zařízeních s iOSem, Androidem a Windows 10 s podnikovým zabezpečením, které se snadno spravuje.

## <a name="watch-what-is-microsoft-365-business-premium"></a>Video: Co je Microsoft 365 Business Premium

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 pro firmy je určeno až pro 300 licencí. Pokud potřebujete více licencí, najdete další informace v dokumentaci k [Microsoftu 365 Enterprise](../enterprise/index.yml). 
  
## <a name="get-microsoft-365-for-business"></a>Získání Microsoft 365 pro firmy

- Pokud máte partnera, dostane Microsoft 365 pro firmy: Microsoft 365 pro firmy [z Partnerského centra Microsoftu](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 pro firmy, můžete si [ho koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Nastavení Microsoft 365 pro firmy

 **Přehled Microsoft 365 sady Office pro firmy**
  
Následující diagram popisuje, jak správci Microsoft 365 pro firmy. Popisuje také postup, jak připravit Windows počítače pro Microsoft 365 pro firmy. Můžete také přidat nová zařízení v Centrum pro správu Microsoftu 365 pomocí [Windows AutoPilota.](add-autopilot-devices-and-profile.md) AutoPilot můžete použít k nastavení a předběžné konfiguraci nových zařízení tak, aby byla připravená k produktivnímu použití, jakmile se uživatel přihlásí pomocí přihlašovacích údajů Microsoft 365 pro firmy.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

## <a name="watch-set-up-microsoft-365-business"></a>Přehrát: Nastavení Microsoft 365 firmy

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Nastavení Microsoft 365 pro firmy (správce)

Přihlaste se [k Centrum pro správu Microsoftu 365](https://admin.microsoft.com/adminportal/home) pomocí přihlašovacích údajů globálního správce a proveďte následující postup nastavení Microsoft 365 pro firmy. 
  
1. [Předpoklady pro ochranu dat na zařízeních s Microsoft 365 pro firmy](pre-requisites-for-data-protection.md)
    
    Nejdřív si přečtěte požadavky, abyste se ujistili, že jsou vaše zařízení připravená Microsoft 365 pro firmy.
    
2. [Použití průvodce nastavením k nastavení Microsoft 365 pro firmy](set-up.md)
    
    Pokud se trvale přesouváte z místní služby **Active Directory** do cloudu, můžete přejít na Centrum pro správu Microsoftu 365 a pomocí průvodce nastavením přidat uživatele ručně nebo můžete provést časovou synchronizaci s Azure AD Připojení. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte taky server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete pomocí minimálního hybridního nasazení rychle migrovat poštovní schránky Exchange do [Microsoft 365](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). K minimálním hybridním krokům patří časová synchronizace uživatelů s Azure AD a migrace e-mailu z místního do cloudu. Po dokončení migrace e-mailu se synchronizace adresářů automaticky vypne, když použijete tuto metodu.
    
    - Pomocí průvodce synchronizací adresářů synchronizujte uživatele s cloudem. Postupujte podle pokynů v části Nastavení [synchronizace adresářů pro Microsoft 365](../enterprise/set-up-directory-synchronization.md) tento proces dokončete. Po synchronizaci uživatelů s cloudem budete muset vypnout synchronizaci adresářů pro [Microsoft 365](../enterprise/turn-off-directory-synchronization.md).
    
    Budete také muset dát každému uživateli, který byl přidán tímto způsobem, licenci na Microsoft 365 pro firmy. Můžete to udělat v průvodci [nastavením](set-up.md) nebo můžete přiřadit [licence uživatelům](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Podle pokynů v části Nastavení mobilních zařízení pro [Microsoft 365](set-up-mobile-devices.md) pro firemní uživatele nainstalujte aplikace Office na zařízení Office ujistěte se, že jsou chráněná Microsoft 365 pro firmy. 
  
### <a name="3-prepare-pcs"></a>3: Příprava počítačů

Správci mohou předem vybrat nastavení pro nové Windows 10 počítače pomocí [Windows AutoPilota](add-autopilot-devices-and-profile.md). Uživatelé mohou nastavit stávající nebo nová Windows 10 zařízení podle pokynů v tomto tématu: Nastavení počítačů Windows počítačů pro [Microsoft 365 pro firemní uživatele](set-up-windows-devices.md). U stávajících zařízení mohou uživatelé **volitelně** [přesouvat soubory do OneDrive pro firmy](move-files-to-onedrive.md). K přesunutí souborů přidružených k profilu Windows jiných OneDrive.
  
Pokud vaše organizace používá místní Windows Server Active Directory, můžete nastavit Microsoft 365 pro firmy tak, aby chránila vaše zařízení Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle pokynů v části Povolení Windows 10 zařízení připojených k doméně, aby je Microsoft 365 [pro](manage-windows-devices.md) firmy nastavili. Tato metoda je upřednostňovaná a zařízení v tomto stavu se nazývají zařízení připojená **k Hybridní službě Azure AD**. 
  
Pokud si zachováte místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízením připojeným k **Azure AD** dát přístup k těmto prostředkům podle pokynů tady: Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 [pro firmy](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktování podpory

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako Microsoft 365 pro firemní správce máte přístup k našemu týmu zákaznické podpory: Kontaktování podpory pro **[firemní produkty - Nápověda pro správce](../business-video/get-help-support.md)**
    
## <a name="related-content"></a>Související obsah

[Microsoft 365 pro obchodní dokumentaci](./index.yml) a zdroje (stránka odkazu)\
[Správa Microsoft 365 pro firmy](manage.md) (článek)\
[Migrace na Microsoft 365 pro firmy](migrate-to-microsoft-365-business.md) (článek)\
[Microsoft 365 pro firemní školicí videa](../business-video/index.yml) (stránka odkazu)