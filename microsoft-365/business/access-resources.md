---
title: Přístup k místním prostředkům ze zařízení Azure AD-JOIN v Microsoft 365 Business
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Přečtěte si, jak získat přístup k místním prostředkům, jako je podnikový podnik, sdílení souborů a tiskárny ze zařízení Azure Active Directory spojené s Windows 10.
ms.openlocfilehash: 22edf0c23d6318e1f70bcb21b2cd697ea0a75da4
ms.sourcegitcommit: 849b365bd3eaa9f3c3a9ef9f5973ef81af9156fa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/16/2020
ms.locfileid: "49688227"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Přístup k místním prostředkům ze zařízení Azure AD-JOIN v Microsoft 365 Business Premium

Tento článek se týká Microsoft 365 Business Premium.

Všechna zařízení s Windows 10, která jsou spojená se službou Azure Active Directory, mají přístup ke všem cloudovým prostředkům, jako jsou aplikace Microsoft 365 a mohou být chráněny Microsoft 365 Business Premium. Můžete taky povolit přístup k místním prostředkům, jako jsou podnikové aplikace (LOB), sdílené soubory a tiskárny. Pokud chcete povolit přístup, použijte [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místního adresáře Active Directory s Azure Active Directory. 

Další informace najdete v tématu [Úvod do správy zařízení v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Tento postup je také shrnut v následujících částech.
 
## <a name="run-azure-ad-connect"></a>Spuštění služby Azure AD Connect

Provedením následujících kroků povolíte zařízením připojeným k Azure AD v organizaci přístup k místním prostředkům.
  
1. Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect způsobem popsaným v části [Nastavení synchronizace adresářů pro Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).
    
2. Po dokončení synchronizace adresáře zkontrolujte, jestli jsou zařízení s Windows 10 ve vaší organizaci v Azure AD spojená. Tento krok se provádí jednotlivě na každém zařízení s Windows 10. Podrobnosti najdete v tématu [nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md) . 
    
3. Jakmile se zařízení s Windows 10 připojí ke službě Azure AD, musí každý uživatel restartovat svoje zařízení a přihlásit se pomocí přihlašovacích údajů k Microsoft 365 Business Premium. Všechna zařízení mají teď taky přístup k místním prostředkům.
    
K získání přístupu k místním prostředkům pro zařízení s připojením Azure AD nejsou potřeba žádné další kroky. Tato funkce je integrovaná ve Windows 10. 

Pokud máte plány pro přihlášení k zařízení AADJ, jako je třeba PIN/bio-metric prostřednictvím WHFB přihlašovacích údajů, a pak přístup k místním prostředkům (sdílené položky, tiskárny.. atd.), postupujte https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Pokud vaše organizace není připravená k nasazení v konfiguraci zařízení spojené s připojením k Azure AD, zvažte nastavení [Konfigurace hybridního zařízení se službou Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Důležité informace o připojení zařízení se systémem Windows k Azure AD

Pokud bylo zařízení se systémem Windows, které jste připojili prostřednictvím služby Azure-AD dřív v doméně, nebo v pracovní skupině, zvažte následující omezení:
  
- Když se zařízení Azure AD spojuje, vytvoří nového uživatele bez odkazu na existující profil. Profily je nutné migrovat ručně. Profil uživatele obsahuje informace, jako jsou oblíbené, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepším postupem je vyhledání nástroje třetí strany pro mapování existujících souborů a nastavení na nový profil.

- Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune srovnatelného [poskytovatele služeb pro konfiguraci](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) . K vyhledání srovnatelných CSP pro existující objekty GPO spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .

- Uživatelé nebudou moct ověřovat v aplikaci, která závisí na ověřování služby Active Directory. Vyhodnoťte starší verzi aplikace a zvažte aktualizaci aplikace používající moderní ověřování, pokud je to možné.

- Vyhledávání tiskáren Active Directory nefunguje. Můžete poskytnout přímé tiskové cesty pro všechny uživatele nebo použít [univerzální tisk](https://aka.ms/UPDocs).
