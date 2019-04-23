---
title: Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Zjistěte, jak získat přístup k místním prostředkům jako obchodními apps, sdílených souborů a tiskáren ze služby Active Directory Azure připojené zařízení Windows 10.
ms.openlocfilehash: 212685bc229f519152e69b09d0a745bfac7a38cd
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276875"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business

Jakékoli zařízení Windows 10 je Azure Active Directory připojen bude mít přístup ke všem prostředkům cloudové, například aplikací sady Office 365 a Microsoft 365 Business může být chráněna. Umožňuje také přístup k prostředkům místního jako řádku obchodní (LOB) aplikací, sdílené soubory a tiskárny, je třeba provést synchronizaci služby Active Directory v prostorách Azure Active Directory pomocí [Azure AD připojit](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). V tématu [Úvod do správy zařízení v Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) Další informace. 
  
## <a name="run-azure-ad-connect"></a>Spustit Azure AD připojit

Postupujte takto Chcete-li povolit zařízení Azure AD, které jsou spojeny vaší organizaci získat přístup k prostředkům místního.
  
1. Synchronizace uživatelů, skupin a kontaktů z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresáře a Azure AD připojit jako popsané v [Nastavení synchronizace adresáře služeb Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po dokončení synchronizace adresáře, ujistěte se, že zařízení Windows 10 organizace jsou Azure AD, které jsou připojeny. Tento krok se provádí individuálně na každé zařízení Windows 10. Podrobnosti naleznete v tématu [Nastavení zařízení Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md) . 
    
3. Jakmile zařízení Windows 10 jsou spojeny Azure AD, každý uživatel by měl restartovat jejich zařízení a přihlášení pomocí svých pověření Microsoft 365 Business. Všechna zařízení budou mít nyní přístup k místním prostředkům také.
    
Žádné další kroky jsou požadovány k získání přístupu k místním, že zařízení připojené prostředky k Azure AD. Toto je vestavěné funkce, které jsou k dispozici v systému Windows 10. 
  
Pokud vaše organizace není připravena k nasazení v Azure AD připojen konfigurace zařízení popsané výše, zvažte nastavení [Konfigurace zařízení Joined hybridní Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Důležité informace při připojení zařízení Windows Azure AD

Jestliže používáte Azure AD připojit zařízení systému Windows, které bylo dříve připojeno k doméně nebo v pracovní skupině, je třeba zvážit následující omezení:
  
- Pokud se připojí zařízení Azure AD, vytvoří nového uživatele bez odkazování na existující profil. Chcete-li odstranit tento problém, profily nutné přenést ručně. Profil uživatele obsahuje informace jako oblíbené položky, místní soubory, nastavení prohlížeče, nastavení nabídky Start, atd. Nejlepším řešením je najít nástroj jiného výrobce mapovat existující soubory a nastavení do nového profilu
    
- Pokud zařízení používá objekty Zásady skupiny (GPO), některé objekty GPO nebude mít srovnatelné [Konfiguraci poskytovatele služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) pro Intune. Spusťte [nástroj MMAT](https://www.microsoft.com/download/details.aspx?id=45520) najít srovnatelné CSP pro existující objekty zásad skupiny. 
    
- Uživatelé nebudou moci přihlásit k aplikacím, které závisí na ověřování služby Active Directory. Které se zabývají vyhodnotit pomocí starší verze aplikace a aktualizujte aplikaci používající moderní ověřování, pokud je to možné.
    
- Active Directory tiskárny zjišťování nebude fungovat. Tento problém lze vyřešit, poskytují přímé tiskárny cesty pro všechny uživatele nebo využít [Hybridní Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
    

