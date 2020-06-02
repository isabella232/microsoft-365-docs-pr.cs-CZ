---
title: Nastavení zásad podmíněného přístupu pro kampaně Microsoft 365
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Přečtěte si, jak nastavit zásady podmíněného přístupu pro kampaně Microsoft 365, abyste přidali podstatné dodatečné zabezpečení.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470641"
---
# <a name="set-up-conditional-access-policies"></a>Nastavení zásad podmíněného přístupu

Tento článek se týká Microsoft 365 Business Premium.

[Zásady podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidat podstatné další zabezpečení. Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny pro všechny zákazníky. Základní zásady jsou sadou předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky. Tyto běžné útoky mohou zahrnovat sprej hesel, přehrání a phishing.

Tyto zásady vyžadují, aby správci a uživatelé zadali druhou formu ověřování (nazývanou vícefaktorové ověřování nebo vícefaktorové ověřování), pokud jsou splněny určité podmínky. Například pokud se uživatel přihlašuje z jiné země, přihlášení může být považováno za riskantní a uživatel musí poskytnout další formu ověřování. 

V současné době zásady směrného plánu zahrnují následující:
- **Vyžadovat vícefaktové ověřování pro správce** &ndash; Vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správce, včetně globálního správce.
- Ochrana koncového **uživatele** &ndash; Vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že přihlášení je riskantní. 
- **Blokovat starší ověřování** &ndash; Starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější ověřovací protokoly. Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí. Tato zásada blokuje přístup klientů, kteří nepodporují podmíněný přístup. 
- **Vyžadovat vícefakční ověřování pro správu** &ndash; služeb Vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde nakonfigurujete zásady směrného plánu). 

Společnost Microsoft doporučuje povolit všechny tyto zásady směrného plánu. Po povolení těchto zásad budou správci a uživatelé vyzváni k registraci pro ověřování Azure Multii-Factor.

Další informace o těchto zásadách naleznete v [tématu Co jsou zásady směrného plánu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Nastavení zásad směrného plánu

1. Přejděte na [portál Azure](https://portal.azure.com)a přejděte na podmíněný přístup **služby Azure Active Directory** \> **Conditional Access**.
    
    Zásady směrného plánu jsou uvedeny na stránce. <br/> <br/>
    ![Stránka, která obsahuje seznam zásad směrného plánu pro podmíněný přístup.](../media/baslinepolicies.png)
1. Pro jednotlivé zásady naleznete následující konkrétní pokyny:

  - [Vyžadovat vícefaktové ověřování pro správce](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Vyžadovat vícefaktové ověřování pro uživatele](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokovat starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vyžadovat vícefakční ověřování pro správu služeb](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Můžete nastavit mnoho dalších zásad, jako je například vyžadování schválených klientských aplikací. Další informace naleznete v [dokumentaci k podmíněnému přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).
