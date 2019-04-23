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
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278158"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="4cd3d-103">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4cd3d-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="4cd3d-104">Vytvoření zásady správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="4cd3d-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="4cd3d-105">Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="4cd3d-106">Přihlásit se do [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) s globální správce pověření.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> <span data-ttu-id="4cd3d-107">Vyberte dlaždici **Správce** a přejděte do Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-107">Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="4cd3d-108">Na levá navigace zvolte **zařízení** \> **zásad** \> **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="4cd3d-109">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="4cd3d-110">V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="4cd3d-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="4cd3d-112">Možnost **Šifrovat pracovní soubory** je zapnutá automaticky.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="4cd3d-113">Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="4cd3d-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="4cd3d-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="4cd3d-116">Další informace naleznete v tématu [nastavení k dispozici](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="4cd3d-116">See [Available settings](#available-settings)for more information.</span></span> 
    
    <span data-ttu-id="4cd3d-117">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-117">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="4cd3d-118">Rozbalte možnost **Obnovit data na zařízeních s Windows**, kterou vám doporučujeme **Zapnout**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-118">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="4cd3d-p103">Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit. Pokyny najdete v článku o [vytvoření a ověření certifikátu agenta obnovování dat (DRA) systému souborů EFS](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="4cd3d-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="4cd3d-p104">Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele. Soubor může otevřít a dešifrovat jenom uživatel. Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný. Může ho dešifrovat správce pomocí certifikátu agenta obnovování dat (DRA).</span><span class="sxs-lookup"><span data-stu-id="4cd3d-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="4cd3d-p105">Pokud chcete přidat další domény nebo umístění SharePointu Online, abyste se ujistili, že soubory ve všech uvedených aplikacích budou chráněné, rozbalte možnost **Chránit další umístění v síti a cloudu**. Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="4cd3d-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="4cd3d-p106">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="4cd3d-131">Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-131">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="4cd3d-132">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="4cd3d-132">Available settings</span></span>

<span data-ttu-id="4cd3d-133">Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-133">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="4cd3d-134">Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="4cd3d-134">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="4cd3d-135">**Nastavení**</span><span class="sxs-lookup"><span data-stu-id="4cd3d-135">**Setting**</span></span>|<span data-ttu-id="4cd3d-136">**Popis**</span><span class="sxs-lookup"><span data-stu-id="4cd3d-136">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4cd3d-137">Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="4cd3d-137">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="4cd3d-138">Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-138">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="4cd3d-139">Resetovat PIN po tomto počtu neúspěšných přihlášení</span><span class="sxs-lookup"><span data-stu-id="4cd3d-139">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="4cd3d-140">Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-140">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="4cd3d-141">Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="4cd3d-141">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="4cd3d-142">Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.</span><span class="sxs-lookup"><span data-stu-id="4cd3d-142">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

