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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Přečtěte si, jak ověřit, že nastavení ochrany aplikací Microsoftu 365 pro firmy se projevilo na zařízeních uživatelů s Windows 10.
ms.openlocfilehash: b63681f040b0fe49127693e9cb7aac7ba6c41af6
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635698"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="53986-103">Ověření nastavení ochrany zařízení v počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="53986-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="53986-104">Ověření nastavené zásady zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="53986-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="53986-105">Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="53986-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="53986-106">Můžete potvrdit, že zásady se projevily, a to tak, že se podíváte na různé obrazovky Nastavení systému Windows na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="53986-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="53986-107">Vzhledem k tomu, že uživatelé nebudou moci na svých zařízeních se systémem Windows 10 upravovat nastavení programu Windows Update a programu Windows Defender, bude mnoho možností zobrazeno šedě.</span><span class="sxs-lookup"><span data-stu-id="53986-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="53986-108">Přejděte na **možnosti** \*\*zabezpečení aktualizace &amp; \*\* \> **Nastavení** \> **Windows Update** \> Restart a zkontrolujte, zda jsou všechna nastavení zobrazena šedě.</span><span class="sxs-lookup"><span data-stu-id="53986-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Všechny možnosti restartování jsou šedě.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="53986-110">Přejděte na **možnosti &amp; zabezpečení** \> aktualizace **nastavení** \> **služby Windows Update** \> **Upřesňující možnosti** a potvrďte, že všechna nastavení jsou zašedlá.</span><span class="sxs-lookup"><span data-stu-id="53986-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Možnosti rozšířených aktualizací systému Windows jsou všechny zobrazeny šedě.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="53986-112">Přejděte na **zabezpečení aktualizace** \> \> \> \> **Advanced options** \*\* &amp; \*\* nastavení **Možnosti Windows Update** **Upřesnit způsob doručení aktualizací**.</span><span class="sxs-lookup"><span data-stu-id="53986-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="53986-113">Zkontrolujte, zda se zobrazí zpráva (červeně), že některá nastavení jsou skryta nebo spravována vaší organizací, a že všechny možnosti jsou zobrazeny šedě.</span><span class="sxs-lookup"><span data-stu-id="53986-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Zvolte způsob doručení aktualizací, protože nastavení je skryto nebo spravuje vaše organizace.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="53986-115">Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte na **položku** \> Zabezpečení \> **aktualizace &amp; \*\* nastavení **programu Windows Defender** \> klepněte na tlačítko **Otevřít program Windows Defender Security Center** \> **Ochrana &amp; vláken Ochrana vláken Ochrana** \> \*\* &amp; před virovou ochranou proti ohrožení mantinela**.</span><span class="sxs-lookup"><span data-stu-id="53986-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="53986-116">Ověřte, zda jsou všechny možnosti zobrazeny šedě.</span><span class="sxs-lookup"><span data-stu-id="53986-116">Verify that all options are grayed out.</span></span> 
    
    ![Nastavení ochrany proti virům a hrozbám jsou zobrazena šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="53986-118">Příbuzná témata</span><span class="sxs-lookup"><span data-stu-id="53986-118">Related Topics</span></span>

[<span data-ttu-id="53986-119">Microsoft 365 pro obchodní dokumentaci a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="53986-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="53986-120">Začínáme s Microsoftem 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="53986-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="53986-121">Správa Microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="53986-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="53986-122">Nastavení konfigurací zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="53986-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

