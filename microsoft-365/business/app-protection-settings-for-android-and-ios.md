---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Zjistěte, jak vytvořit, upravit, nebo odstranit zásadu správy aplikace a ochrana souborů práce na Android nebo iOS zařízení.
ms.openlocfilehash: 21cc1d91c2952c6e9414d3742c26547fc36016a5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073504"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="74927-103">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="74927-103">Set app protection settings for Android or iOS devices</span></span>

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="74927-105">Vytvoření zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="74927-105">Create an app management policy</span></span>

1. <span data-ttu-id="74927-106">Přejděte na stránku Správce na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="74927-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="74927-107">V levá navigace zvolte **zařízení** \> **zásad** \> **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="74927-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="74927-108">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="74927-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="74927-109">V části **Typ zásady** zvolte **Správa aplikací pro Android** nebo **Správa aplikací pro iOS** (podle toho, jakou sadu zásad chcete vytvořit).</span><span class="sxs-lookup"><span data-stu-id="74927-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="74927-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="74927-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="74927-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="74927-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="74927-112">Další informace naleznete v tématu [nastavení k dispozici](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="74927-112">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="74927-113">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="74927-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="74927-p102">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="74927-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="74927-117">Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="74927-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="74927-118">Úprava zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="74927-118">Edit an app management policy</span></span>

1. <span data-ttu-id="74927-119">Na kartě **zásady** klepněte na příkaz **Upravit zásady**.</span><span class="sxs-lookup"><span data-stu-id="74927-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="74927-120">V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit.</span><span class="sxs-lookup"><span data-stu-id="74927-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="74927-p103">Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když hodnotu změníte, automaticky se do zásady uloží.</span><span class="sxs-lookup"><span data-stu-id="74927-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="74927-123">Jakmile skončíte, podokno **Upravit zásadu** zavřete.</span><span class="sxs-lookup"><span data-stu-id="74927-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="74927-124">Odstranění zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="74927-124">Delete an app management policy</span></span>

1. <span data-ttu-id="74927-125">Na stránce **zásady** vyberte zásady a pak **Odstranit**.</span><span class="sxs-lookup"><span data-stu-id="74927-125">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="74927-126">**Odstranění zásady** podokně zvolte **Potvrdit** odstranění zásady nebo zásady, kterou jste zvolili.</span><span class="sxs-lookup"><span data-stu-id="74927-126">On the **Delete policy** pane choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="74927-127">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="74927-127">Available settings</span></span>

<span data-ttu-id="74927-128">Následující tabulky poskytují podrobné informace o dostupných nastaveních, která chrání pracovní soubory na zařízeních, a nastaveních, která spravují přístup uživatelů k souborům Office z mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="74927-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="74927-129">Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="74927-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="74927-130">Nastavení chránící pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="74927-130">Settings that protect work files</span></span>

<span data-ttu-id="74927-131">Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="74927-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="74927-132">Nastavení</span><span class="sxs-lookup"><span data-stu-id="74927-132">Setting</span></span>  <br/> |<span data-ttu-id="74927-133">Popis</span><span class="sxs-lookup"><span data-stu-id="74927-133">Description</span></span>  <br/> |
|<span data-ttu-id="74927-134">Odstranit pracovní soubory z neaktivního zařízení za</span><span class="sxs-lookup"><span data-stu-id="74927-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="74927-135">Pokud se zařízení nebude používat určený počet dní, budou všechny pracovní soubory uložené na zařízení automaticky odstraněny.</span><span class="sxs-lookup"><span data-stu-id="74927-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="74927-136">Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="74927-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="74927-137">Pokud je toto nastavení **zapnuté**, jediným možným úložištěm pracovních souboru bude OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="74927-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="74927-138">Šifrovat pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="74927-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="74927-p104">Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. Ani v případě ztráty nebo odcizení nebude moct nikdo data vaší společnosti přečíst.  </span><span class="sxs-lookup"><span data-stu-id="74927-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="74927-141">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="74927-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="74927-142">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="74927-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="74927-143">Nastavení</span><span class="sxs-lookup"><span data-stu-id="74927-143">Setting</span></span>  <br/> |<span data-ttu-id="74927-144">Popis</span><span class="sxs-lookup"><span data-stu-id="74927-144">Description</span></span>  <br/> |
|<span data-ttu-id="74927-145">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="74927-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="74927-146">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="74927-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="74927-147">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="74927-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="74927-148">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="74927-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="74927-149">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="74927-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="74927-150">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="74927-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="74927-151">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="74927-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="74927-p105">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  </span><span class="sxs-lookup"><span data-stu-id="74927-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="74927-155">Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="74927-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="74927-156">Nám umožňují ve výchozím nastavení, ale jestliže je nastavena **na**uživatele by mohl zkopírovat informace v souboru pracovní soubor osobních.</span><span class="sxs-lookup"><span data-stu-id="74927-156">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="74927-157">Pokud je toto nastavení **Vypnuto**, uživatel nebude možné kopírovat informace z pracovního účtu do osobní aplikace nebo osobní účet.</span><span class="sxs-lookup"><span data-stu-id="74927-157">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

