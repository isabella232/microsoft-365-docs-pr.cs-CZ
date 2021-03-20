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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit, že se nastavení ochrany aplikací Microsoft 365 pro firmy projeví na zařízeních s Windows 10 vašich uživatelů.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912408"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="1e229-103">Ověření nastavení ochrany zařízení na počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="1e229-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="1e229-104">Ověření nastavení zásad zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="1e229-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="1e229-105">Po nastavení [zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásada projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="1e229-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="1e229-106">Můžete potvrdit, že se zásady projeví, když se podíváme na různé obrazovky nastavení Windows na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="1e229-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="1e229-107">Vzhledem k tomu, že uživatelé nebudou moct na svých zařízeních s Windows 10 upravovat nastavení Antivirové ochrany v programu Windows Update a Windows Defender, mnoho možností se zobrazí šedě.</span><span class="sxs-lookup"><span data-stu-id="1e229-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="1e229-108">Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **Možnosti restartování** a potvrďte, že jsou všechna nastavení šedá.</span><span class="sxs-lookup"><span data-stu-id="1e229-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Všechny možnosti restartování jsou šedé.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="1e229-110">Přejděte na **Nastavení Aktualizace** zabezpečení Windows Update – upřesnit možnosti a ověřte, že všechna nastavení \> **&amp;** jsou \>  \>  šedá.</span><span class="sxs-lookup"><span data-stu-id="1e229-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Možnosti upřesňujících aktualizací systému Windows jsou všechny šedé.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="1e229-112">Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **– upřesnit možnosti** \> **Zvolte způsob doručení aktualizací.**</span><span class="sxs-lookup"><span data-stu-id="1e229-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="1e229-113">Potvrďte, že vidíte zprávu (červeně), že některá nastavení jsou skrytá nebo spravovaná vaší organizací a všechny možnosti jsou šedé.</span><span class="sxs-lookup"><span data-stu-id="1e229-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Výběr způsobu doručení aktualizací označuje, že nastavení je ve vaší organizaci skryté nebo spravované.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="1e229-115">Pokud chcete otevřít Centrum zabezpečení  v programu Windows Defender, přejděte na Nastavení Aktualizace zabezpečení Windows Defenderu klikněte na Otevřít Centrum zabezpečení v programu Windows Defender Ochrana proti virům ochrana před vlákny \> **&amp;** Nastavení \>  \> ochrany  \> **&amp;** \> **&amp; před viry**.</span><span class="sxs-lookup"><span data-stu-id="1e229-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="1e229-116">Ověřte, jestli jsou všechny možnosti šedé.</span><span class="sxs-lookup"><span data-stu-id="1e229-116">Verify that all options are grayed out.</span></span> 
    
    ![Nastavení ochrany před viry a hrozbou jsou šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="1e229-118">Související témata</span><span class="sxs-lookup"><span data-stu-id="1e229-118">Related Topics</span></span>

[<span data-ttu-id="1e229-119">Dokumentace a materiály k Microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="1e229-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="1e229-120">Začínáme s Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="1e229-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="1e229-121">Správa Microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="1e229-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="1e229-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="1e229-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
