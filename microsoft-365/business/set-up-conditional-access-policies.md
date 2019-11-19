---
title: Nastavení zásad podmíněného přístupu pro kampaně společnosti Microsoft 365
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Naučte se nastavit zásady podmíněného přístupu pro aplikaci Microsoft 365 kampaněmi.
ms.openlocfilehash: 0fccd103e3633c7fa5ac07c731341eee93059986
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715076"
---
# <a name="set-up-conditional-access-policies"></a>Nastavení zásad podmíněného přístupu

Zásady [podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidávají podstatné dodatečné zabezpečení. Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny všem zákazníkům. Zásady směrného plánu představují sadu předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky. Tyto běžné útoky mohou zahrnovat postřik hesla, přehrání a podvodné zprávy.

Tyto zásady vyžadují, aby správci a uživatelé zadávali při splnění určitých podmínek druhou formu ověřování (tzv. vícefaktorové ověřování nebo MFA). Pokud se například uživatel přihlašuje z jiné země, může být přihlášení považováno za rizikové a uživatel musí poskytnout další způsob ověřování. 

Zásady základní linie v současné době zahrnují následující:
- **Požadovat MFA pro** správce – vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správců, včetně globálního správce.
- **Ochrana koncového uživatele** – vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že je přihlášení riskantní. 
- **Blokovat starší ověřování** – starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější a ověřovací protokoly. Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí. Tato zásada blokuje přístup od klientů, kteří nepodporují podmíněný přístup. 
- **Vyžadují MFA pro správu servisu** – vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde se konfigurují základní zásady). 

Společnost Microsoft doporučuje povolit všechny tyto zásady základní linie. Po povolení těchto zásad budou správci a uživatelé vyzváni k zaregistrování pro ověřování Azure Multii-Factor.

Další informace o těchto zásadách naleznete v tématu [co jsou základní zásady](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Nastavení zásad směrného plánu

1. Přejděte na [portál Azure](https://portal.azure.com)a pak přejděte na Azure **podmíněný přístup** **služby Active Directory** \> .
    
    Základní zásady jsou uvedeny na stránce. <br/> <br/>
    ![Stránka se seznamem zásad základní úrovně pro podmíněný přístup.](media/baslinepolicies.png)
1. Pro jednotlivé zásady se podívejte na následující specifické pokyny:

  - [Vyžadovat MFA pro administrátoři](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vyžadovat MFA pro uživatele](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokovat starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vyžadovat MFA pro správu servisu](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Můžete nastavit mnoho dalších zásad, například vyžadování schválených klientských aplikací. Další informace naleznete v dokumentaci k [podmíněnému přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).
