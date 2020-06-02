---
title: Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Přečtěte si o zásadách ochrany, které vám umožňují spravovat, jak uživatelé přistupují k aplikacím Office a pracovním souborům z mobilních zařízení.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471061"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="a4a1b-103">Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="a4a1b-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="a4a1b-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a4a1b-105">[] Nastavení zásad, které řídí, jakým způsobem uživatelé přistupují k souborům Office ze svých mobilních zařízení, je ve výchozím nastavení **vypnuté**.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="a4a1b-106">Doporučujeme přijmout výchozí hodnoty během instalace a vytvořit zásady aplikací pro Android, iOS a Windows 10, které platí pro všechny uživatele.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="a4a1b-107">Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="a4a1b-108">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="a4a1b-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="a4a1b-109">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="a4a1b-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="a4a1b-110">Nastavení</span><span class="sxs-lookup"><span data-stu-id="a4a1b-110">Setting</span></span>  <br/> |<span data-ttu-id="a4a1b-111">Popis</span><span class="sxs-lookup"><span data-stu-id="a4a1b-111">Description</span></span>  <br/> |
|<span data-ttu-id="a4a1b-112">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="a4a1b-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="a4a1b-113">Pokud je toto nastavení **zapnuto**, musí uživatelé před použitím aplikací Office na svém mobilním zařízení poskytnout i jinou formu ověřování.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="a4a1b-114">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="a4a1b-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="a4a1b-115">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="a4a1b-116">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="a4a1b-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="a4a1b-117">Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se zobrazí výzva k opětovnému přihlášení.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="a4a1b-118">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="a4a1b-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="a4a1b-119">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="a4a1b-120">To znamená, že uživatel může upravit operační systém, což může učinit zařízení náchylnější k malwaru.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="a4a1b-121">Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="a4a1b-122">Nepovolit uživatelům kopírování obsahu z aplikací Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="a4a1b-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="a4a1b-123">Pokud je nastavení **zapnuto**, uživatel nemůže kopírovat informace v pracovním souboru do osobního souboru.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="a4a1b-124">Pokud je nastavení **Vypnuto**, může uživatel zkopírovat informace z pracovního souboru do osobní aplikace nebo osobního účtu.</span><span class="sxs-lookup"><span data-stu-id="a4a1b-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

