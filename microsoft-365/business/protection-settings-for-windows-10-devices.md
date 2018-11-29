---
title: Nastavení ochrany aplikací pro zařízení s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Naučte se vytvořit zásadu správy aplikací a ochrany pracovních souborů v zařízení Windows 10.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982821"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="86be7-103">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="86be7-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="86be7-104">Vytvoření zásady správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="86be7-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="86be7-105">Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="86be7-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="86be7-p101">Přihlaste se k [Microsoft 365 Business](https://portal.office.com) pod uživatelským jménem a heslem globálního správce. Vyberte dlaždici **Správce** a přejděte do Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="86be7-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="86be7-108">Na kartě **Zásady zařízení** portálu pro správce zvolte **Přidat zásadu**.</span><span class="sxs-lookup"><span data-stu-id="86be7-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="86be7-110">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="86be7-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="86be7-111">V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="86be7-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="86be7-112">Pod \*\* typ zařízení \*\*, zvolte **osobní** nebo **Ve vlastnictví společnosti**.</span><span class="sxs-lookup"><span data-stu-id="86be7-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="86be7-113">Možnost **Šifrovat pracovní soubory** je zapnutá automaticky.</span><span class="sxs-lookup"><span data-stu-id="86be7-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="86be7-114">Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="86be7-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="86be7-p102">Rozbalte položku **Spravovat přístup uživatelů k souborů sady Office na zařízení** \> nastavit, jakým způsobem. **Spravovat přístup uživatelů k zařízení Office na mobilních zařízeních** je **Vypnuto** ve výchozím nastavení, ale je vhodné **jej zapnout** a přijměte výchozí hodnoty. Další informace naleznete v tématu [nastavení k dispozici](protection-settings-for-windows-10-devices.md#bkmk_settings) .</span><span class="sxs-lookup"><span data-stu-id="86be7-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="86be7-118">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="86be7-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="86be7-119">Rozbalte možnost **Obnovit data na zařízeních s Windows**, kterou vám doporučujeme **Zapnout**.</span><span class="sxs-lookup"><span data-stu-id="86be7-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="86be7-p103">Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit. Pokyny najdete v článku o [vytvoření a ověření certifikátu agenta obnovování dat (DRA) systému souborů EFS](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="86be7-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="86be7-p104">Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele. Soubor může otevřít a dešifrovat jenom uživatel. Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný. Může ho dešifrovat správce pomocí certifikátu agenta obnovování dat (DRA).</span><span class="sxs-lookup"><span data-stu-id="86be7-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="86be7-p105">Pokud chcete přidat další domény nebo umístění SharePointu Online, abyste se ujistili, že soubory ve všech uvedených aplikacích budou chráněné, rozbalte možnost **Chránit další umístění v síti a cloudu**. Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="86be7-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="86be7-p106">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="86be7-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="86be7-132">Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="86be7-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="86be7-133">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="86be7-133">Available settings</span></span>

<span data-ttu-id="86be7-134">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office.</span><span class="sxs-lookup"><span data-stu-id="86be7-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="86be7-135">Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="86be7-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="86be7-136">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="86be7-136">**Setting**</span></span>|<span data-ttu-id="86be7-137">**Popis**</span><span class="sxs-lookup"><span data-stu-id="86be7-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="86be7-138">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="86be7-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="86be7-139">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="86be7-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="86be7-140">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="86be7-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="86be7-141">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="86be7-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="86be7-142">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="86be7-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="86be7-143">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="86be7-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

