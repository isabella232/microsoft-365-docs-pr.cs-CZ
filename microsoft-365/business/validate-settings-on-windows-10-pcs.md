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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit nastavení ochrany aplikace Microsoft 365 Business app v zařízeních systému Windows 10.
ms.openlocfilehash: 5fed2278856f40233b142d3c7c4bc623e3777799
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575462"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="eb950-103">Ověření nastavení ochrany zařízení v počítačích se systémem Windows 10</span><span class="sxs-lookup"><span data-stu-id="eb950-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="eb950-104">Ověření, zda jsou nastaveny zásady zařízení systému Windows 10</span><span class="sxs-lookup"><span data-stu-id="eb950-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="eb950-105">Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může zásada trvat až několik hodin, než se zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="eb950-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="eb950-106">Můžete potvrdit, že se zásady projevily na různých obrazovkách nastavení systému Windows na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="eb950-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="eb950-107">Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení systému Windows Update a programu Windows Defender Antivirus na svých zařízeních systému Windows 10, bude mnoho těchto možností šedé.</span><span class="sxs-lookup"><span data-stu-id="eb950-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="eb950-108">Přejděte k **Nastavení** \> \*\*aktualizovat &amp; \*\* \> **Možnosti restartování** **systému Windows Update** \> a potvrďte, že všechna nastavení jsou šedá.</span><span class="sxs-lookup"><span data-stu-id="eb950-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Všechny možnosti restartování jsou zobrazeny šedě.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="eb950-110">Přejděte k **Nastavení** \> **aktualizace &amp; zabezpečení** \> v **systému Windows Update** \> **upřesňující možnosti** a potvrďte, že všechna nastavení jsou šedá.</span><span class="sxs-lookup"><span data-stu-id="eb950-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Možnosti rozšířené aktualizace systému Windows jsou všechny zobrazeny šedě.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="eb950-112">Přejít na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **upřesňující možnosti** \> **Zvolte způsob doručování aktualizací**.</span><span class="sxs-lookup"><span data-stu-id="eb950-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="eb950-113">Potvrďte, že je zobrazena zpráva (červeně), že některá nastavení jsou skryta nebo spravována organizací, a všechny možnosti jsou zobrazeny šedě.</span><span class="sxs-lookup"><span data-stu-id="eb950-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Volba způsobu doručování aktualizací indikuje, že nastavení jsou skryta nebo spravována organizací.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="eb950-115">Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte k **Nastavení** \> \*\* &amp; aktualizace zabezpečení\*\* \> **programu Windows Defender** \> klepněte na možnost **otevřít** \> \*\* &amp; vlákno programu Centrum zabezpečení Windows Defender ochrany\*\* \> **nastavení &amp; ochrany proti virům**.</span><span class="sxs-lookup"><span data-stu-id="eb950-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="eb950-116">Ověřte, zda jsou všechny možnosti zobrazeny šedě.</span><span class="sxs-lookup"><span data-stu-id="eb950-116">Verify that all options are greyed out.</span></span> 
    
    ![Nastavení ochrany proti virům a ohrožení je šedé.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="eb950-118">Příbuzná témata</span><span class="sxs-lookup"><span data-stu-id="eb950-118">Related Topics</span></span>

[<span data-ttu-id="eb950-119">Dokumentace a zdroje informací o Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="eb950-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="eb950-120">Začínáme s Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="eb950-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="eb950-121">Správa Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="eb950-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="eb950-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="eb950-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

