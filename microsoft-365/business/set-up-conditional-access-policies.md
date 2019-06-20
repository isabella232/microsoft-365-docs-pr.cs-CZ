---
title: Nastavit zásady podmíněného přístupu pro Microsoft 365 kampaně
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Zjistěte, jak nastavit zásady podmíněného přístupu pro Microsoft 365 kampaně.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086293"
---
# <a name="set-up-conditional-access-policies"></a>Nastavení zásad podmíněného přístupu

Zásady [podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidat substancial další zabezpečení. Společnost Microsoft poskytuje sadu zásady podmíněného přístupu podle směrného plánu, které se doporučuje pro všechny zákazníky. Základní zásady jsou sadu předdefinovaných zásad, které pomáhá chránit před útoky mnoho společných organizací. Tyto společné útoky patří heslo spreje, replay a útoky typu phishing.

Tyto zásady vyžadují admins a uživatelům zadat druhou formu ověřování (nazývané vícefaktorového ověřování nebo MFA) při splnění určitých podmínek. Pokud je uživatel přihlášení z jiné země, přihlášení mohly být považovány za nebezpečné a uživatel musí poskytnout další formu ověřování. 

V současné době zahrnují následující základní zásady:
- **Vyžadují MFA pro správce** – vícenásobné ověření vyžaduje většina privilegovaného správce rolí, včetně globálního správce.
- **Ochrana koncového uživatele** – vyžaduje vícenásobné ověření pro uživatele pouze v případě, že přihlášení je riskantní. 
- **Starší verze ověřování blok** – starší klientské aplikace a některé nové aplikace nepoužívejte novější, bezpečnější, ověřovací protokoly. Tyto starší aplikace může obejít zásady podmíněného přístupu a získat neoprávněný přístup k prostředí. Tento přístup zásady bloky od klientů, kteří nepodporují podmíněného přístupu. 
- **MFA vyžaduje pro správu Service** – vícenásobné ověření vyžaduje pro přístup do nástroje pro správu, včetně Azure portálu (Pokud konfigurujete zásady podle směrného plánu). 

Společnost Microsoft doporučuje že povolit všechny tyto základní zásady. Po povolení těchto zásad jsou Administrátoři a uživatelé vyzváni k registraci pro ověřování Azure Multii-faktor.

Další informace o těchto zásadách naleznete v tématu [Jaké jsou základní zásady](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Nastavte základní zásady

1. Přejděte na [portál Azure](https://portal.azure.com)a potom přejděte do **Adresáře Active Directory Azure** \> **Podmíněného přístupu**.
    
    Základní zásady jsou uvedeny na stránce. <br/> <br/>
    ![Stránka, která obsahuje základní zásady podmíněného přístupu.](media/baslinepolicies.png)
1. Viz následující pokyny specifické pro každou zásadu:

  - [Vyžadují MFA pro správce](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire MFA pro uživatele](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Starší verze ověřování blok](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Vyžadují MFA pro řízení servisu](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Můžete nastavit mnoho další zásady, jako je například požadavek schválené klientských aplikací. Naleznete další informace v [Dokumentaci podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/) .