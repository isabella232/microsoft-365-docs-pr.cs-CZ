---
title: Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
description: Dozvíte se, jak získat přístup k prostorovým zdrojům, jako jsou například aplikace Business Apps, sdílení souborů a tiskárny z Azure Active Directory do zařízení Windows 10.
ms.openlocfilehash: 6065dd68bc8d306898ee02baa97fe07f71042439
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992243"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business

Jakékoli zařízení systému Windows 10, které je připojené ke službě Active Directory, bude mít přístup ke všem cloumovým prostředkům, jako je například aplikace sady Office 365, a mohou být chráněny společností Microsoft 365 Business. Chcete-li také povolit přístup k interaktivním prostředkům, jako jsou například aplikace Business (LOB), sdílení souborů a tiskárny, je nutné synchronizovat své prostory Active Directory s Azure Active Directory pomocí [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). 

Další informace naleznete [v tématu Úvod k nástroji Správa zařízení v Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .
Tyto kroky jsou také shrnuty v následujících oddílech.

## <a name="run-azure-ad-connect"></a>Spustit Azure AD Connect

Chcete-li umožnit přístup k prostředkům v rámci podniku, proveďte následující kroky, které umožní připojení k zařízením Azure AD vaší organizace.
  
1. Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře Active Directory na Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po dokončení synchronizace adresářů se přesvědčte, zda jsou zařízení systému Windows 10 v organizaci připojena k programu Azure AD. Tento krok se provádí jednotlivě na každém zařízení se systémem Windows 10. Podrobnosti naleznete v části [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md) . 
    
3. Jakmile se zařízení se systémem Windows 10 připojí k programu Azure AD, měli by každý uživatel restartovat svá zařízení a přihlásit se pomocí svých obchodních pověření společnosti Microsoft 365. Všechna zařízení budou mít nyní přístup i k prostředkům na místě.
    
K získání přístupu k prostředkům na místě pro zařízení spojená s Azure AD nejsou zapotřebí žádné další kroky. Toto je vestavěná funkce dostupná v systému Windows 10. 
  
Pokud vaše organizace není připravena k nasazení ve výše popsané konfiguraci zařízení Azure AD, zvažte nastavení [Konfigurace zařízení připojené k hybridní síti Azure](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Důležité informace o připojení zařízení systému Windows k Azure AD

Pokud jste Azure AD, který se připojuje k zařízení systému Windows, které bylo dříve součástí domény nebo pracovní skupiny, je třeba zvážit následující omezení:
  
- Když se zařízení připojí k Azure AD, vytvoří nového uživatele bez odkazu na existující profil. Chcete-li tento problém odstranit, je třeba profily ručně migrovat. Profil uživatele obsahuje informace jako oblíbené položky, místní soubory, nastavení prohlížeče, nastavení nabídky Start atd. Nejlepším přístupem je najít nástroj jiného výrobce pro mapování existujících souborů a nastavení na nový profil

- Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune obdobu [zprostředkovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP). Chcete-li vyhledat srovnatelné zprostředkovatele kryptografických služeb pro existující objekty GPO, spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .

- Uživatelé nebudou moci provádět ověření u aplikací, které závisejí na ověřování služby Active Directory. Chcete-li se vypořádat s tímto vyhodnotím pomocí starší aplikace a zvažte aktualizaci aplikace, která používá moderní ověřování, pokud je to možné.

- Zjišťování tiskárny služby Active Directory nebude funkční. Chcete-li tento problém vyřešit, zadejte přímé cesty k tiskárnám pro všechny uživatele nebo využijte [hybridní tisk shluku](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
