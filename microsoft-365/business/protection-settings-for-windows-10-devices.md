---
title: Nastavení ochrany aplikací pro zařízení s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Naučte se vytvářet zásady správy aplikací a chránit pracovní soubory na zařízeních systému Windows 10.
ms.openlocfilehash: ca6d789e0242975a0395e6cf5653d3f43f819801
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715246"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="28196-103">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="28196-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="28196-104">Vytvoření zásady správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="28196-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="28196-105">Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="28196-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="28196-106">Přejděte do centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>adrese.</span><span class="sxs-lookup"><span data-stu-id="28196-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="28196-107">Na levém navigačním panelu zvolte položku \*\*\*\* \> **zásady** \> zařízení **Add**.</span><span class="sxs-lookup"><span data-stu-id="28196-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="28196-108">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="28196-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="28196-109">V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="28196-109">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="28196-110">V části **typ zařízení**vyberte položku **osobní** nebo **vlastněná společnost**.</span><span class="sxs-lookup"><span data-stu-id="28196-110">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="28196-111">Možnost **Šifrovat pracovní soubory** je zapnutá automaticky.</span><span class="sxs-lookup"><span data-stu-id="28196-111">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="28196-112">Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="28196-112">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="28196-113">Rozbalte položku **obnovit data u zařízení systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="28196-113">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="28196-114">Doporučujeme **zapnout jej.**</span><span class="sxs-lookup"><span data-stu-id="28196-114">We recommend that you turn it **On**.</span></span>
    
    <span data-ttu-id="28196-115">Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit.</span><span class="sxs-lookup"><span data-stu-id="28196-115">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="28196-116">Pokyny naleznete v tématu [Vytvoření a ověření certifikátu agenta obnovení dat systému souborů EFS (Encrypting File System)](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="28196-116">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="28196-117">Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele.</span><span class="sxs-lookup"><span data-stu-id="28196-117">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="28196-118">Soubor může otevřít a dešifrovat jenom uživatel.</span><span class="sxs-lookup"><span data-stu-id="28196-118">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="28196-119">Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný.</span><span class="sxs-lookup"><span data-stu-id="28196-119">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="28196-120">Správce může dešifrovat soubor pomocí certifikátu agenta obnovování dat (DRA).</span><span class="sxs-lookup"><span data-stu-id="28196-120">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="28196-122">Chcete-li zajistit ochranu souborů ve všech uvedených aplikacích, rozbalte položku **Chraňte další místa v síti a shluku** , pokud chcete přidat další domény nebo umístění služby SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="28196-122">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="28196-123">Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="28196-123">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="28196-p105">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="28196-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="28196-127">Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="28196-127">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 