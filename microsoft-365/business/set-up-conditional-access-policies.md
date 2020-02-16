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
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="e4dc7-103">Nastavení zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="e4dc7-103">Set up conditional access policies</span></span>

<span data-ttu-id="e4dc7-104">[Zásady podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidávají podstatné další zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="e4dc7-105">Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny pro všechny zákazníky.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="e4dc7-106">Zásady podle směrného plánu jsou sadou předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="e4dc7-107">Tyto běžné útoky mohou zahrnovat sprej heslem, přehrání a phishing.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="e4dc7-108">Tyto zásady vyžadují, aby správci a uživatelé zadali druhou formu ověřování (nazývané vícefaktorové ověřování nebo vícefaktorové ověřování), pokud jsou splněny určité podmínky.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="e4dc7-109">Pokud se například uživatel přihlašuje z jiné země, může být přihlášení považováno za rizikové a uživatel musí poskytnout další formu ověřování.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="e4dc7-110">V současné době zásady směrného plánu zahrnují následující:</span><span class="sxs-lookup"><span data-stu-id="e4dc7-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="e4dc7-111">**Vyžadovat vícefaktorové** &ndash; ověřování pro správce Vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správce, včetně globálního správce.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="e4dc7-112">**Ochrana** &ndash; koncových uživatelů Vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že je přihlášení riskantní.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="e4dc7-113">**Blokovat starší ověřování** &ndash; Starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější ověřovací protokoly.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="e4dc7-114">Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup k vašemu prostředí.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="e4dc7-115">Tato zásada blokuje přístup klientům, kteří nepodporují podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="e4dc7-116">**Vyžadovat vícefaktorové ověřování pro správu** &ndash; služeb Vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde nakonfigurujete zásady směrného plánu).</span><span class="sxs-lookup"><span data-stu-id="e4dc7-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="e4dc7-117">Společnost Microsoft doporučuje povolit všechny tyto zásady směrného plánu.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="e4dc7-118">Po povolení těchto zásad budou správci a uživatelé vyzváni k registraci pro ověřování multiifaktoru Azure.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="e4dc7-119">Další informace o těchto zásadách naleznete v tématu [Co jsou zásady základní ho použití](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="e4dc7-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="e4dc7-120">Nastavení zásad směrného plánu</span><span class="sxs-lookup"><span data-stu-id="e4dc7-120">Set up baseline policies</span></span>

1. <span data-ttu-id="e4dc7-121">Přejděte na [portál Azure](https://portal.azure.com)a přejděte na **podmíněný přístup** **služby Azure Active Directory** \> .</span><span class="sxs-lookup"><span data-stu-id="e4dc7-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="e4dc7-122">Zásady směrného plánu jsou uvedeny na stránce.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="e4dc7-123">![Stránka, která obsahuje seznam zásad směrného plánu pro podmíněný přístup.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="e4dc7-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="e4dc7-124">Pro každou zásadu naleznete následující konkrétní pokyny:</span><span class="sxs-lookup"><span data-stu-id="e4dc7-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="e4dc7-125">Vyžadovat vícefaktorové čekání pro správce</span><span class="sxs-lookup"><span data-stu-id="e4dc7-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="e4dc7-126">Vyžadovat vícefaktorové čekání pro uživatele</span><span class="sxs-lookup"><span data-stu-id="e4dc7-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="e4dc7-127">Blokovat starší ověřování</span><span class="sxs-lookup"><span data-stu-id="e4dc7-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="e4dc7-128">Vyžadovat vícefaktorové řešení pro správu služeb</span><span class="sxs-lookup"><span data-stu-id="e4dc7-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="e4dc7-129">Můžete nastavit mnoho dalších zásad, jako je například vyžadování schválených klientských aplikací.</span><span class="sxs-lookup"><span data-stu-id="e4dc7-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="e4dc7-130">Další informace naleznete v [dokumentaci podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="e4dc7-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
