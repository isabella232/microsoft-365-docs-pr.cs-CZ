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
description: Zjistěte, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny z zařízení s Windows 10 připojeného k Azure Active Directory.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445342"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business Premium

Tento článek se týká Microsoft 365 Business Premium.

Všechna zařízení s Windows 10, ke které je připojená služba Azure Active Directory, má přístup ke všem cloudovým prostředkům, jako jsou vaše aplikace Microsoft 365, a může být chráněno službou Microsoft 365 Business Premium. Můžete také povolit přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky souborů a tiskárny. Pokud chcete povolit přístup, [použijte Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místní služby Active Directory s Azure Active Directory. 

Další informace najdete v tématu [Úvod ke správě zařízení v Azure Active Directory](/azure/active-directory/device-management-introduction).
Tyto kroky jsou také shrnuty v následujících částech.
 
## <a name="run-azure-ad-connect"></a>Spuštění služby Azure AD Connect

Proveďte následující kroky, abyste zařízením připojeným k Azure AD vaší organizace umožnili přístup k místním prostředkům.
  
1. Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v článku Nastavení synchronizace adresářů pro [Office 365.](../enterprise/set-up-directory-synchronization.md)
    
2. Po dokončení synchronizace adresářů se ujistěte, že jsou zařízení s Windows 10 vaší organizace připojená k Azure AD. Tento krok se provádí jednotlivě na každém zařízení s Windows 10. Podrobnosti najdete v tématu Nastavení zařízení s Windows pro [uživatele Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
3. Jakmile jsou zařízení s Windows 10 připojená k Azure AD, musí každý uživatel restartovat svá zařízení a přihlásit se pomocí přihlašovacích údajů Microsoft 365 Business Premium. Všechna zařízení teď mají přístup i k místním prostředkům.
    
K získání přístupu k místním prostředkům pro zařízení připojená k Azure AD nejsou potřeba žádné další kroky. Tato funkce je integrovaná ve Windows 10. 

Pokud máte v plánu přihlásit se k jinému zařízení AADJ, než je metoda hesla, třeba PIN/Biometric přes přihlašovací údaje WHFB, a pak získat přístup k místním prostředkům (sdílené složky, tiskárny.). atd.), postupujte podle https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Pokud vaše organizace není připravená nasadit v konfiguraci zařízení připojené k Azure AD popsané výše, zvažte nastavení konfigurace zařízení připojeného k hybridní službě [Azure AD.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Důležité informace při připojení zařízení s Windows k Azure AD

Pokud zařízení s Windows, ke které jste připojili Azure-AD, bylo dříve připojené k doméně nebo v pracovní skupině, zvažte následující omezení:
  
- Když se zařízení Azure AD připojí, vytvoří nového uživatele bez odkazu na existující profil. Profily se musí migrovat ručně. Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepším přístupem je najít nástroj jiného výrobce, který namapuje existující soubory a nastavení na nový profil.

- Pokud zařízení používá objekty Zásady skupiny (GPO), nemusí některé objekty zásad skupiny v Intune mít srovnatelného poskytovatele služeb konfigurace. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Spusťte nástroj [MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) abyste našli srovnatelné csP pro stávající objekty zásad skupiny.

- Uživatelé nemusí být schopni ověřit aplikace, které jsou závislé na ověřování služby Active Directory. Vyhodnoťte starší aplikaci a zvažte aktualizaci na aplikaci, která používá moderní ověřování, pokud je to možné.

- Zjišťování tiskárny ve službě Active Directory nebude fungovat. Můžete zadat přímé cesty tiskárny pro všechny uživatele nebo použít [Univerzální tisk](/universal-print/).

### <a name="related-articles"></a>Související články

[Předpoklady pro Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
