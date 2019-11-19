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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Naučte se nastavit aplikaci Microsoft 365 Business.
ms.openlocfilehash: f269e970cc1ee5ba7455ea799b238db577116f09
ms.sourcegitcommit: 38934a2115d5cdeb44c7484d57be07686c6f7720
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704109"
---
# <a name="get-started-with-microsoft-365-business"></a>Začínáme s Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co je Microsoft 365 Business

Microsoft 365 Business je komplexní sada nástrojů pro produktivitu práce a spolupráci, jako jsou aplikace Outlook, Word, Excel a další produkty sady Office, které jsou vždy aktuální. Své pracovní soubory můžete chránit na všech zařízeních iOS, Android a Windows 10 se zabezpečením podnikové kvality, které lze snadno spravovat.
  
Společnost Microsoft 365 Business je určena na 300 licencí. Potřebujete-li více licencí, vyhledejte další informace v dokumentaci k [produktu Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) . 
  
## <a name="get-microsoft-365-business"></a>Jak získat Microsoft 365 Business

- Pokud máte partnera, budou mít společnost Microsoft 365 Business: [získat microsoft 365 Business od společnosti Microsoft Partner Center](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 Business, můžete si ho [koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

 **Přehled sady Microsoft 365 Business Suite**
  
Následující diagram popisuje způsob, jakým správci nastavují aplikaci Microsoft 365 Business. Popisuje také kroky při přípravě počítačů s Windows na Microsoft 365 Business. Nová zařízení můžete také přidat v centru Microsoft 365 Business Admin Center pomocí [systému Windows AutoPilot](add-autopilot-devices-and-profile.md). Funkci AutoPilot můžete použít k nastavení a předkonfiguraci nových zařízení tak, aby byla připravena k produktivním využití, jakmile se uživatel přihlásí pomocí svých obchodních pověření společnosti Microsoft 365.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: nastavení aplikace Microsoft 365 Business (admin)

Přihlaste se ke [středisku microsoft 365 Business Admin Center](https://portal.office.com/adminportal/home) s globálními pověřeními pro správu a dokončete následující kroky pro nastavení služby Microsoft 365 Business. 
  
1. [Předpoklady pro ochranu dat u zařízení s aplikací Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte předpoklady, abyste se ujistili, že zařízení jsou připravena pro Microsoft 365 Business.
    
2. [Pomocí Průvodce instalací můžete nastavit aplikaci Microsoft 365 Business](set-up.md)
    
    Pokud **trvale přesouváte z místního adresáře služby Active Directory do mraku**, můžete přejít do centra pro správu Microsoft 365 Business admin a pomocí Průvodce nastavením přidat uživatele ručně, nebo můžete provést jednočasovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
    - Pokud máte také server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete [pomocí minimálního hybridního systému rychle migrovat poštovní schránky serveru Exchange do sady Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Minimální hybridní kroky zahrnují jednočasovou synchronizaci uživatelů s Azure AD a přenos e-mailů z prostoru na mrak. Po dokončení přenesení e-mailu je synchronizace adresářů při použití této metody automaticky vypnuta.
    
    - Pomocí Průvodce synchronizací adresářů sady Office 365 můžete uživatele synchronizovat s mrakem. K dokončení tohoto procesu použijte postup, který je popsaný v článku [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po synchronizaci uživatelů s mrakem bude nutné vypnout [synchronizaci adresářů pro sadu Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Bude také nutné přidělit každému uživateli, který byl tímto způsobem přidán, licenci společnosti Microsoft 365 Business. To lze provést v [Průvodci instalací](set-up.md) nebo můžete [přiřadit licence uživatelům sady Office 365 pro podniky](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů v [nastavení mobilních zařízení pro aplikaci microsoft 365 obchodní uživatelé](set-up-mobile-devices.md) k instalaci aplikací sady Office do zařízení a ujistěte se, že jsou chráněny společností Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: připravit počítače

Správci mohou pomocí [systému Windows AutoPilot](add-autopilot-devices-and-profile.md)předem vybrat nastavení pro nové počítače se systémem Windows 10. Uživatelé mohou vytvořit svá stávající nebo nová zařízení systému Windows 10 podle kroků v tomto tématu: [Nastavení počítačů se systémem Windows pro aplikaci Microsoft 365 Business Users](set-up-windows-devices.md). U existujících zařízení mohou uživatelé **volitelně** [přesunout soubory do zóny pro obchod](move-files-to-onedrive.md). Mohou také používat nástroje jiných výrobců k přesunu souborů přidružených k profilu systému Windows do funkce OneDrive.
  
Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle kroků, [které umožňují, aby zařízení systému Windows 10 spojená s doménou byla spravována společností Microsoft 365 Business](manage-windows-devices.md) . Tato metoda je upřednostňována a zařízení v tomto stavu se nazývají " **Hybrid Azure-spojené zařízení**". 
  
Pokud zachováte místní adresář služby Active Directory, který bude obsahovat některé z místních zdrojů (například sdílené položky a tiskárny), můžete k těmto zdrojům poskytnout přístup k těmto prostředkům pomocí technologie **Azure AD** , a to následujícím postupem: [přístup k místním prostředkům z zařízení PŘIPOJENÉM Azure ad v Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontaktujte podporu.

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako společnost Microsoft 365 Business admin máte přístup k našemu týmu zákaznické podpory: ** [kontaktování podpory pro obchodní produkty-Nápověda pro správce](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Související témata
[Dokumentace a zdroje informací k Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoft 365 Business](manage.md)[Migrace na Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

