---
title: Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Zjistěte, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny z Azure Active Directory připojeného Windows 10 zařízení.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843316"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business Premium

Tento článek se týká Microsoft 365 Business Premium.

Každé Windows 10 zařízení, které je Azure Active Directory připojené, má přístup ke všem cloudovým prostředkům, jako jsou vaše aplikace Microsoft 365, a může být chráněno Microsoft 365 Business Premium. Můžete také povolit přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky souborů a tiskárny. Pokud chcete povolit přístup, použijte [Azure AD Připojení](/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místního adresáře Active Directory s Azure Active Directory.

Další informace najdete v tématu [Úvod ke správě zařízení v Azure Active Directory](/azure/active-directory/device-management-introduction).
Tyto kroky jsou také shrnuty v následujících částech.

## <a name="run-azure-ad-connect"></a>Spuštění služby Azure AD Připojení

Proveďte následující kroky, abyste zařízením připojeným k Azure AD vaší organizace umožnili přístup k místním prostředkům.

1. Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Připojení, jak je popsáno v článku Nastavení synchronizace adresářů pro [Office 365](../enterprise/set-up-directory-synchronization.md).

2. Po dokončení synchronizace adresářů se ujistěte, že jsou vaše Windows 10 připojená k Azure AD. Tento krok se provádí jednotlivě na každém Windows 10 zařízení. Podrobnosti [najdete v Windows zařízení pro Microsoft 365 Business Premium uživatele.](set-up-windows-devices.md)

3. Jakmile jsou Windows 10 připojená k Azure AD, musí každý uživatel restartovat svá zařízení a přihlásit se pomocí svých přihlašovacích Microsoft 365 Business Premium přihlašovacích údajů. Všechna zařízení teď mají přístup i k místním prostředkům.

K získání přístupu k místním prostředkům pro zařízení připojená k Azure AD nejsou potřeba žádné další kroky. Tato funkce je integrovaná v Windows 10.

Pokud máte v plánu přihlásit se k jinému zařízení AADJ než k metodě hesla, jako je PIN/Biometric přes přihlašovací údaje WHFB, a pak získat přístup k místním prostředkům (sdílené složky, tiskárny atd.), postupujte podle tohoto [článku.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

Pokud vaše organizace není připravená nasadit v konfiguraci zařízení připojené k Azure AD popsané výše, zvažte nastavení konfigurace zařízení připojeného k hybridní službě [Azure AD.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Důležité informace při připojení Windows k Azure AD

Pokud Windows zařízení, ke které jste připojili Azure-AD, dřív připojené k doméně nebo v pracovní skupině, zvažte následující omezení:

- Když se zařízení Azure AD připojí, vytvoří nového uživatele bez odkazu na existující profil. Profily se musí migrovat ručně. Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepším přístupem je najít nástroj jiného výrobce, který namapuje existující soubory a nastavení na nový profil.

- Pokud zařízení používá objekty Zásady skupiny (GPO), nemusí některé objekty zásad skupiny v Intune mít srovnatelného poskytovatele služeb konfigurace. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Spusťte nástroj [MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) abyste našli srovnatelné csP pro stávající objekty zásad skupiny.

- Uživatelé nemusí být schopni ověřit aplikace, které jsou závislé na ověřování služby Active Directory. Vyhodnoťte starší aplikaci a zvažte aktualizaci na aplikaci, která používá moderní ověřování, pokud je to možné.

- Zjišťování tiskárny ve službě Active Directory nebude fungovat. Můžete zadat přímé cesty tiskárny pro všechny uživatele nebo použít [Univerzální tisk](/universal-print/).

### <a name="related-articles"></a>Související články

[Předpoklady pro Azure AD Připojení](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
