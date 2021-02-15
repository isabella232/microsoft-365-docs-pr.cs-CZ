---
title: Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business
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
description: Zjistěte, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny, ze zařízení s Windows 10 připojeném k Azure Active Directory.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233834"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business Premium

Tento článek se týká Microsoftu 365 Business Premium.

Každé zařízení s Windows 10, ke které je připojená služba Azure Active Directory, má přístup ke všem cloudovým prostředkům, jako jsou vaše aplikace Microsoft 365, a může je chránit microsoft 365 Business Premium. Můžete taky povolit přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky souborů a tiskárny. Pokud chcete povolit přístup, [použijte Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místní služby Active Directory s Azure Active Directory. 

Další informace najdete v článku [Úvod ke správě zařízení v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
Kroky jsou shrnuty i v následujících částech.
 
## <a name="run-azure-ad-connect"></a>Spuštění služby Azure AD Connect

Následujícím postupem povolíte zařízením připojeným k Azure AD vaší organizace přístup k místním prostředkům.
  
1. Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, spusťte průvodce synchronizací adresářů a Azure AD Connect podle popisu v části Nastavení synchronizace adresářů pro [Office 365.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)
    
2. Po dokončení synchronizace adresářů se ujistěte, že jsou zařízení s Windows 10 ve vaší organizaci připojená ke službě Azure AD. Tento krok se provádí jednotlivě na každém zařízení s Windows 10. Podrobnosti najdete v článku Nastavení zařízení s Windows pro uživatele [Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
3. Jakmile jsou zařízení s Windows 10 připojená ke službě Azure AD, musí každý uživatel svoje zařízení restartovat a přihlásit se pomocí svých přihlašovacích údajů Microsoft 365 Business Premium. Všechna zařízení teď mají přístup i k místním prostředkům.
    
K získání přístupu k místním prostředkům pro zařízení připojená k Azure AD není potřeba žádné další kroky. Tato funkce je součástí Windows 10. 

Pokud máte v plánu přihlásit se k jinému zařízení AADJ než k metodě hesla, jako je třeba PIN kód nebo biometrická metrika, pomocí přihlášení pomocí přihlašovacích údajů WHFB, a pak budete mít přístup k místním prostředkům (sdílené složky, tiskárny). atd.), postupujte prosím podle https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Pokud vaše organizace není připravená k nasazení v konfiguraci zařízení připojené k Azure AD popsané výše, zvažte nastavení konfigurace zařízení připojeného k hybridní službě [Azure AD.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Co byste měli zvážit, když připojíte zařízení s Windows k Azure AD

Pokud bylo zařízení s Windows, ke které jste připojili službu Azure-AD, dřív připojeno k doméně nebo v pracovní skupině, zvažte následující omezení:
  
- Když se zařízení připojí k Azure AD, vytvoří nového uživatele bez odkazování na existující profil. Profily je nutné migrovat ručně. Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepší řešení je najít nástroj třetí strany, který namapuje existující soubory a nastavení na nový profil.

- Pokud zařízení používá objekty Zásady skupiny ( GPO), nemusí některé [](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) gpOs mít v Intune srovnatelně poskytovatele konfiguračních služeb (CSP). Spuštěním nástroje [MMAT najdete](https://www.microsoft.com/download/details.aspx?id=45520) srovnatelné csP pro stávající GPOS.

- Uživatelé nemusí být schopni ověření v aplikacích, které jsou závislé na ověřování služby Active Directory. Vyhodnoťte starší aplikaci a zvažte možnost aktualizace na aplikaci, která používá moderní ověřování (pokud je to možné).

- Zjišťování tiskárny ve službě Active Directory nebude fungovat. Můžete poskytnout přímé cesty k tiskárně všem uživatelům nebo použít univerzální [tisk.](https://aka.ms/UPDocs)
