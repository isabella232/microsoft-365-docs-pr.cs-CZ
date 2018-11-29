---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Zjistěte, jak vytvořit, upravit, nebo odstranit zásadu správy aplikace a ochrana souborů práce na Android nebo iOS zařízení.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983661"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="af0e3-103">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="af0e3-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="af0e3-104">Vytvoření zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="af0e3-104">Create an app management policy</span></span>

1. <span data-ttu-id="af0e3-105">Přihlaste se k [Microsoft 365 Business](https://portal.office.com) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="af0e3-105">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="af0e3-106">V Centru pro správu přejděte na kartu **Zásady zařízení** a zvolte **Přidat zásadu**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-106">In the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="af0e3-108">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="af0e3-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="af0e3-109">V části **Typ zásady** zvolte **Správa aplikací pro Android** nebo **Správa aplikací pro iOS** (podle toho, jakou sadu zásad chcete vytvořit).</span><span class="sxs-lookup"><span data-stu-id="af0e3-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="af0e3-p101">Rozbalte položku **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** a **Správa přístupu uživatelů na soubory sady Office na mobilních zařízeních** \> nastavit, jakým způsobem. **Správa přístupu uživatelů na soubory sady Office na mobilních zařízeních** je **Vypnuto** ve výchozím nastavení, ale je vhodné **jej zapnout** a přijměte výchozí hodnoty. Další informace naleznete v tématu [nastavení k dispozici](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) .</span><span class="sxs-lookup"><span data-stu-id="af0e3-p101">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="af0e3-113">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="af0e3-p102">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="af0e3-117">Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="af0e3-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="af0e3-118">Úprava zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="af0e3-118">Edit an app management policy</span></span>

1. <span data-ttu-id="af0e3-119">Na kartě **zásady** klepněte na příkaz **Upravit zásady**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="af0e3-120">V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit.</span><span class="sxs-lookup"><span data-stu-id="af0e3-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="af0e3-p103">Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když hodnotu změníte, automaticky se do zásady uloží.</span><span class="sxs-lookup"><span data-stu-id="af0e3-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="af0e3-123">Jakmile skončíte, podokno **Upravit zásadu** zavřete.</span><span class="sxs-lookup"><span data-stu-id="af0e3-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="af0e3-124">Odstranění zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="af0e3-124">Delete an app management policy</span></span>

1. <span data-ttu-id="af0e3-125">Na kartě **Zásady** zvolte **Odstranit zásadu**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-125">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="af0e3-126">V podokně **Odstranit zásadu** zvolte zásady, které chcete odstranit \> **Vybrat** a potom vybranou zásadu nebo zásady odstraňte kliknutím na **Potvrdit**.</span><span class="sxs-lookup"><span data-stu-id="af0e3-126">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="af0e3-127">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="af0e3-127">Available settings</span></span>

<span data-ttu-id="af0e3-128">Následující tabulky poskytují podrobné informace o dostupných nastaveních, která chrání pracovní soubory na zařízeních, a nastaveních, která spravují přístup uživatelů k souborům Office z mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="af0e3-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="af0e3-129">Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="af0e3-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="af0e3-130">Nastavení chránící pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="af0e3-130">Settings that protect work files</span></span>

<span data-ttu-id="af0e3-131">Následující nastavení jsou k dispozici pro ochranu pracovních souborů, když se zařízení uživatele ztratí nebo je odcizeno:</span><span class="sxs-lookup"><span data-stu-id="af0e3-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="af0e3-132">Nastavení</span><span class="sxs-lookup"><span data-stu-id="af0e3-132">Setting</span></span>  <br/> |<span data-ttu-id="af0e3-133">Popis</span><span class="sxs-lookup"><span data-stu-id="af0e3-133">Description</span></span>  <br/> |
|<span data-ttu-id="af0e3-134">Odstranit pracovní soubory z neaktivního zařízení za</span><span class="sxs-lookup"><span data-stu-id="af0e3-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="af0e3-135">Pokud se zařízení nebude používat určený počet dní, budou všechny pracovní soubory uložené na zařízení automaticky odstraněny.</span><span class="sxs-lookup"><span data-stu-id="af0e3-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="af0e3-136">Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="af0e3-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="af0e3-137">Pokud je toto nastavení **zapnuté**, jediným možným úložištěm pracovních souboru bude OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="af0e3-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="af0e3-138">Šifrovat pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="af0e3-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="af0e3-p104">Toto nastavení ponechte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. Ani v případě ztráty nebo odcizení nebude moct nikdo data vaší společnosti přečíst.  </span><span class="sxs-lookup"><span data-stu-id="af0e3-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="af0e3-141">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="af0e3-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="af0e3-142">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="af0e3-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="af0e3-143">Nastavení</span><span class="sxs-lookup"><span data-stu-id="af0e3-143">Setting</span></span>  <br/> |<span data-ttu-id="af0e3-144">Popis</span><span class="sxs-lookup"><span data-stu-id="af0e3-144">Description</span></span>  <br/> |
|<span data-ttu-id="af0e3-145">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="af0e3-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="af0e3-146">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="af0e3-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="af0e3-147">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="af0e3-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="af0e3-148">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="af0e3-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="af0e3-149">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="af0e3-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="af0e3-150">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="af0e3-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="af0e3-151">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="af0e3-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="af0e3-p105">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. Uživatel takového zařízení může měnit operační systém, ale jeho zařízení je náchylnější k malwarovým útokům. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  </span><span class="sxs-lookup"><span data-stu-id="af0e3-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="af0e3-155">Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="af0e3-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="af0e3-p106">Nám umožňují ve výchozím nastavení, ale jestliže je nastavena **na**uživatele by mohl zkopírovat informace v souboru pracovní soubor osobních. Pokud je toto nastavení **Vypnuto**, uživatel nebude možné kopírovat informace z pracovního účtu do osobní aplikace nebo osobní účet.</span><span class="sxs-lookup"><span data-stu-id="af0e3-p106">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file. If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.  </span></span><br/> |
   

  

