---
title: Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Seznamte se s zásadami ochrany, které mohou pomoci zabezpečit přístup k aplikacím sady Office z mobilních zařízení.
ms.openlocfilehash: c24dae7e0eea777e728ebead9a2abcc3785763dd
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633343"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="782d5-103">Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="782d5-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="782d5-104">[] Nastavení zásad, které řídí, jakým způsobem uživatelé přistupují k souborům Office ze svých mobilních zařízení, je ve výchozím nastavení **vypnuté**.</span><span class="sxs-lookup"><span data-stu-id="782d5-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="782d5-105">Doporučujeme, abyste při instalaci přijali výchozí hodnoty a vytvořili tak zásady použití pro systémy Android, iOS a Windows 10, které se vztahují na všechny uživatele.</span><span class="sxs-lookup"><span data-stu-id="782d5-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="782d5-106">Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="782d5-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="782d5-107">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="782d5-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="782d5-108">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="782d5-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="782d5-109">Nastavení</span><span class="sxs-lookup"><span data-stu-id="782d5-109">Setting</span></span>  <br/> |<span data-ttu-id="782d5-110">Popis</span><span class="sxs-lookup"><span data-stu-id="782d5-110">Description</span></span>  <br/> |
|<span data-ttu-id="782d5-111">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="782d5-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="782d5-112">Pokud je toto nastavení **zapnuto**, musí uživatelé před použitím aplikací sady Office v mobilním zařízení zadat kromě uživatelského jména a hesla i jiný způsob ověřování.</span><span class="sxs-lookup"><span data-stu-id="782d5-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="782d5-113">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="782d5-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="782d5-114">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="782d5-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="782d5-115">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="782d5-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="782d5-116">Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se znovu zobrazí výzva k přihlášení.</span><span class="sxs-lookup"><span data-stu-id="782d5-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="782d5-117">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="782d5-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="782d5-118">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem.</span><span class="sxs-lookup"><span data-stu-id="782d5-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="782d5-119">To znamená, že uživatel může změnit operační systém, což může zařízení učinit náchylnějším k malwaru.</span><span class="sxs-lookup"><span data-stu-id="782d5-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="782d5-120">Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.</span><span class="sxs-lookup"><span data-stu-id="782d5-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="782d5-121">Nepovolit uživatelům kopírovat obsah z aplikací sady Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="782d5-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="782d5-122">Pokud je nastavení **zapnuto**, nemůže uživatel kopírovat informace v pracovním souboru do osobního souboru.</span><span class="sxs-lookup"><span data-stu-id="782d5-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="782d5-123">Pokud je nastavení **vypnuto**, může uživatel zkopírovat informace z pracovního souboru do osobního aplikace nebo osobního účtu.</span><span class="sxs-lookup"><span data-stu-id="782d5-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

