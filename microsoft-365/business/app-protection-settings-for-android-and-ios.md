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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Naučte se vytvářet, upravovat nebo odstraňovat zásady správy aplikací a chránit pracovní soubory na zařízeních Android nebo iOS.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321839"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="61856-103">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="61856-103">Set app protection settings for Android or iOS devices</span></span>

![To je nápis https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="61856-105">Vytvoření zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="61856-105">Create an app management policy</span></span>

1. <span data-ttu-id="61856-106">Přejděte do centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>adrese.</span><span class="sxs-lookup"><span data-stu-id="61856-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="61856-107">V levém navigačním okně zvolte položku \*\*\*\* \> **zásady** \> zařízení **Add**.</span><span class="sxs-lookup"><span data-stu-id="61856-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="61856-108">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="61856-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="61856-109">V části **Typ zásady**vyberte položku **Správa aplikací pro Android** nebo **správu aplikací pro iOS**podle toho, kterou sadu zásad chcete vytvořit.</span><span class="sxs-lookup"><span data-stu-id="61856-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="61856-110">Rozbalení **chránit pracovní soubory při ztrátě nebo odcizení zařízení** a **správě přístupu uživatelů k souborům sady Office na mobilních zařízeních**</span><span class="sxs-lookup"><span data-stu-id="61856-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="61856-111">Nastavte požadované nastavení.</span><span class="sxs-lookup"><span data-stu-id="61856-111">Configure the settings how you would like.</span></span> <span data-ttu-id="61856-112">**Správa přístupu uživatelů k souborům sady Office na mobilních zařízeních** je ve výchozím nastavení **vypnuta** , doporučujeme jej však **zapnout a přijmout** výchozí hodnoty.</span><span class="sxs-lookup"><span data-stu-id="61856-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="61856-113">Další informace naleznete v tématu [dostupné nastavení](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="61856-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="61856-114">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="61856-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="61856-116">V dalším kroku rozhodněte, **pro koho tato nastavení platí**.</span><span class="sxs-lookup"><span data-stu-id="61856-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="61856-117">Pokud nechcete použít výchozí skupinu zabezpečení **All Users** , zvolte možnost **změnit**, zvolte skupiny zabezpečení, které \> **Toto nastavení zvolí**.</span><span class="sxs-lookup"><span data-stu-id="61856-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="61856-118">Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="61856-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="61856-119">Úprava zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="61856-119">Edit an app management policy</span></span>

1. <span data-ttu-id="61856-120">Na kartě **zásady** zvolte možnost **upravit zásady**.</span><span class="sxs-lookup"><span data-stu-id="61856-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="61856-121">V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit.</span><span class="sxs-lookup"><span data-stu-id="61856-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="61856-122">Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady.</span><span class="sxs-lookup"><span data-stu-id="61856-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="61856-123">Změníte-li hodnotu, bude automaticky uložena do zásady.</span><span class="sxs-lookup"><span data-stu-id="61856-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="61856-124">Po dokončení zavřete podokno **zásad úprav** .</span><span class="sxs-lookup"><span data-stu-id="61856-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="61856-125">Odstranění zásady správy aplikací</span><span class="sxs-lookup"><span data-stu-id="61856-125">Delete an app management policy</span></span>

1. <span data-ttu-id="61856-126">Na stránce **zásady** zvolte zásadu a pak ji **odstraňte**.</span><span class="sxs-lookup"><span data-stu-id="61856-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="61856-127">V podokně **zásad odstranění** zvolte možnost **Potvrdit** odstranění zvolených zásad nebo zásad.</span><span class="sxs-lookup"><span data-stu-id="61856-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="61856-128">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="61856-128">Available settings</span></span>

<span data-ttu-id="61856-129">Následující tabulky obsahují podrobné informace o dostupných nastaveních pro ochranu pracovních souborů na zařízeních a nastavení, které řídí způsob, jakým uživatelé přistupují k souborům sady Office z mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="61856-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="61856-130">Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="61856-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="61856-131">Nastavení chránící pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="61856-131">Settings that protect work files</span></span>

<span data-ttu-id="61856-132">Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="61856-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="61856-133">Nastavení</span><span class="sxs-lookup"><span data-stu-id="61856-133">Setting</span></span>  <br/> |<span data-ttu-id="61856-134">Popis</span><span class="sxs-lookup"><span data-stu-id="61856-134">Description</span></span>  <br/> |
|<span data-ttu-id="61856-135">Odstranit pracovní soubory z neaktivního zařízení za</span><span class="sxs-lookup"><span data-stu-id="61856-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="61856-136">Pokud zařízení není používáno po dobu, kterou zde zadáte, budou všechny pracovní soubory uložené v zařízení automaticky odstraněny.</span><span class="sxs-lookup"><span data-stu-id="61856-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="61856-137">Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="61856-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="61856-138">Pokud je toto nastavení **zapnuto**, jediné dostupné umístění pro uložení pracovních souborů je OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="61856-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="61856-139">Šifrovat pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="61856-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="61856-140">Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním.</span><span class="sxs-lookup"><span data-stu-id="61856-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="61856-141">I když dojde ke ztrátě nebo odcizení zařízení, nikdo nemůže číst data vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="61856-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="61856-142">Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních</span><span class="sxs-lookup"><span data-stu-id="61856-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="61856-143">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:</span><span class="sxs-lookup"><span data-stu-id="61856-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="61856-144">Nastavení</span><span class="sxs-lookup"><span data-stu-id="61856-144">Setting</span></span>  <br/> |<span data-ttu-id="61856-145">Popis</span><span class="sxs-lookup"><span data-stu-id="61856-145">Description</span></span>  <br/> |
|<span data-ttu-id="61856-146">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="61856-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="61856-147">Pokud je toto nastavení **zapnuto** , musí uživatelé před použitím aplikací sady Office na mobilních zařízeních poskytnout další způsob ověřování, a to kromě uživatelského jména a hesla.</span><span class="sxs-lookup"><span data-stu-id="61856-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="61856-148">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="61856-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="61856-149">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="61856-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="61856-150">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="61856-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="61856-151">Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se znovu zobrazí výzva k přihlášení.</span><span class="sxs-lookup"><span data-stu-id="61856-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="61856-152">Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem</span><span class="sxs-lookup"><span data-stu-id="61856-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="61856-p105">Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  </span><span class="sxs-lookup"><span data-stu-id="61856-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="61856-156">Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací</span><span class="sxs-lookup"><span data-stu-id="61856-156">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="61856-157">Tuto možnost ve výchozím nastavení povolíte, ale pokud je toto nastavení **zapnuto**, může uživatel zkopírovat informace v pracovním souboru do osobního souboru.</span><span class="sxs-lookup"><span data-stu-id="61856-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="61856-158">Pokud je toto nastavení **vypnuto**, nebude uživatel moci kopírovat informace z pracovního účtu do osobní aplikace nebo osobního účtu.</span><span class="sxs-lookup"><span data-stu-id="61856-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
