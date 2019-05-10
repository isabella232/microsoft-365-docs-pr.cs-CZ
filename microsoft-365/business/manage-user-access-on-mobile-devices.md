---
title: Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
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
description: Informace týkající se zásad ochrany, které vám mohou pomoci zabezpečený přístup k aplikacím sady Office z mobilních zařízení.
ms.openlocfilehash: b49ec33f4899a25f92ffd9d7a25d3e435016749e
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660318"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="690ae-103">Správa přístupu uživatelů k dokumentům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="690ae-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="690ae-p101">[] Nastavení zásad, které řídí, jakým způsobem uživatelé přistupují k souborům Office ze svých mobilních zařízení, je ve výchozím nastavení **vypnuté**. Doporučujeme vám přijmou během instalace výchozí hodnoty, abyste vytvořili zásady aplikací pro Android, iOS a Windows 10, které platí pro všechny uživatele. Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="690ae-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="690ae-107">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="690ae-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="690ae-108">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="690ae-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="690ae-109">Nastavení</span><span class="sxs-lookup"><span data-stu-id="690ae-109">Setting</span></span>  <br/> |<span data-ttu-id="690ae-110">Popis</span><span class="sxs-lookup"><span data-stu-id="690ae-110">Description</span></span>  <br/> |
|<span data-ttu-id="690ae-111">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="690ae-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="690ae-112">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="690ae-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="690ae-113">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="690ae-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="690ae-114">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="690ae-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="690ae-115">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="690ae-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="690ae-116">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="690ae-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="690ae-117">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="690ae-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="690ae-p102">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  </span><span class="sxs-lookup"><span data-stu-id="690ae-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="690ae-121">Nepovolit uživatelům kopírovat obsah z aplikací sady Office do aplikace osobní</span><span class="sxs-lookup"><span data-stu-id="690ae-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="690ae-122">Po **Zapnutí**nastavení uživatele nelze kopírovat informace v souboru pracovní soubor osobních.</span><span class="sxs-lookup"><span data-stu-id="690ae-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="690ae-123">Pokud je toto nastavení **Vypnuto**, uživatel můžete kopírovat informace z pracovní soubor app na osobní nebo osobní účet.</span><span class="sxs-lookup"><span data-stu-id="690ae-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

