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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dozvíte se, jak získat přístup k prostorovým zdrojům, jako je například obchodní aplikace, sdílení souborů a tiskárny z Azure Active Directory do zařízení Windows 10.
ms.openlocfilehash: fdc1eca6913ba6af4f6b65691fdee2165e7c827e
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323389"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business

Všechna zařízení systému Windows 10, která jsou připojena ke službě Active Directory, mají přístup ke všem prostředkům založeným na cloudu, jako jsou například aplikace sady Office 365, a může být chráněna společností Microsoft 365 Business. Můžete také povolit přístup k interním zdrojům, jako jsou obchodní aplikace (LOB), sdílení souborů a tiskárny. Chcete-li umožnit přístup, použijte [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci svých prostor služby Active Directory s Azure Active Directory. 

Další informace naleznete v tématu [Úvod k správě zařízení v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Tyto kroky jsou také shrnuty v následujících oddílech.

## <a name="run-azure-ad-connect"></a>Spustit Azure AD Connect

Chcete-li umožnit přístup k prostředkům v rámci podniku, proveďte následující kroky, které umožní připojení k zařízením Azure AD vaší organizace.
  
1. Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů a funkci Azure AD Connect, jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po dokončení synchronizace adresářů se přesvědčte, zda jsou zařízení systému Windows 10 v organizaci připojena k programu Azure AD. Tento krok se provádí jednotlivě na každém zařízení se systémem Windows 10. Podrobnosti naleznete v části [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md) . 
    
3. Jakmile jsou zařízení se systémem Windows 10 připojena k serveru Azure AD, musí každý uživatel restartovat svá zařízení a přihlásit se pomocí svých obchodních pověření společnosti Microsoft 365. Všechna zařízení mají nyní přístup i k prostředkům na místě.
    
K získání přístupu k prostředkům na místě pro zařízení spojená s Azure AD nejsou zapotřebí žádné další kroky. Tato funkce je integrována do systému Windows 10. 
  
Pokud vaše organizace není připravena k nasazení ve výše popsané konfiguraci zařízení Azure AD, zvažte nastavení [Konfigurace zařízení připojené k hybridní síti Azure](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Důležité informace o spojení zařízení se systémem Windows s Azure AD

Pokud se zařízení systému Windows, které jste připojili Azure-AD, dříve připojilo k doméně nebo v pracovní skupině, zvažte následující omezení:
  
- Když se zařízení připojí k Azure AD, vytvoří nového uživatele bez odkazu na existující profil. Profily je nutné migrovat ručně. Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepším přístupem je najít nástroj jiného výrobce pro mapování existujících souborů a nastavení na nový profil.

- Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune obdobu [zprostředkovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP). Chcete-li vyhledat srovnatelné zprostředkovatele kryptografických služeb pro existující objekty GPO, spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .

- Uživatelé nebudou moci provádět ověření u aplikací, které závisejí na ověřování služby Active Directory. Vyhodnoťte starší verzi aplikace a zvažte aktualizaci aplikace, která používá moderní ověřování, pokud je to možné.

- Zjišťování tiskárny služby Active Directory nebude fungovat. Můžete poskytnout přímé cesty k tiskárnám pro všechny uživatele nebo použít [hybridní shluk tisku](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
