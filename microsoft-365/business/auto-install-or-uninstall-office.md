---
title: Automatická instalace nebo odinstalace Office na zařízeních s Windows 10
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Nainstalujte nebo odinstalujte sadu Office u zařízení Windows 10 z centra Business admin společnosti Microsoft 365. '
ms.openlocfilehash: 70fd2f1ded87e04f506b1ba415c820af5d535938
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121252"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="67f05-103">Automatická instalace nebo odinstalace Office na zařízeních s Windows 10</span><span class="sxs-lookup"><span data-stu-id="67f05-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="67f05-104">[![Popisek vám dá vědět, že se centrum pro správu mění a další podrobnosti naleznete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="67f05-104">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="67f05-105">K rychlé a jednoduché instalaci Office na počítače s Windows 10 můžete použít Centrum pro správu Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="67f05-105">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="67f05-106">Pokud se chcete dozvědět, jak to funguje s dříve nainstalovanými aplikacemi Office, napřed si přečtěte článek [Příprava instalace klienta Office](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="67f05-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="67f05-107">Správa nasazení Office</span><span class="sxs-lookup"><span data-stu-id="67f05-107">Manage Office deployments</span></span>

1. <span data-ttu-id="67f05-108">Přihlaste se do [Centra pro správu](https://aka.ms/bcsportal) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="67f05-108">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="67f05-109">Na kartě **Zařízení** zvolte **Spravovat nasazení Office**.</span><span class="sxs-lookup"><span data-stu-id="67f05-109">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="67f05-110">Není-li karta **Akce zařízení** zobrazena, klepněte na **domovské** stránce centra pro správu na tlačítko **Přidat** (+) a přidejte je do domovského adresáře.</span><span class="sxs-lookup"><span data-stu-id="67f05-110">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="67f05-112">V otevřeném podokně **Spravovat nasazení Office** zvolte **Přidat skupinu** a vyberte skupiny, které chcete použít.</span><span class="sxs-lookup"><span data-stu-id="67f05-112">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="67f05-113">Po přidání jedné nebo více skupin, které chcete použít, vyberte v rozevíracím seznamu **Akce nasazení** buď **Co nejdříve si nainstalujte Office**, nebo **Odinstalovat Office**.</span><span class="sxs-lookup"><span data-stu-id="67f05-113">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="67f05-115">Zvolte **Další** \> zkontrolujte nastavení a pak zvolte **Potvrdit**.</span><span class="sxs-lookup"><span data-stu-id="67f05-115">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="67f05-116">32bitová verze Office se automaticky nainstaluje nebo odinstaluje v zařízeních vlastněných uživateli, kteří jsou zařazení do jedné nebo několika použitých skupin.</span><span class="sxs-lookup"><span data-stu-id="67f05-116">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="67f05-117">Pokud chcete automatickou instalaci zkontrolovat, otevřete na počítači, který byl vybrán pro instalaci Office, Správce úloh a zkontrolujte, že je na něm proces Microsoft Office Klikni a spusť.</span><span class="sxs-lookup"><span data-stu-id="67f05-117">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


