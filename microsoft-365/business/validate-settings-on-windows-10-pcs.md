---
title: Ověření nastavení ochrany aplikací pro Windows 10 počítače
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit, Microsoft 365 nastavení ochrany aplikací pro firmy na zařízeních Windows 10 uživatelů.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925253"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="2ff8f-103">Ověření nastavení ochrany zařízení pro Windows 10 počítače</span><span class="sxs-lookup"><span data-stu-id="2ff8f-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="2ff8f-104">Ověření, Windows 10 jsou nastavené zásady zařízení</span><span class="sxs-lookup"><span data-stu-id="2ff8f-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="2ff8f-105">Po nastavení [zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásada projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="2ff8f-106">Můžete potvrdit, že se zásady projeví, když se podíváme na Windows Nastavení obrazovkách na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="2ff8f-107">Vzhledem k tomu, že uživatelé nebudou moct změnit nastavení aktualizace Windows a Antivirová ochrana v programu Windows Defender na svých Windows 10 zařízeních, zobrazí se řada možností šedě.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="2ff8f-108">Přejděte na **Nastavení** Aktualizace zabezpečení Windows Možnosti restartování aktualizace a potvrďte, že jsou všechna \> **&amp;** \>  \>  nastavení šedá.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Všechny možnosti restartování jsou šedé.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="2ff8f-110">Přejděte na **Nastavení** Aktualizace zabezpečení Windows Upřesnit možnosti aktualizace a potvrďte, že jsou všechna \> **&amp;** \>  \>  nastavení šedá.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Rozšířené možnosti aktualizací jsou všechny šedé.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="2ff8f-112">Přejděte na **Nastavení** Aktualizace \> **&amp; zabezpečení** Windows Upřesnit možnosti Zvolte \>  \>  \> **způsob doručení aktualizací.**</span><span class="sxs-lookup"><span data-stu-id="2ff8f-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="2ff8f-113">Potvrďte, že vidíte zprávu (červeně), že některá nastavení jsou skrytá nebo spravovaná vaší organizací a všechny možnosti jsou šedé.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Výběr způsobu doručení aktualizací označuje, že nastavení je ve vaší organizaci skryté nebo spravované.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="2ff8f-115">Pokud chcete otevřít Windows Defender Security Center, přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Defender** na Otevřít \> Windows Defender Security **Center** \> **Ochrana &amp;** \> **&amp;** před viry Nastavení ochrany před viry .</span><span class="sxs-lookup"><span data-stu-id="2ff8f-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="2ff8f-116">Ověřte, jestli jsou všechny možnosti šedé.</span><span class="sxs-lookup"><span data-stu-id="2ff8f-116">Verify that all options are grayed out.</span></span> 
    
    ![Nastavení ochrany před viry a hrozbou jsou šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="2ff8f-118">Související témata</span><span class="sxs-lookup"><span data-stu-id="2ff8f-118">Related Topics</span></span>

[<span data-ttu-id="2ff8f-119">Microsoft 365 pro obchodní dokumentaci a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="2ff8f-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="2ff8f-120">Začínáme s Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="2ff8f-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="2ff8f-121">Správa Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="2ff8f-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="2ff8f-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="2ff8f-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
