---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
f1.keywords:
- NOCSH
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Přečtěte si, jak ověřit nastavení ochrany aplikací Microsoft 365 Business na zařízeních s Windows 10.
ms.openlocfilehash: 1762382aec00a80e006cf38b66c28d02c0c25989
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42056637"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="944e1-103">Ověření nastavení ochrany zařízení v počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="944e1-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="944e1-104">Ověření nastavení zásad zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="944e1-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="944e1-105">Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="944e1-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="944e1-106">Zásady se projevily na různých obrazovkách nastavení systému Windows v zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="944e1-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="944e1-107">Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení Windows Update a Windows Defender Antivirus na svých zařízeních s Windows 10, mnoho možností bude šedě.</span><span class="sxs-lookup"><span data-stu-id="944e1-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="944e1-108">Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> Restart **možnosti** a zkontrolujte, zda všechna nastavení jsou šedě.</span><span class="sxs-lookup"><span data-stu-id="944e1-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Všechny možnosti restartování jsou šedě.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="944e1-110">Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **Upřesnit možnosti** a zkontrolujte, zda všechna nastavení jsou šedě.</span><span class="sxs-lookup"><span data-stu-id="944e1-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Možnosti aktualizací rozšířené systému Windows jsou zobrazeny šedě.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="944e1-112">Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Rozšířené možnosti** \> **služby Windows Update** \> **Zvolte způsob doručení aktualizací**.</span><span class="sxs-lookup"><span data-stu-id="944e1-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="944e1-113">Zkontrolujte, zda se zobrazí zpráva (červeně), že některá nastavení jsou skryta nebo spravována vaší organizací a všechny možnosti jsou šedě.</span><span class="sxs-lookup"><span data-stu-id="944e1-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Zvolte, jak jsou aktualizace doručovány, na stránce indikuje, že nastavení jsou skrytá nebo spravovaná vaší organizací.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="944e1-115">Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte **na** \> \*\*nastavení zabezpečení aktualizace &amp; \*\* \> **Windows Defender,** \> klepněte na příkaz Otevřít program Windows **Defender Security Center** \> **Anti &amp; thread protection** \> \*\*Anti-hrozeb &amp; \*\*.</span><span class="sxs-lookup"><span data-stu-id="944e1-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="944e1-116">Ověřte, zda jsou všechny možnosti šedě.</span><span class="sxs-lookup"><span data-stu-id="944e1-116">Verify that all options are grayed out.</span></span> 
    
    ![Nastavení ochrany proti virům a hrozbám je šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="944e1-118">Související témata</span><span class="sxs-lookup"><span data-stu-id="944e1-118">Related Topics</span></span>

[<span data-ttu-id="944e1-119">Dokumentace a zdroje informací o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="944e1-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="944e1-120">Začínáme s Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="944e1-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="944e1-121">Správa Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="944e1-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="944e1-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="944e1-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

