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
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="491ba-103">Nastavení zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="491ba-103">Set up conditional access policies</span></span>

<span data-ttu-id="491ba-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="491ba-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="491ba-105">[Zásady podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidat podstatné další zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="491ba-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="491ba-106">Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny pro všechny zákazníky.</span><span class="sxs-lookup"><span data-stu-id="491ba-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="491ba-107">Základní zásady jsou sadou předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky.</span><span class="sxs-lookup"><span data-stu-id="491ba-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="491ba-108">Tyto běžné útoky mohou zahrnovat sprej hesel, přehrání a phishing.</span><span class="sxs-lookup"><span data-stu-id="491ba-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="491ba-109">Tyto zásady vyžadují, aby správci a uživatelé zadali druhou formu ověřování (nazývanou vícefaktorové ověřování nebo vícefaktorové ověřování), pokud jsou splněny určité podmínky.</span><span class="sxs-lookup"><span data-stu-id="491ba-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="491ba-110">Například pokud se uživatel přihlašuje z jiné země, přihlášení může být považováno za riskantní a uživatel musí poskytnout další formu ověřování.</span><span class="sxs-lookup"><span data-stu-id="491ba-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="491ba-111">V současné době zásady směrného plánu zahrnují následující:</span><span class="sxs-lookup"><span data-stu-id="491ba-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="491ba-112">**Vyžadovat vícefaktové ověřování pro správce** &ndash; Vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správce, včetně globálního správce.</span><span class="sxs-lookup"><span data-stu-id="491ba-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="491ba-113">Ochrana koncového **uživatele** &ndash; Vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že přihlášení je riskantní.</span><span class="sxs-lookup"><span data-stu-id="491ba-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="491ba-114">**Blokovat starší ověřování** &ndash; Starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější ověřovací protokoly.</span><span class="sxs-lookup"><span data-stu-id="491ba-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="491ba-115">Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí.</span><span class="sxs-lookup"><span data-stu-id="491ba-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="491ba-116">Tato zásada blokuje přístup klientů, kteří nepodporují podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="491ba-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="491ba-117">**Vyžadovat vícefakční ověřování pro správu** &ndash; služeb Vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde nakonfigurujete zásady směrného plánu).</span><span class="sxs-lookup"><span data-stu-id="491ba-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="491ba-118">Společnost Microsoft doporučuje povolit všechny tyto zásady směrného plánu.</span><span class="sxs-lookup"><span data-stu-id="491ba-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="491ba-119">Po povolení těchto zásad budou správci a uživatelé vyzváni k registraci pro ověřování Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="491ba-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="491ba-120">Další informace o těchto zásadách naleznete v [tématu Co jsou zásady směrného plánu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="491ba-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="491ba-121">Nastavení zásad směrného plánu</span><span class="sxs-lookup"><span data-stu-id="491ba-121">Set up baseline policies</span></span>

1. <span data-ttu-id="491ba-122">Přejděte na [portál Azure](https://portal.azure.com)a přejděte na podmíněný přístup **služby Azure Active Directory** \> **Conditional Access**.</span><span class="sxs-lookup"><span data-stu-id="491ba-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="491ba-123">Zásady směrného plánu jsou uvedeny na stránce.</span><span class="sxs-lookup"><span data-stu-id="491ba-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="491ba-124">![Stránka, která obsahuje seznam zásad směrného plánu pro podmíněný přístup.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="491ba-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="491ba-125">Pro jednotlivé zásady naleznete následující konkrétní pokyny:</span><span class="sxs-lookup"><span data-stu-id="491ba-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="491ba-126">Vyžadovat vícefaktové ověřování pro správce</span><span class="sxs-lookup"><span data-stu-id="491ba-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="491ba-127">Vyžadovat vícefaktové ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="491ba-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="491ba-128">Blokovat starší ověřování</span><span class="sxs-lookup"><span data-stu-id="491ba-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="491ba-129">Vyžadovat vícefakční ověřování pro správu služeb</span><span class="sxs-lookup"><span data-stu-id="491ba-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="491ba-130">Můžete nastavit mnoho dalších zásad, jako je například vyžadování schválených klientských aplikací.</span><span class="sxs-lookup"><span data-stu-id="491ba-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="491ba-131">Další informace naleznete v [dokumentaci k podmíněnému přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="491ba-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
