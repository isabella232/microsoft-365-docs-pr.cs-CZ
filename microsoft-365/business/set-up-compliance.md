---
title: Zvyšte ochranu proti ohrožení společnosti Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Nastavte funkce kompatibility tak, aby nedocházelo ke ztrátám dat a k popisu citlivých dat.
ms.openlocfilehash: 73709c1302a2e9e46eb2d54ea021438b5f1743c5
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575652"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="0426f-103">Nastavení funkcí kompatibility</span><span class="sxs-lookup"><span data-stu-id="0426f-103">Set up compliance features</span></span>

<span data-ttu-id="0426f-104">Společnost Microsoft 365 Business obsahuje funkce pro ochranu dat a zařízení a pomáhá zabezpečit vaše a citlivé informace zákazníků.</span><span class="sxs-lookup"><span data-stu-id="0426f-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="0426f-105">Nastavení funkcí DLP</span><span class="sxs-lookup"><span data-stu-id="0426f-105">Set up DLP features</span></span>

<span data-ttu-id="0426f-106">Viz [Vytvoření zásady DLP ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) pro příklad, jak nastavit zásady ochrany proti osobním identifikovatelným informacím (PII).</span><span class="sxs-lookup"><span data-stu-id="0426f-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="0426f-107">DLP přináší mnoho šablon zásad připravených k použití pro mnoho různých národních prostředí.</span><span class="sxs-lookup"><span data-stu-id="0426f-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="0426f-108">Například australské finanční údaje, zákon o osobním informování Kanady, finanční data USA atd. Podívejte [se, co šablony zásad DLP obsahují](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pro úplný seznam.</span><span class="sxs-lookup"><span data-stu-id="0426f-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="0426f-109">Všechny tyto šablony lze povolit podobným příkladem šablony PII.</span><span class="sxs-lookup"><span data-stu-id="0426f-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="0426f-110">Nastavení uchování e-mailu pomocí archivace online serveru Exchange</span><span class="sxs-lookup"><span data-stu-id="0426f-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="0426f-111">Funkce pro **archivaci online systému Exchange** pomáhá udržovat dodržování a regulační standardy zachováním obsahu e-mailu pro program eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="0426f-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="0426f-112">Pomáhá také snižovat riziko v případě žaloby a poskytuje způsob, jak obnovit data po porušení zabezpečení nebo kdy je nutné obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="0426f-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="0426f-113">Chcete-li zachovat veškerý obsah uživatele nebo pomocí zásad uchovávání informací upravit, co chcete zachovat, můžete použít blokování sporů.</span><span class="sxs-lookup"><span data-stu-id="0426f-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="0426f-114">**Soudní spor:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat umístěním celé poštovní schránky uživatele do blokování soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="0426f-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="0426f-115">Chcete-li umístit poštovní schránku na soudní řízení, v centru pro správu:</span><span class="sxs-lookup"><span data-stu-id="0426f-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="0426f-116">V levém navigačním poli přejděte na **uživatele** \> **Active Users**.</span><span class="sxs-lookup"><span data-stu-id="0426f-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="0426f-117">Vyberte uživatele, jehož poštovní schránku chcete umístit do soudního sporu, a v uživatelském podokně rozbalte **Nastavení pošty** a vedle **dalších nastavení** zvolte možnost **Upravit vlastnosti serveru Exchange**.</span><span class="sxs-lookup"><span data-stu-id="0426f-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="0426f-118">Na stránce poštovní schránky uživatele zvolte \* \* funkce poštovní schránky \* \* na levém navigačním panelu a pak zvolte možnost **Povolit** odkaz v rámci **soudního sporu**.</span><span class="sxs-lookup"><span data-stu-id="0426f-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="0426f-119">V dialogovém okně **soudní spor** můžete určit dobu trvání v poli **Doba trvání soudního** sporu, ponechat pole prázdné, chcete-li umístit nekonečné blokování.</span><span class="sxs-lookup"><span data-stu-id="0426f-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="0426f-120">Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který bude pravděpodobně nutné objasnit \> **uložení**tohoto sporu.</span><span class="sxs-lookup"><span data-stu-id="0426f-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="0426f-121">**Uchovávání informací:** Můžete povolit vlastní zásady uchovávání informací, například chcete-li zachovat určitou dobu nebo trvale odstranit obsah na konci retenční periody.</span><span class="sxs-lookup"><span data-stu-id="0426f-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="0426f-122">Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="0426f-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="0426f-123">Nastavit popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="0426f-123">Set up Sensitivity labels</span></span>

<span data-ttu-id="0426f-124">Štítky s citlivostí jsou součástí plánu 1 Azure Information Protection (AIP) a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily pomocí popisků.</span><span class="sxs-lookup"><span data-stu-id="0426f-124">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="0426f-125">Štítky mohou být automaticky použity správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, v níž jsou uživatelům poskytnuta doporučení.</span><span class="sxs-lookup"><span data-stu-id="0426f-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="0426f-126">Chcete-li nastavit popisky citlivosti, zobrazte [Vytvoření a správu popisků citlivosti](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videa.</span><span class="sxs-lookup"><span data-stu-id="0426f-126">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="0426f-127">Ruční instalace klienta ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="0426f-127">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="0426f-128">Ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="0426f-128">To manually install the AIP client:</span></span>

1. <span data-ttu-id="0426f-129">Stáhněte **AzinfoProtection_UL. exe** z [webu služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="0426f-129">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="0426f-130">Instalaci můžete ověřit zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **Citlivost** .</span><span class="sxs-lookup"><span data-stu-id="0426f-130">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="0426f-131">![Rozevírací karta zámku v dokumentu aplikace Word.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="0426f-131">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="0426f-132">Další informace naleznete v části [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="0426f-132">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
