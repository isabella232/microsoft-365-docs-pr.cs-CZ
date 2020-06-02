---
title: Nastavení ochrany aplikací pro zařízení s Windows 10
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Přečtěte si, jak vytvořit zásady správy aplikací a chránit pracovní soubory na osobních zařízeních s Windows 10 uživatelů.
ms.openlocfilehash: df10470c6bd7aad2f35700a267c4d24d949f569c
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470861"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="cf59b-103">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf59b-103">Set application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="cf59b-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf59b-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="cf59b-105">Vytvoření zásady správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf59b-105">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="cf59b-106">Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="cf59b-106">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="cf59b-107">Přejděte do centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="cf59b-107">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="cf59b-108">V levém navigačním zařízení zvolte **Přidat** \> **zásady zařízení** \> **Add**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="cf59b-109">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="cf59b-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="cf59b-110">V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="cf59b-111">V části **Typ zařízení**zvolte **osobní** nebo **vlastněné společnosti**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-111">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="cf59b-112">Možnost **Šifrovat pracovní soubory** je zapnutá automaticky.</span><span class="sxs-lookup"><span data-stu-id="cf59b-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="cf59b-113">Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="cf59b-114">Rozbalte **možnost Obnovit data na zařízeních se systémem Windows**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-114">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="cf59b-115">Doporučujeme jej zapnout **.**</span><span class="sxs-lookup"><span data-stu-id="cf59b-115">We recommend that you turn it **On**.</span></span>
    
    <span data-ttu-id="cf59b-116">Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit.</span><span class="sxs-lookup"><span data-stu-id="cf59b-116">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="cf59b-117">Pokyny naleznete v [tématu Vytvoření a ověření certifikátu AGENT OBNOVENÍ DAT (EFS) systému EFS](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="cf59b-117">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="cf59b-118">Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele.</span><span class="sxs-lookup"><span data-stu-id="cf59b-118">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="cf59b-119">Soubor může otevřít a dešifrovat jenom uživatel.</span><span class="sxs-lookup"><span data-stu-id="cf59b-119">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="cf59b-120">Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný.</span><span class="sxs-lookup"><span data-stu-id="cf59b-120">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="cf59b-121">Správce může k dešifrování souboru použít certifikát DRA (Data Recovery Agent).</span><span class="sxs-lookup"><span data-stu-id="cf59b-121">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="cf59b-123">Pokud chcete přidat další domény nebo umístění SharePointu Online, rozbalte možnost **Chránit další umístění v síti a cloudu,** abyste měli jistotu, že jsou soubory ve všech uvedených aplikacích chráněné.</span><span class="sxs-lookup"><span data-stu-id="cf59b-123">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="cf59b-124">Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="cf59b-124">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="cf59b-p105">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="cf59b-p105">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="cf59b-128">Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="cf59b-128">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
