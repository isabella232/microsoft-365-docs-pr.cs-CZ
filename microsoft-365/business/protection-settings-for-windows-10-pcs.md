---
title: Nastavení ochrany zařízení pro počítače s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Informace o výchozím nastavení a další nastavení, které jsou k dispozici v Microsoft Business 365 k zabezpečení zařízení Windows 10.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982141"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="e04a9-103">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="e04a9-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="e04a9-104">Zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="e04a9-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="e04a9-105">Podívejte se na video o tom, jak zabezpečit zařízení s Windows 10 s Microsoft 365 Business:</span><span class="sxs-lookup"><span data-stu-id="e04a9-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="e04a9-106">Přihlaste se k [Microsoft 365 Business](https://portal.office.com) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="e04a9-106">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="e04a9-107">V Centru pro správu přejděte na kartu **Zásady zařízení** a zvolte **Přidat zásadu**.</span><span class="sxs-lookup"><span data-stu-id="e04a9-107">in the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="e04a9-109">V podokně **Přidat zásadu** zadejte název, který je jedinečný.</span><span class="sxs-lookup"><span data-stu-id="e04a9-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="e04a9-110">V části **Typ zásady** zvolte **Konfigurace zařízení s Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="e04a9-110">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="e04a9-p101">Rozbalte **Zabezpečit zařízení s Windows 10** \> nakonfigurujte nastavení požadovaným způsobem. Další informace najdete v části [Dostupná nastavení](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings).</span><span class="sxs-lookup"><span data-stu-id="e04a9-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="e04a9-113">Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**.</span><span class="sxs-lookup"><span data-stu-id="e04a9-113">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="e04a9-p102">Dále zvolit **který toto nastavení obdrží?** Pokud nechcete použít výchozí skupinu zabezpečení **všech uživatelů** , zvolte **změnit**, vyhledejte skupinu zabezpečení, který bude toto nastavení získat \> **Vybrat**.</span><span class="sxs-lookup"><span data-stu-id="e04a9-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="e04a9-117">Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením.</span><span class="sxs-lookup"><span data-stu-id="e04a9-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="e04a9-118">Dostupná nastavení</span><span class="sxs-lookup"><span data-stu-id="e04a9-118">Available settings</span></span>

<span data-ttu-id="e04a9-p103">Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení.</span><span class="sxs-lookup"><span data-stu-id="e04a9-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="e04a9-121">Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="e04a9-121">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="e04a9-122">Nastavení</span><span class="sxs-lookup"><span data-stu-id="e04a9-122">Setting</span></span>  <br/> |<span data-ttu-id="e04a9-123">Popis</span><span class="sxs-lookup"><span data-stu-id="e04a9-123">Description</span></span>  <br/> |
|<span data-ttu-id="e04a9-124">Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="e04a9-124">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="e04a9-125">Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.</span><span class="sxs-lookup"><span data-stu-id="e04a9-125">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="e04a9-126">Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e04a9-126">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="e04a9-127">Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.</span><span class="sxs-lookup"><span data-stu-id="e04a9-127">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="e04a9-128">Použít pravidla k omezení potenciálních oblastí útoku na zařízení</span><span class="sxs-lookup"><span data-stu-id="e04a9-128">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="e04a9-p104">Pokud je omezování potenciálních oblastí útoku zapnuté, pomáhá blokovat akce a aplikace, které obvykle používá malware k napadnutí zařízení. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [omezování potenciálních oblastí útoku](https://go.microsoft.com/fwlink/?linkid=870417).  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="e04a9-132">Chránit složky před hrozbami, jako je ransomware</span><span class="sxs-lookup"><span data-stu-id="e04a9-132">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="e04a9-p105">Toto nastavení využívá řízený přístup ke složkám a chrání data společnosti před úpravami prostřednictvím podezřelých nebo škodlivých aplikací, jako je ransomware. Těmto typům aplikací se v chráněných složkách nepovolí provést změny. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [ochraně složek pomocí řízeného přístupu](https://go.microsoft.com/fwlink/?linkid=870418).  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="e04a9-137">Bránit síťovému přístupu k potenciálně škodlivému obsahu na internetu</span><span class="sxs-lookup"><span data-stu-id="e04a9-137">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="e04a9-p106">Pomocí tohoto nastavení můžete blokovat odchozí uživatelská připojení k umístěním na internetu s nízkou reputací, která můžou být hostiteli podvodů, útoků phishing, zneužití nebo jiného škodlivého obsahu. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [ochraně sítě](https://go.microsoft.com/fwlink/?linkid=870419).  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="e04a9-141">Chránit soubory a složky na počítačích před neoprávněným přístupem pomocí BitLockeru</span><span class="sxs-lookup"><span data-stu-id="e04a9-141">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="e04a9-p107">BitLocker chrání data tím, že šifruje pevné disky počítačů. Brání tak vyzrazení dat v případě ztráty nebo odcizení počítačů. Další informace najdete v [častých otázkách k BitLockeru](https://go.microsoft.com/fwlink/?linkid=871000).  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="e04a9-144">Povolit uživatelům stahovat aplikace z webu Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="e04a9-144">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="e04a9-p108">Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="e04a9-147">Umožnit uživatelům přístup ke Cortaně</span><span class="sxs-lookup"><span data-stu-id="e04a9-147">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="e04a9-p109">Cortana může být velice užitečná. Může vám zapínat nebo vypínat nastavení, dávat vám pokyny a postarat se o to, abyste chodili včas na schůzky. Proto jsme nastavení nechali implicitně **zapnuté**.  </span><span class="sxs-lookup"><span data-stu-id="e04a9-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="e04a9-150">Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="e04a9-150">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="e04a9-151">Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.</span><span class="sxs-lookup"><span data-stu-id="e04a9-151">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="e04a9-152">Automaticky aktualizovat zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="e04a9-152">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="e04a9-153">Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.</span><span class="sxs-lookup"><span data-stu-id="e04a9-153">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="e04a9-154">Vypnout obrazovku zařízení po nečinnosti</span><span class="sxs-lookup"><span data-stu-id="e04a9-154">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="e04a9-p110">Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.</span><span class="sxs-lookup"><span data-stu-id="e04a9-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

