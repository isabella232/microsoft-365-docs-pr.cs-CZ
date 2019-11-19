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
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="ce78c-103">Nastavení zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="ce78c-103">Set up conditional access policies</span></span>

<span data-ttu-id="ce78c-104">Zásady [podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidávají podstatné dodatečné zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="ce78c-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="ce78c-105">Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny všem zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="ce78c-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="ce78c-106">Zásady směrného plánu představují sadu předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky.</span><span class="sxs-lookup"><span data-stu-id="ce78c-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="ce78c-107">Tyto běžné útoky mohou zahrnovat postřik hesla, přehrání a podvodné zprávy.</span><span class="sxs-lookup"><span data-stu-id="ce78c-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="ce78c-108">Tyto zásady vyžadují, aby správci a uživatelé zadávali při splnění určitých podmínek druhou formu ověřování (tzv. vícefaktorové ověřování nebo MFA).</span><span class="sxs-lookup"><span data-stu-id="ce78c-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="ce78c-109">Pokud se například uživatel přihlašuje z jiné země, může být přihlášení považováno za rizikové a uživatel musí poskytnout další způsob ověřování.</span><span class="sxs-lookup"><span data-stu-id="ce78c-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="ce78c-110">Zásady základní linie v současné době zahrnují následující:</span><span class="sxs-lookup"><span data-stu-id="ce78c-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="ce78c-111">**Požadovat MFA pro** správce – vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správců, včetně globálního správce.</span><span class="sxs-lookup"><span data-stu-id="ce78c-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="ce78c-112">**Ochrana koncového uživatele** – vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že je přihlášení riskantní.</span><span class="sxs-lookup"><span data-stu-id="ce78c-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="ce78c-113">**Blokovat starší ověřování** – starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější a ověřovací protokoly.</span><span class="sxs-lookup"><span data-stu-id="ce78c-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="ce78c-114">Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí.</span><span class="sxs-lookup"><span data-stu-id="ce78c-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="ce78c-115">Tato zásada blokuje přístup od klientů, kteří nepodporují podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="ce78c-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="ce78c-116">**Vyžadují MFA pro správu servisu** – vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde se konfigurují základní zásady).</span><span class="sxs-lookup"><span data-stu-id="ce78c-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="ce78c-117">Společnost Microsoft doporučuje povolit všechny tyto zásady základní linie.</span><span class="sxs-lookup"><span data-stu-id="ce78c-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="ce78c-118">Po povolení těchto zásad budou správci a uživatelé vyzváni k zaregistrování pro ověřování Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="ce78c-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="ce78c-119">Další informace o těchto zásadách naleznete v tématu [co jsou základní zásady](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="ce78c-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="ce78c-120">Nastavení zásad směrného plánu</span><span class="sxs-lookup"><span data-stu-id="ce78c-120">Set up baseline policies</span></span>

1. <span data-ttu-id="ce78c-121">Přejděte na [portál Azure](https://portal.azure.com)a pak přejděte na Azure **podmíněný přístup** **služby Active Directory** \> .</span><span class="sxs-lookup"><span data-stu-id="ce78c-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="ce78c-122">Základní zásady jsou uvedeny na stránce.</span><span class="sxs-lookup"><span data-stu-id="ce78c-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="ce78c-123">![Stránka se seznamem zásad základní úrovně pro podmíněný přístup.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="ce78c-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="ce78c-124">Pro jednotlivé zásady se podívejte na následující specifické pokyny:</span><span class="sxs-lookup"><span data-stu-id="ce78c-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="ce78c-125">Vyžadovat MFA pro administrátoři</span><span class="sxs-lookup"><span data-stu-id="ce78c-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="ce78c-126">Vyžadovat MFA pro uživatele</span><span class="sxs-lookup"><span data-stu-id="ce78c-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="ce78c-127">Blokovat starší ověřování</span><span class="sxs-lookup"><span data-stu-id="ce78c-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="ce78c-128">Vyžadovat MFA pro správu servisu</span><span class="sxs-lookup"><span data-stu-id="ce78c-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="ce78c-129">Můžete nastavit mnoho dalších zásad, například vyžadování schválených klientských aplikací.</span><span class="sxs-lookup"><span data-stu-id="ce78c-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="ce78c-130">Další informace naleznete v dokumentaci k [podmíněnému přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="ce78c-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
