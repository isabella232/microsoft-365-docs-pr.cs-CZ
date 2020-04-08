---
title: Přístup k místním prostředkům ze zařízení s azure a d-up v Microsoftu 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Zjistěte, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny z Azure Active Directory, které se připojilo k zařízení s Windows 10.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 053d42480d8aa3792ecb0027ddd53d383a029474
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/07/2020
ms.locfileid: "41593227"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Přístup k místním prostředkům ze zařízení s azure a d-up v Microsoftu 365 Business

Každé zařízení s Windows 10, které je připojenou službou Azure Active Directory, má přístup ke všem cloudovým prostředkům, jako jsou vaše aplikace Office 365, a může být chráněno Microsoftem 365 Business. Můžete také povolit přístup k místním prostředkům, jako jsou obchodní aplikace , sdílené složky a tiskárny. Chcete-li povolit přístup, použijte [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místní služby Active Directory s Azure Active Directory. 

Další informace najdete [v tématu Úvod ke správě zařízení ve službě Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Kroky jsou také shrnuty v následujících částech.

> [!IMPORTANT]
> Tento postup se vztahuje pouze na oauth a NTLM. Protokol Kerberos není podporován.
 
## <a name="run-azure-ad-connect"></a>Spuštění služby Azure AD Connect

Pomocí následujících kroků povolte zařízením Azure AD vaší organizace přístup k místním prostředkům.
  
1. Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v části [Nastavení synchronizace adresářů pro Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Po dokončení synchronizace adresářů se ujistěte, že jsou připojená zařízení vaší organizace s Windows 10. Tento krok se provádí individuálně na každém zařízení s Windows 10. Podrobnosti najdete [v tématu Nastavení zařízení s Windows pro uživatele Microsoft 365 Business.](set-up-windows-devices.md) 
    
3. Jakmile jsou zařízení s Windows 10 připojena k Azure AD, každý uživatel musí restartovat svá zařízení a přihlásit se pomocí svých přihlašovacích údajů k Microsoft 365 Business. Všechna zařízení teď mají přístup i k místním prostředkům.
    
K získání přístupu k místním prostředkům pro zařízení připojená k Azure AD nejsou potřeba žádné další kroky. Tato funkce je integrována do systému Windows 10. 

Pokud máte v plánu se přihlásit k zařízení AADJ jiné než metoda hesla, jako je PIN / Bio-metric pomocí přihlašovacích údajů WHFB a pak přístup k místním zdrojům (akcie, tiskárny.. atd.), postupujte prosímhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Pokud vaše organizace není připravena k nasazení v konfiguraci zařízení připojil Azure AD popsané výše, zvažte nastavení [konfigurace zařízení připojení hybridní Azure AD](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Důležité informace o připojení zařízení s Windows do Azure AD

Pokud zařízení s Windows, ke kterému jste se připojili, bylo dříve připojeno k doméně nebo v pracovní skupině, zvažte následující omezení:
  
- Když se zařízení Azure AD připojí, vytvoří nového uživatele bez odkazování na existující profil. Profily musí být migrovány ručně. Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start. Nejlepším přístupem je najít nástroj jiného výrobce pro mapování existujících souborů a nastavení do nového profilu.

- Pokud zařízení používá objekty zásad skupiny (GPO), některé objekty zásad skupiny nemusí mít v Intune srovnatelného [zprostředkovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP). Spusťte [nástroj MMAT](https://www.microsoft.com/download/details.aspx?id=45520) a vyhledejte srovnatelné csp pro existující objekty zásad skupiny.

- Uživatelé nebudou moci ověřit, zda aplikace, které jsou závislé na ověřování služby Active Directory. Vyhodnoťte starší verzi aplikace a zvažte aktualizaci na aplikaci, která používá moderní auth, pokud je to možné.

- Zjišťování tiskárny služby Active Directory nebude fungovat. Můžete poskytnout přímé cesty tiskárny pro všechny uživatele nebo použít [hybridní cloudový tisk](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
