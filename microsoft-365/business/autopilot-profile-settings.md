---
title: Informace o nastavení profilu AutoPilota .
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Profily autopilota vám pomohou řídit způsob instalace systému Windows na uživatelských zařízeních. Profily obsahují výchozí a volitelná nastavení, jako je přeskočení instalace Cortany.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593327"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="663a1-104">Informace o nastavení profilu AutoPilota .</span><span class="sxs-lookup"><span data-stu-id="663a1-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="663a1-105">Nastavení profilu autopilota</span><span class="sxs-lookup"><span data-stu-id="663a1-105">AutoPilot profile settings</span></span>

<span data-ttu-id="663a1-106">Profily AutoPilot můžete použít k řízení způsobu instalace systému Windows na uživatelských zařízeních.</span><span class="sxs-lookup"><span data-stu-id="663a1-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="663a1-107">Profily obsahují následující nastavení.</span><span class="sxs-lookup"><span data-stu-id="663a1-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="663a1-108">**Výchozí funkce autopilota (povinné), které jsou nastaveny automaticky:**</span><span class="sxs-lookup"><span data-stu-id="663a1-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="663a1-109">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="663a1-109">**Setting**</span></span>|<span data-ttu-id="663a1-110">**Popis**</span><span class="sxs-lookup"><span data-stu-id="663a1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="663a1-111">Přeskočit registraci Cortany, OneDrivu a OEM</span><span class="sxs-lookup"><span data-stu-id="663a1-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="663a1-112">Přeskočí instalaci spotřebitelských aplikací, jako je Cortana a osobní OneDrive.</span><span class="sxs-lookup"><span data-stu-id="663a1-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="663a1-113">Uživatel zařízení je může nainstalovat později, pokud je uživatel místním správcem zařízení.</span><span class="sxs-lookup"><span data-stu-id="663a1-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="663a1-114">Původní registrace výrobce je přeskočena, protože zařízení bude spravováno společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="663a1-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="663a1-115">Přihlaste se ke značce vaší společnosti</span><span class="sxs-lookup"><span data-stu-id="663a1-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="663a1-116">Pokud má vaše společnost na [přihlašovací stránku Office 365 značku Přidat vaši společnost](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), uživatel zařízení toto prostředí získá při přihlášení.</span><span class="sxs-lookup"><span data-stu-id="663a1-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="663a1-117">Automatický zápis MDM s nakonfigurovanými účty AAD.</span><span class="sxs-lookup"><span data-stu-id="663a1-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="663a1-118">Identitu uživatele bude spravovat služba Azure Active Directory a uživatelé se k Windows a Office 365 přihlásí pomocí přihlašovacích údajů Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="663a1-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="663a1-119">**Volitelné nastavení:**</span><span class="sxs-lookup"><span data-stu-id="663a1-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="663a1-120">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="663a1-120">**Setting**</span></span>|<span data-ttu-id="663a1-121">**Popis**</span><span class="sxs-lookup"><span data-stu-id="663a1-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="663a1-122">Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)</span><span class="sxs-lookup"><span data-stu-id="663a1-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="663a1-123">Pokud je tato možnost nastavena na **zapnuto**, uživatel zařízení neuvidí licenční smlouvu pro zařízení a systém Windows, když se poprvé přihlásí.</span><span class="sxs-lookup"><span data-stu-id="663a1-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="663a1-124">Nedovolte, aby se uživatel stal místním správcem</span><span class="sxs-lookup"><span data-stu-id="663a1-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="663a1-125">Pokud je tato možnost nastavena na **Zapnuto**, uživatel zařízení nebude moci nainstalovat žádné osobní aplikace, jako je například Cortana.</span><span class="sxs-lookup"><span data-stu-id="663a1-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
