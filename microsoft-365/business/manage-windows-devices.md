---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dozvíte se, jak povolit aplikaci Microsoft 365 chránit místní služby AD připojené k zařízením Windows 10.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992223"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Tuto možnost můžete nastavit tak, že nejprve synchronizujete službu Active Directory s Azure Active Directory a poté zaregistrujete zařízení systému Windows 10 s Azure AD a nastavíte je pro správu mobilních zařízení společností Microsoft 365 Business.
Následující video podrobně popisuje postup nastavení tohoto postupu pro nejběžnější scénář.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Nastavení zařízení připojených k doméně, která budou spravována společností Microsoft 365 Business

Chcete-li nastavit zařízení spojená s doménou organizace tak, aby měla užitek z možností poskytovaných službou Active Directory společnosti Azure, můžete kromě prostředí služby Active Directory implementovat také zařízení, která byla připojena k objektu **Hybrid Azure**. Jedná se o zařízení, která jsou připojena k vaší budově v prostředí Active Directory a k Azure Active Directory. Tato zařízení mohou být chráněna a spravována společností Microsoft 365 Business. 
  
Dokončete následující kroky a vytvořte tak zařízení Windows 10 Hybrid Azure AD a spravováno společností Microsoft 365 Business.
  
1. Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře služby Active Directory na Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure (Active Directory Connect), jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Postup je pro společnost Microsoft 365 Business zcela stejný. 
  
2. Než dokončíte krok 3 a povolíte, aby zařízení Windows 10 byla připojena k hybridním Azure, musíte zajistit splnění následujících předpokladů:

   - Používáte nejnovější verzi připojení k programu Azure AD.

   - Azure AD Connect synchronizovalo všechny počítačové objekty zařízení, které chcete použít jako hybridní Azure AD. Pokud objekty počítače patří do určitých organizačních jednotek, zkontrolujte, zda jsou tyto organizační jednotky nastaveny pro synchronizaci také v Azure AD Connect.
    
3. Registrovat existující domény spojené se systémem Windows 10 na hybridní Azure AD vstoupil a zapsat je pro správu mobilních zařízení společností Intune (Microsoft 365 Business):
    
4. Postupujte podle podrobných pokynů pro [konfiguraci hybridních zařízení připojených ke službě Active Directory](https://go.microsoft.com/fwlink/p/?linkid=872870). Tím umožníte synchronizaci v prostředí služby Active Directory s počítači se systémem Windows 10 a nastavíte jejich připravenost na mraky.
    
5. Chcete-li zapsat zařízení systému Windows 10 pro správu mobilních zařízení, naleznete pokyny v části [zápis zařízení Windows 10 s Intune pomocí zásad skupiny](https://go.microsoft.com/fwlink/p/?linkid=872871) . Zásady skupiny lze nastavit na úrovni místního počítače nebo hromadných operací, na serveru řadiče domény je možné vytvořit toto nastavení zásad skupiny.