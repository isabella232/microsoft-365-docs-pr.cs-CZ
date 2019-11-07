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
ms.openlocfilehash: 4c744d6a900dba3c11ee51e75602a430268e15bb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/07/2019
ms.locfileid: "38029098"
---
# <a name="get-started-with-microsoft-365-business"></a>Začínáme s Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Co je Microsoft 365 Business

Microsoft 365 Business je komplexní sada nástrojů zaměřených na produktivitu firmy a spolupráci, do které například patří vždy aktuální Outlook, Word, Excel a další produkty Office. Pracovní soubory můžete chránit na všech zařízeních s iOSem, Androidem a Windows 10. Umožňuje to zabezpečení na podnikové úrovni s jednoduchou správou.
  
Microsoft 365 Business umožňuje používat maximálně 300 licencí. Pokud potřebujete více licencí, podívejte se na dokumentaci k [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986), kde získáte více informací. 
  
## <a name="get-microsoft-365-business"></a>Jak získat Microsoft 365 Business

- Pokud máte partnera, získá partner Microsoft 365 Business: [Jak získat Microsoft 365 Business z partnerského centra Microsoftu](get-microsoft-365-business.md).
    
- Pokud nemáte partnera a chcete získat Microsoft 365 Business, můžete si ho [koupit tady](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

 **Přehled sady Microsoft 365 Business Suite**
  
Následující diagram popisuje způsob, jakým správci nastavují aplikaci Microsoft 365 Business. Popisuje také kroky při přípravě počítačů s Windows na Microsoft 365 Business. Nová zařízení také můžete přidat v Centru pro správu Microsoft 365 Business s použitím [Windows AutoPilota](add-autopilot-devices-and-profile.md). Pomocí AutoPilota také můžete nastavit a předběžně nakonfigurovat nová zařízení, aby byla připravená k použití hned, jak se uživatel přihlásí pomocí přihlašovacích údajů služby Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: nastavení aplikace Microsoft 365 Business (admin)

Přihlaste se do [Centra pro správu Microsoft 365 Business](https://portal.office.com/adminportal/home) pod přihlašovacími údaji globálního správce a nastavte Microsoft 365 Business podle následujících pokynů. 
  
1. [Předpoklady pro ochranu dat na zařízeních s Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Nejprve si přečtěte předpoklady, abyste měli jistotu, že vaše zařízení jsou na Microsoft 365 Business připravená.
    
2. [Nastavení Microsoft 365 Business pomocí průvodce nastavením](set-up.md)
    
    Pokud **trvale přesouváte z místního adresáře služby Active Directory do shluku**, můžete uživatele přidat ručně do centra Business admin v aplikaci Microsoft 365 pomocí Průvodce nastavením nebo můžete provést jednočasovou synchronizaci s Azure AD Connect. Můžete to udělat dvěma způsoby: 
    
  - Pokud máte také server Exchange 2010, Exchange 2013 nebo Exchange 2016, můžete [pomocí minimálního hybridního systému rychle migrovat poštovní schránky serveru Exchange do sady Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). Kroky minimálních hybridních možností zahrnují jednorázovou synchronizaci uživatelů do Azure AD a zároveň přesun e-mailů z místního úložiště do cloudu. Po dokončení přesunu e-mailů se u této metody synchronizace adresářů automaticky vypne.
    
  - K synchronizaci uživatelů s cloudem můžete použít průvodce synchronizací adresářů Office 365. K dokončení tohoto procesu použijte postup, který je popsaný v článku [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846). Po synchronizaci uživatelů s cloudem budete muset [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Každému uživateli přidanému tímto způsobem budete muset udělit licenci na Microsoft 365 Business. To lze provést v [Průvodci instalací](set-up.md)nebo v [licencích k přiřazení uživatelům sady Office 365 pro podniky](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Příprava mobilních zařízení

Postupujte podle pokynů v[nastavení mobilních zařízení pro aplikaci microsoft 365 obchodní uživatelé](set-up-mobile-devices.md) k instalaci aplikací sady Office do zařízení a k zajištění jejich ochrany společností Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: připravit počítače

Správci mohou předem vybrat nastavení pro nová zařízení Windows 10 počítačů pomocí [systému Windows AutoPilot](add-autopilot-devices-and-profile.md). Uživatelé mohou vytvořit svá stávající nebo nová zařízení systému Windows 10 podle kroků v tomto tématu: [Nastavení počítačů se systémem Windows pro aplikaci Microsoft 365 Business Users](set-up-windows-devices.md). U existujících zařízení mohou uživatelé také **volitelně**[přesunout soubory do zóny pro obchod](move-files-to-onedrive.md). Mohou také používat nástroje jiných výrobců k přesunu souborů přidružených k profilu systému Windows do funkce OneDrive.
  
Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle kroků, [které umožňují, aby zařízení systému Windows 10 spojená s doménou byla spravována společností Microsoft 365 Business](manage-windows-devices.md) . Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají " **Hybrid Azure-spojené zařízení**". 
  
Pokud zachováte místní adresář služby Active Directory, který bude obsahovat některé z místních zdrojů (například sdílené položky a tiskárny), můžete k těmto zdrojům poskytnout přístup k těmto prostředkům prostřednictvím **Azure** , a to následujícím postupem: přístup k [místním prostředkům z Zařízení připojené k Azure v aplikaci Microsoft 365 Business](access-resources.md).
  
Po instalaci systému Windows 10 počítačů můžete systém [Office automaticky nainstalovat](auto-install-or-uninstall-office.md) do zařízení. 
  
## <a name="contact-support"></a>Kontaktujte podporu.

 **Pokud potřebujete kontaktovat podporu:**
  
- Obraťte se na partnera.
    
- Jako společnost Microsoft 365 Business admin máte přístup k našemu týmu zákaznické podpory, ** [kontaktujte podporu pro obchodní produkty-Nápověda pro správce](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Příbuzná témata
[Dokumentace a zdroje informací k Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Správa Microsoft 365 Business](manage.md)[Migrace na Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

