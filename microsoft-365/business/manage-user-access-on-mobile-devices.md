---
title: Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
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
description: Informace týkající se zásad ochrany, které vám mohou pomoci zabezpečený přístup k aplikacím sady Office z mobilních zařízení.
ms.openlocfilehash: b77d30686b26f95de684238d1b9afd57550a7c7f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278603"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="bbdef-103">Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="bbdef-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="bbdef-p101">[] Nastavení zásad, které řídí, jakým způsobem uživatelé přistupují k souborům Office ze svých mobilních zařízení, je ve výchozím nastavení **vypnuté**. Doporučujeme vám přijmou během instalace výchozí hodnoty, abyste vytvořili zásady aplikací pro Android, iOS a Windows 10, které platí pro všechny uživatele. Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="bbdef-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="bbdef-107">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="bbdef-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="bbdef-108">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="bbdef-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="bbdef-109">Nastavení</span><span class="sxs-lookup"><span data-stu-id="bbdef-109">Setting</span></span>  <br/> |<span data-ttu-id="bbdef-110">Popis</span><span class="sxs-lookup"><span data-stu-id="bbdef-110">Description</span></span>  <br/> |
|<span data-ttu-id="bbdef-111">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="bbdef-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="bbdef-112">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="bbdef-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="bbdef-113">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="bbdef-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="bbdef-114">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="bbdef-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="bbdef-115">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="bbdef-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="bbdef-116">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="bbdef-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="bbdef-117">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="bbdef-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="bbdef-p102">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  </span><span class="sxs-lookup"><span data-stu-id="bbdef-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="bbdef-121">Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="bbdef-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="bbdef-p103">Ve výchozím nastavení toto umožňujeme, ale pokud je nastavení **zapnuté**, uživatel může kopírovat informace z pracovního souboru do osobního souboru. Pokud je toto nastavení **vypnuté**, uživatel informace z pracovního souboru do osobní aplikace nebo na osobní účet kopírovat nemůže.  </span><span class="sxs-lookup"><span data-stu-id="bbdef-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

