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
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="fdb38-103">Nastavení zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="fdb38-103">Set up conditional access policies</span></span>

<span data-ttu-id="fdb38-104">Zásady [podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) přidat substancial další zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="fdb38-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="fdb38-105">Společnost Microsoft poskytuje sadu zásady podmíněného přístupu podle směrného plánu, které se doporučuje pro všechny zákazníky.</span><span class="sxs-lookup"><span data-stu-id="fdb38-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="fdb38-106">Základní zásady jsou sadu předdefinovaných zásad, které pomáhá chránit před útoky mnoho společných organizací.</span><span class="sxs-lookup"><span data-stu-id="fdb38-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="fdb38-107">Tyto společné útoky patří heslo spreje, replay a útoky typu phishing.</span><span class="sxs-lookup"><span data-stu-id="fdb38-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="fdb38-108">Tyto zásady vyžadují admins a uživatelům zadat druhou formu ověřování (nazývané vícefaktorového ověřování nebo MFA) při splnění určitých podmínek.</span><span class="sxs-lookup"><span data-stu-id="fdb38-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="fdb38-109">Pokud je uživatel přihlášení z jiné země, přihlášení mohly být považovány za nebezpečné a uživatel musí poskytnout další formu ověřování.</span><span class="sxs-lookup"><span data-stu-id="fdb38-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="fdb38-110">V současné době zahrnují následující základní zásady:</span><span class="sxs-lookup"><span data-stu-id="fdb38-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="fdb38-111">**Vyžadují MFA pro správce** – vícenásobné ověření vyžaduje většina privilegovaného správce rolí, včetně globálního správce.</span><span class="sxs-lookup"><span data-stu-id="fdb38-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="fdb38-112">**Ochrana koncového uživatele** – vyžaduje vícenásobné ověření pro uživatele pouze v případě, že přihlášení je riskantní.</span><span class="sxs-lookup"><span data-stu-id="fdb38-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="fdb38-113">**Starší verze ověřování blok** – starší klientské aplikace a některé nové aplikace nepoužívejte novější, bezpečnější, ověřovací protokoly.</span><span class="sxs-lookup"><span data-stu-id="fdb38-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="fdb38-114">Tyto starší aplikace může obejít zásady podmíněného přístupu a získat neoprávněný přístup k prostředí.</span><span class="sxs-lookup"><span data-stu-id="fdb38-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="fdb38-115">Tento přístup zásady bloky od klientů, kteří nepodporují podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="fdb38-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="fdb38-116">**MFA vyžaduje pro správu Service** – vícenásobné ověření vyžaduje pro přístup do nástroje pro správu, včetně Azure portálu (Pokud konfigurujete zásady podle směrného plánu).</span><span class="sxs-lookup"><span data-stu-id="fdb38-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="fdb38-117">Společnost Microsoft doporučuje že povolit všechny tyto základní zásady.</span><span class="sxs-lookup"><span data-stu-id="fdb38-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="fdb38-118">Po povolení těchto zásad jsou Administrátoři a uživatelé vyzváni k registraci pro ověřování Azure Multii-faktor.</span><span class="sxs-lookup"><span data-stu-id="fdb38-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="fdb38-119">Další informace o těchto zásadách naleznete v tématu [Jaké jsou základní zásady](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="fdb38-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="fdb38-120">Nastavte základní zásady</span><span class="sxs-lookup"><span data-stu-id="fdb38-120">Set up baseline policies</span></span>

1. <span data-ttu-id="fdb38-121">Přejděte na [portál Azure](https://portal.azure.com)a potom přejděte do **Adresáře Active Directory Azure** \> **Podmíněného přístupu**.</span><span class="sxs-lookup"><span data-stu-id="fdb38-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="fdb38-122">Základní zásady jsou uvedeny na stránce.</span><span class="sxs-lookup"><span data-stu-id="fdb38-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="fdb38-123">![Stránka, která obsahuje základní zásady podmíněného přístupu.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="fdb38-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="fdb38-124">Viz následující pokyny specifické pro každou zásadu:</span><span class="sxs-lookup"><span data-stu-id="fdb38-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="fdb38-125">Vyžadují MFA pro správce</span><span class="sxs-lookup"><span data-stu-id="fdb38-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="fdb38-126">Reequire MFA pro uživatele</span><span class="sxs-lookup"><span data-stu-id="fdb38-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="fdb38-127">Starší verze ověřování blok</span><span class="sxs-lookup"><span data-stu-id="fdb38-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="fdb38-128">Vyžadují MFA pro řízení servisu</span><span class="sxs-lookup"><span data-stu-id="fdb38-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="fdb38-129">Můžete nastavit mnoho další zásady, jako je například požadavek schválené klientských aplikací.</span><span class="sxs-lookup"><span data-stu-id="fdb38-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="fdb38-130">Naleznete další informace v [Dokumentaci podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/) .</span><span class="sxs-lookup"><span data-stu-id="fdb38-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>