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
description: Přečtěte si, jak nastavit zásady podmíněného přístupu pro kampaně Microsoft 365, abyste přidali podstatné další zabezpečení.
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403012"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="a4b3f-103">Nastavení zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="a4b3f-103">Set up conditional access policies</span></span>

<span data-ttu-id="a4b3f-104">[Zásady podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidávají značné dodatečné zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="a4b3f-105">Společnost Microsoft poskytuje sadu zásad podmíněného přístupu podle směrného plánu, které jsou doporučeny pro všechny zákazníky.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="a4b3f-106">Zásady směrného plánu jsou sadou předdefinovaných zásad, které pomáhají chránit organizace před mnoha běžnými útoky.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="a4b3f-107">Tyto běžné útoky mohou zahrnovat sprej hesla, přehrání a phishing.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="a4b3f-108">Tyto zásady vyžadují, aby správci a uživatelé zadali druhou formu ověřování (tzv. vícefaktorové ověřování nebo vícefaktorové ověřování) při splnění určitých podmínek.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="a4b3f-109">Například pokud se uživatel přihlašuje z jiné země, přihlášení může být považováno za rizikové a uživatel musí poskytnout další formu ověřování.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="a4b3f-110">V současné době zásady směrného plánu zahrnují následující:</span><span class="sxs-lookup"><span data-stu-id="a4b3f-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="a4b3f-111">**Vyžadovat vícefaktorové pomocné správou pro správce** &ndash; Vyžaduje vícefaktorové ověřování pro nejvíce privilegované role správce, včetně globálního správce.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="a4b3f-112">Ochrana koncových **uživatelů** &ndash; Vyžaduje vícefaktorové ověřování pro uživatele pouze v případě, že přihlášení je riskantní.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="a4b3f-113">**Blokovat starší verze ověřování** &ndash; Starší klientské aplikace a některé nové aplikace nepoužívají novější, bezpečnější ověřovací protokoly.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="a4b3f-114">Tyto starší aplikace mohou obejít zásady podmíněného přístupu a získat neoprávněný přístup do vašeho prostředí.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="a4b3f-115">Tato zásada blokuje přístup od klientů, kteří nepodporují podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="a4b3f-116">**Vyžadovat vícefaktorové řízení pro správu** &ndash; služeb Vyžaduje vícefaktorové ověřování pro přístup k nástrojům pro správu, včetně portálu Azure (kde nakonfigurujete zásady směrného plánu).</span><span class="sxs-lookup"><span data-stu-id="a4b3f-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="a4b3f-117">Společnost Microsoft doporučuje povolit všechny tyto zásady směrného plánu.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="a4b3f-118">Po povolení těchto zásad budou správci a uživatelé vyzváni k registraci pro ověřování Azure Multii-Factor.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="a4b3f-119">Další informace o těchto zásadách naleznete v tématu [Co jsou zásady směrného plánu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="a4b3f-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="a4b3f-120">Nastavení zásad směrného plánu</span><span class="sxs-lookup"><span data-stu-id="a4b3f-120">Set up baseline policies</span></span>

1. <span data-ttu-id="a4b3f-121">Přejděte na [portál Azure](https://portal.azure.com)a přejděte na podmíněný přístup **služby Azure Active Directory** \> **Conditional Access**.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="a4b3f-122">Zásady směrného plánu jsou uvedeny na stránce.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="a4b3f-123">![Stránka se seznamem zásad směrného plánu pro podmíněný přístup.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="a4b3f-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="a4b3f-124">Podívejte se na následující konkrétní pokyny pro každou zásadu:</span><span class="sxs-lookup"><span data-stu-id="a4b3f-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="a4b3f-125">Vyžadovat vícefaktorové pomocné správou pro správce</span><span class="sxs-lookup"><span data-stu-id="a4b3f-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="a4b3f-126">Vyžadovat vícefaktorové faktory pro uživatele</span><span class="sxs-lookup"><span data-stu-id="a4b3f-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="a4b3f-127">Blokovat starší verze ověřování</span><span class="sxs-lookup"><span data-stu-id="a4b3f-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="a4b3f-128">Vyžadovat vícefaktorové řízení pro správu služeb</span><span class="sxs-lookup"><span data-stu-id="a4b3f-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="a4b3f-129">Můžete nastavit mnoho dalších zásad, například vyžadování schválených klientských aplikací.</span><span class="sxs-lookup"><span data-stu-id="a4b3f-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="a4b3f-130">Další informace naleznete v [dokumentaci podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="a4b3f-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
