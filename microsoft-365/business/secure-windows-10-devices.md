---
title: Zabezpečení zařízení s Windows 10
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
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
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Přečtěte si informace o konfiguraci nastavení výchozích zásad zařízení, které bude každé zařízení s Windows 10 dostávat po přihlášení ke svému pracovnímu nebo školnímu účtu.
ms.openlocfilehash: 86db1c152f9f6ac1fe6093b4a55a74b69fbd8b0f
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579968"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="f3934-103">Zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="f3934-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="f3934-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f3934-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f3934-105">[] Nastavení, která tady nakonfigurujete, jsou součástí výchozí zásady zařízení pro Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f3934-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="f3934-106">Všichni uživatelé, kteří připojují zařízení s Windows 10, včetně mobilních zařízení a počítačů, když se přihlásí pomocí svého pracovního účtu, dostanou tato nastavení automaticky.</span><span class="sxs-lookup"><span data-stu-id="f3934-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="f3934-107">Doporučujeme vám během instalace přijmou výchozí zásady a další zásady, které budou cílit na konkrétní skupiny uživatelů, přidat později.</span><span class="sxs-lookup"><span data-stu-id="f3934-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="f3934-108">Nastavení pro zabezpečení zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="f3934-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="f3934-p102">Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="f3934-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="f3934-111">Nastavení</span><span class="sxs-lookup"><span data-stu-id="f3934-111">Setting</span></span>  <br/> |<span data-ttu-id="f3934-112">Popis</span><span class="sxs-lookup"><span data-stu-id="f3934-112">Description</span></span>  <br/> |
|<span data-ttu-id="f3934-113">Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender</span><span class="sxs-lookup"><span data-stu-id="f3934-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="f3934-114">Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.</span><span class="sxs-lookup"><span data-stu-id="f3934-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="f3934-115">Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f3934-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="f3934-116">Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.</span><span class="sxs-lookup"><span data-stu-id="f3934-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="f3934-117">Chránit soubory a složky na počítačích před neoprávněným přístupem pomocí BitLockeru</span><span class="sxs-lookup"><span data-stu-id="f3934-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="f3934-118">Nástroj BitLocker chrání data šifrováním pevných disků počítače a chrání před vystavením datům, pokud dojde ke ztrátě nebo odcizení počítače.</span><span class="sxs-lookup"><span data-stu-id="f3934-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="f3934-119">Další informace najdete v článku [Časté otázky k nástroji Bitlocker.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)</span><span class="sxs-lookup"><span data-stu-id="f3934-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="f3934-120">Vypnout obrazovku zařízení po nečinnosti</span><span class="sxs-lookup"><span data-stu-id="f3934-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="f3934-p104">Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.</span><span class="sxs-lookup"><span data-stu-id="f3934-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|