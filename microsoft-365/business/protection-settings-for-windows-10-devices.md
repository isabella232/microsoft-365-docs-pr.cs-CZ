---
title: Úprava nebo nastavení ochrany aplikací pro zařízení s Windows 10
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
description: Zjistěte, jak vytvářet nebo upravovat zásady správy aplikací a chránit pracovní soubory na osobních zařízeních s Windows 10 vašich uživatelů.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912816"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="2b2df-103">Nastavení nebo úpravy nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="2b2df-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="2b2df-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2b2df-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="2b2df-105">Úprava zásad správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="2b2df-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="2b2df-106">Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="2b2df-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="2b2df-107">V levém navigačním panelu zvolte **Zásady** \> **zařízení** .</span><span class="sxs-lookup"><span data-stu-id="2b2df-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="2b2df-108">Zvolte existující zásady aplikace pro Windows a pak **Upravit**.</span><span class="sxs-lookup"><span data-stu-id="2b2df-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="2b2df-109">Vedle **nastavení,** které chcete změnit, zvolte Upravit a pak **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="2b2df-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="2b2df-110">Vytvoření zásady správy aplikací pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="2b2df-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="2b2df-111">Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="2b2df-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="2b2df-112">Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="2b2df-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="2b2df-113">V levém navigačním panelu zvolte **Přidat** \> **zásady** \> **zařízení.**</span><span class="sxs-lookup"><span data-stu-id="2b2df-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="2b2df-114">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="2b2df-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="2b2df-115">V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="2b2df-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="2b2df-116">V **části Typ zařízení** zvolte Osobní nebo **Vlastněné společností**. </span><span class="sxs-lookup"><span data-stu-id="2b2df-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="2b2df-117">Možnost **Šifrovat pracovní soubory** je zapnutá automaticky.</span><span class="sxs-lookup"><span data-stu-id="2b2df-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="2b2df-118">Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="2b2df-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="2b2df-119">Rozbalte **obnovit data na zařízeních s Windows.**</span><span class="sxs-lookup"><span data-stu-id="2b2df-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="2b2df-120">Doporučujeme ho **zapnout.**</span><span class="sxs-lookup"><span data-stu-id="2b2df-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="2b2df-121">Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit.</span><span class="sxs-lookup"><span data-stu-id="2b2df-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="2b2df-122">Pokyny najdete v tématu Vytvoření a ověření certifikátu Agenta obnovení dat [systému souborů EFS (Encrypting File System) (DRA).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)</span><span class="sxs-lookup"><span data-stu-id="2b2df-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="2b2df-123">Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele.</span><span class="sxs-lookup"><span data-stu-id="2b2df-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="2b2df-124">Soubor může otevřít a dešifrovat jenom uživatel.</span><span class="sxs-lookup"><span data-stu-id="2b2df-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="2b2df-125">Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný.</span><span class="sxs-lookup"><span data-stu-id="2b2df-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="2b2df-126">Správce může k dešifrování souboru použít certifikát Agenta obnovení dat (DRA).</span><span class="sxs-lookup"><span data-stu-id="2b2df-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="2b2df-128">Pokud **chcete přidat** další domény nebo umístění SharePointu Online, abyste měli jistotu, že jsou soubory ve všech uvedených aplikacích chráněné, rozbalte Zamknout další síťová a cloudová umístění.</span><span class="sxs-lookup"><span data-stu-id="2b2df-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="2b2df-129">Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="2b2df-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="2b2df-p104">V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="2b2df-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="2b2df-133">Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="2b2df-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>