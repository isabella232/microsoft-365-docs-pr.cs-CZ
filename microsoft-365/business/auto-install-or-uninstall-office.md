---
title: Automatická instalace nebo odinstalace Office na zařízeních s Windows 10
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
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Instalace nebo odinstalování sady Office v zařízení Windows 10 z středisku pro správce Microsoft 365 Business. '
ms.openlocfilehash: 997c001ed1520f1ac989255632d36f9b7bedd16c
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983331"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="38916-103">Automatická instalace nebo odinstalace Office na zařízeních s Windows 10</span><span class="sxs-lookup"><span data-stu-id="38916-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="38916-104">K rychlé a jednoduché instalaci Office na počítače s Windows 10 můžete použít Centrum pro správu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="38916-104">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="38916-105">Pokud se chcete dozvědět, jak to funguje s dříve nainstalovanými aplikacemi Office, napřed si přečtěte článek [Příprava instalace klienta Office](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="38916-105">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="38916-106">Správa nasazení Office</span><span class="sxs-lookup"><span data-stu-id="38916-106">Manage Office deployments</span></span>

1. <span data-ttu-id="38916-107">Přihlaste se do [Centra pro správu](https://aka.ms/bcsportal) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="38916-107">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="38916-p101">Na kartě **zařízení** zvolte **Spravovat nasazení sady Office**.    Pokud není zobrazena karta **Akce zařízení** v **domovské** stránky admin center klepněte na tlačítko **Přidat** (+) přidat do admin domácí.</span><span class="sxs-lookup"><span data-stu-id="38916-p101">On the **Devices** card, choose **Manage Office Deployment**.    If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="38916-111">V otevřeném podokně **Spravovat nasazení Office** zvolte **Přidat skupinu** a vyberte skupiny, které chcete použít.</span><span class="sxs-lookup"><span data-stu-id="38916-111">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="38916-112">Po přidání jedné nebo více skupin, které chcete použít, vyberte v rozevíracím seznamu **Akce nasazení** buď **Co nejdříve si nainstalujte Office**, nebo **Odinstalovat Office**.</span><span class="sxs-lookup"><span data-stu-id="38916-112">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="38916-114">Zvolte **Další** \> zkontrolujte nastavení a pak zvolte **Potvrdit**.</span><span class="sxs-lookup"><span data-stu-id="38916-114">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="38916-115">32bitová verze Office se automaticky nainstaluje nebo odinstaluje v zařízeních vlastněných uživateli, kteří jsou zařazení do jedné nebo několika použitých skupin.</span><span class="sxs-lookup"><span data-stu-id="38916-115">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="38916-116">Pokud chcete automatickou instalaci zkontrolovat, otevřete na počítači, který byl vybrán pro instalaci Office, Správce úloh a zkontrolujte, že je na něm proces Microsoft Office Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="38916-116">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


