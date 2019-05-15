---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit nastavení ochrany Microsoft 365 Business aplikace v zařízení Windows 10.
ms.openlocfilehash: 15c2d54c6281369875d15985c9d4ed16f0114176
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072224"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="c0c0c-103">Ověřit nastavení ochrany zařízení Windows 10 počítačů</span><span class="sxs-lookup"><span data-stu-id="c0c0c-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="c0c0c-104">Ověřte, zda jsou nastaveny zásady Windows 10 zařízení</span><span class="sxs-lookup"><span data-stu-id="c0c0c-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="c0c0c-105">Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat několik hodin zásady se projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="c0c0c-106">Můžete ověřit, že zásady ručitelského pohledem na různé obrazovky nastavení systému Windows na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="c0c0c-107">Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení služby Windows Update a Windows Defender Antivirus na jejich zařízeních Windows 10, mnoho z těchto možností bude šedé.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="c0c0c-108">Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Možnosti restartování** a potvrďte, že jsou všechna nastavení šedě.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Všechny možnosti restartování jsou označeny šedou barvou.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="c0c0c-110">Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Rozšířené možnosti** a potvrďte, že jsou všechna nastavení šedě.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Možnosti aktualizace Windows Advanced se všechny zobrazí šedě.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="c0c0c-112">Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Rozšířené možnosti** \> **zvolit způsob doručování aktualizací**.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="c0c0c-113">Potvrďte, že uvidíte zprávu (červeně), některá nastavení jsou skrytá nebo spravovány v organizaci a všech možností se zobrazí šedě.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Zvolit způsob doručování aktualizací stránky označuje nastavení skrytých nebo spravuje vaše organizace.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="c0c0c-115">Chcete-li otevřít Centrum zabezpečení systému Windows Defender, přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Program Windows Defender** \> klepněte na tlačítko **Spustit Centrum zabezpečení v aplikaci Windows Defender** \> **viru &amp; vlákna Ochrana** \> **viru &amp; ochrany proti novým ohrožením ochrany nastavení**.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="c0c0c-116">Ověřte, že všechny možnosti jsou označeny šedou barvou.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-116">Verify that all options are greyed out.</span></span> 
    
    ![Nastavení ochrany proti virům a ohrožením jsou označeny šedou barvou.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="c0c0c-118">Klepnutím na odkaz Příbuzná témata.</span><span class="sxs-lookup"><span data-stu-id="c0c0c-118">Related Topics</span></span>

[<span data-ttu-id="c0c0c-119">Dokumentace a zdroje informací o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c0c0c-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="c0c0c-120">Začínáme s Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c0c0c-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="c0c0c-121">Správa Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c0c0c-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="c0c0c-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="c0c0c-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

