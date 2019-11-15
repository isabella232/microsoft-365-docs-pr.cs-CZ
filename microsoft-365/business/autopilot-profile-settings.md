---
title: Informace o nastavení profilu AutoPilota .
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
description: Profily AutoPilot vám pomohou určit, jak bude systém Windows nainstalován na uživatelských zařízeních. Profily obsahují výchozí a volitelná nastavení, jako je vynechání instalace Cortana.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321779"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="f2fa9-104">Informace o nastavení profilu AutoPilota .</span><span class="sxs-lookup"><span data-stu-id="f2fa9-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="f2fa9-105">Nastavení profilu AutoPilot</span><span class="sxs-lookup"><span data-stu-id="f2fa9-105">AutoPilot profile settings</span></span>

<span data-ttu-id="f2fa9-106">Pomocí profilů automatických Opilot můžete řídit způsob instalace systému Windows na uživatelská zařízení.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="f2fa9-107">Profily obsahují následující nastavení.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="f2fa9-108">**Automaticky nastaveny výchozí funkce AutoPilot (povinné):**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="f2fa9-109">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-109">**Setting**</span></span>|<span data-ttu-id="f2fa9-110">**Popis**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2fa9-111">Přeskočit Cortana, OneDrive a registraci OEM</span><span class="sxs-lookup"><span data-stu-id="f2fa9-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="f2fa9-112">Přeskočí instalaci zákaznických aplikací, jako je Cortana a Personal OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="f2fa9-113">Uživatel zařízení je může nainstalovat později, dokud je uživatel místním správcem zařízení.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="f2fa9-114">Původní registrace výrobce je přeskočena, protože zařízení bude spravováno společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="f2fa9-115">Přihlášení ke zkušenostem s firemní značkou</span><span class="sxs-lookup"><span data-stu-id="f2fa9-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="f2fa9-116">Pokud vaše společnost disponuje [značkou vaší společnosti na přihlašovací stránce sady Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), zobrazí se uživateli zařízení při přihlášení tato zkušenost.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="f2fa9-117">Automatický zápis MDM s konfigurovanými účty AAD.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="f2fa9-118">Identita uživatele bude spravována společností Azure Active Directory a uživatelé se budou přihlašovat k systému Windows a sadě Office 365 se svými pověřeními Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="f2fa9-119">**Volitelná nastavení:**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="f2fa9-120">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-120">**Setting**</span></span>|<span data-ttu-id="f2fa9-121">**Popis**</span><span class="sxs-lookup"><span data-stu-id="f2fa9-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2fa9-122">Přeskočit nastavení ochrany osobních údajů (ve výchozím nastavení vypnuto)</span><span class="sxs-lookup"><span data-stu-id="f2fa9-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="f2fa9-123">Je-li tato možnost nastavena na zapnuto, nezobrazí se uživateli zařízení licenční smlouva pro zařízení a systém Windows při prvním **přihlášení**.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="f2fa9-124">Nepovolit uživateli stát se místním správcem</span><span class="sxs-lookup"><span data-stu-id="f2fa9-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="f2fa9-125">Pokud je tato možnost nastavena na **zapnuto**, nebude uživatel zařízení moci instalovat žádné osobní aplikace, například Cortana.</span><span class="sxs-lookup"><span data-stu-id="f2fa9-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
