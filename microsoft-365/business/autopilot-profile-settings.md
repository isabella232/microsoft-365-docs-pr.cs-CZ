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
description: Profily autopilota vám pomohou řídit, jak se systém Windows nainstaluje na uživatelská zařízení. Profily obsahují výchozí a volitelná nastavení, jako je přeskočit instalaci Cortany.
ms.openlocfilehash: 0c706d12ba262856ff40ea3bee57c64234fd77f7
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165835"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="c5fe8-104">Informace o nastavení profilu AutoPilota .</span><span class="sxs-lookup"><span data-stu-id="c5fe8-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="c5fe8-105">Nastavení profilu autopilota</span><span class="sxs-lookup"><span data-stu-id="c5fe8-105">AutoPilot profile settings</span></span>

<span data-ttu-id="c5fe8-106">Pomocí profilů AutoPilot můžete určit, jak je systém Windows nainstalován na uživatelských zařízeních.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="c5fe8-107">Profily obsahují následující nastavení.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="c5fe8-108">**Výchozí funkce autopilota (povinné), které jsou nastaveny automaticky:**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="c5fe8-109">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-109">**Setting**</span></span>|<span data-ttu-id="c5fe8-110">**Popis**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5fe8-111">Přeskočit registraci Cortany, OneDrivu a OEM</span><span class="sxs-lookup"><span data-stu-id="c5fe8-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="c5fe8-112">Přeskočí instalaci spotřebitelských aplikací, jako je Cortana a osobní OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="c5fe8-113">Uživatel zařízení můžete nainstalovat později, pokud je uživatel místní správce na zařízení.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="c5fe8-114">Původní registrace výrobce je přeskočena, protože zařízení bude spravovat Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="c5fe8-115">Přihlaste se se svou firemní značkou</span><span class="sxs-lookup"><span data-stu-id="c5fe8-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="c5fe8-116">Pokud má vaše společnost [značku Přidat firemní značku na přihlašovací stránku Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), uživatel zařízení získá toto prostředí při přihlášení.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="c5fe8-117">Automatický zápis MDM s nakonfigurovanými účty AAD.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="c5fe8-118">Identitu uživatele bude spravovat služba Azure Active Directory a uživatelé se přihlásí k Windows a Microsoftu 365 pomocí svých přihlašovacích údajů k Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="c5fe8-119">**Volitelná nastavení:**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="c5fe8-120">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-120">**Setting**</span></span>|<span data-ttu-id="c5fe8-121">**Popis**</span><span class="sxs-lookup"><span data-stu-id="c5fe8-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5fe8-122">Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)</span><span class="sxs-lookup"><span data-stu-id="c5fe8-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="c5fe8-123">Pokud je tato možnost nastavena **na Zapnuto**, uživatel zařízení neuvidí licenční smlouvu pro zařízení a systém Windows při prvním přihlášení.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="c5fe8-124">Nedovolte, aby se uživatel stal místním správcem</span><span class="sxs-lookup"><span data-stu-id="c5fe8-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="c5fe8-125">Pokud je tato možnost nastavena **na Zapnuto**, uživatel zařízení nebude moci instalovat žádné osobní aplikace, například Cortanu.</span><span class="sxs-lookup"><span data-stu-id="c5fe8-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
