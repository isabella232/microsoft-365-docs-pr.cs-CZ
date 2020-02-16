---
title: Nastavení zásad podmíněného přístupu pro kampaně Microsoft365
f1.keywords:
- NOCSH
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
description: Přečtěte si, jak nastavit zásady podmíněného přístupu pro kampaně Microsoft 365.
ms.openlocfilehash: 1ef90bd77da43ded624d85cef9c7a33beec74345
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064598"
---
# <a name="set-up-conditional-access-policies"></a>Nastavení zásad podmíněného přístupu

[Zásady podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidávají podstatné další zabezpečení. Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny pro všechny zákazníky. Zásady podle směrného plánu jsou sadou předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky. Tyto běžné útoky mohou zahrnovat sprej heslem, přehrání a phishing.

Tyto zásady vyžadují, aby správci a uživatelé zadali druhou formu ověřování (nazývané vícefaktorové ověřování nebo vícefaktorové ověřování), pokud jsou splněny určité podmínky. Pokud se například uživatel přihlašuje z jiné země, může být přihlášení považováno za rizikové a uživatel musí poskytnout další formu ověřování. 

V současné době zásady směrného plánu zahrnují následující:
- **Vyžadovat vícefaktorové** &ndash; ověřování pro správce Vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správce, včetně globálního správce.
- **Ochrana** &ndash; koncových uživatelů Vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že je přihlášení riskantní. 
- **Blokovat starší ověřování** &ndash; Starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější ověřovací protokoly. Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí. Tato zásada blokuje přístup klientům, kteří nepodporují podmíněný přístup. 
- **Vyžadovat vícefaktorové ověřování pro správu** &ndash; služeb Vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde nakonfigurujete zásady směrného plánu). 

Společnost Microsoft doporučuje povolit všechny tyto zásady směrného plánu. Po povolení těchto zásad budou správci a uživatelé vyzváni k registraci pro ověřování multiifaktoru Azure.

Další informace o těchto zásadách naleznete v tématu [Co jsou zásady základní ho použití](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Nastavení zásad směrného plánu

1. Přejděte na [portál Azure](https://portal.azure.com)a přejděte na **podmíněný přístup** **služby Azure Active Directory** \> .
    
    Zásady směrného plánu jsou uvedeny na stránce. <br/> <br/>
    ![Stránka, která obsahuje seznam zásad směrného plánu pro podmíněný přístup.](../media/baslinepolicies.png)
1. Pro každou zásadu naleznete následující konkrétní pokyny:

  - [Vyžadovat vícefaktorové čekání pro správce](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vyžadovat vícefaktorové čekání pro uživatele](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokovat starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vyžadovat vícefaktorové řešení pro správu služeb](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Můžete nastavit mnoho dalších zásad, jako je například vyžadování schválených klientských aplikací. Další informace naleznete v [dokumentaci podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).
