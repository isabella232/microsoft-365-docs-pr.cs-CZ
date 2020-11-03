---
title: Zvýšení ochrany před hrozbami pro Microsoft 365 Business Premium
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Nastavení funkcí pro dodržování předpisů pro ochranu před ztrátou dat a zachování důvěrných informací a vašich zákazníků.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841167"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="be4c8-103">Nastavení funkcí pro dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="be4c8-103">Set up compliance features</span></span>

<span data-ttu-id="be4c8-104">Společnost Microsoft 365 Business Premium přichází s funkcemi pro ochranu vašich dat a zařízení a pomáhá zabezpečit citlivé informace a vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="be4c8-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="be4c8-105">Nastavení funkcí ochrany před únikem informací</span><span class="sxs-lookup"><span data-stu-id="be4c8-105">Set up DLP features</span></span>

<span data-ttu-id="be4c8-106">Další informace o tom, jak nastavit zásadu pro ochranu před ztrátou osobních údajů, najdete v tématu [Vytvoření zásad DLP ze šablony](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) .</span><span class="sxs-lookup"><span data-stu-id="be4c8-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="be4c8-107">Technologie DLP přináší mnoho šablon zásad připravených k použití pro mnoho různých národních prostředí.</span><span class="sxs-lookup"><span data-stu-id="be4c8-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="be4c8-108">Například Austrálie finanční data, Kanada – osobní údaje, finanční údaje USA a další.</span><span class="sxs-lookup"><span data-stu-id="be4c8-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="be4c8-109">Podívejte [se, jaké jsou šablony zásad DLP](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) pro úplný seznam.</span><span class="sxs-lookup"><span data-stu-id="be4c8-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="be4c8-110">Všechny tyto šablony můžou být povolené v příkladu šablony PII.</span><span class="sxs-lookup"><span data-stu-id="be4c8-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="be4c8-111">Nastavení uchovávání e-mailů s archivací Exchange Online</span><span class="sxs-lookup"><span data-stu-id="be4c8-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="be4c8-112">Funkce **archivace licencí na Exchange Online** pomáhají udržovat dodržování předpisů v e-mailu pro eDiscovery na základě souladu s pravidly pro správu shody.</span><span class="sxs-lookup"><span data-stu-id="be4c8-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="be4c8-113">Pomáhá také snížit vaše riziko, pokud se jedná o soudní řízení a způsob, jak obnovit data po porušení zabezpečení nebo když potřebujete obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="be4c8-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="be4c8-114">Chcete-li zachovat veškerý obsah uživatele, můžete použít podržení sporu, nebo můžete pomocí zásad uchovávání informací přizpůsobit, co chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="be4c8-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="be4c8-115">**Držení sporu:** Všechny poštovní schránky, včetně odstraněných položek, můžete zachovat tak, že zadáte celou poštovní schránku uživatele na blokování soudního sporu.</span><span class="sxs-lookup"><span data-stu-id="be4c8-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="be4c8-116">Umístění poštovní schránky v centru pro správu – blokování soudního sporu:</span><span class="sxs-lookup"><span data-stu-id="be4c8-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="be4c8-117">V levém navigačním panelu přejděte na **Uživatelé** \> **aktivní uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="be4c8-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="be4c8-118">Vyberte uživatele, jehož poštovní schránku chcete umístit na přihlášeného.</span><span class="sxs-lookup"><span data-stu-id="be4c8-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="be4c8-119">V podokně uživatel rozbalte položku **Nastavení pošty** a vedle **Možnosti další nastavení** zvolte **Upravit vlastnosti Exchange**.</span><span class="sxs-lookup"><span data-stu-id="be4c8-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="be4c8-120">Na stránce poštovní schránky pro uživatele zvolte \* \* funkce poštovní schránky \* \* na levém navigačním panelu a pak zvolte **Povolit** odkaz v části **pozdržení sporu**.</span><span class="sxs-lookup"><span data-stu-id="be4c8-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="be4c8-121">V dialogovém okně **podržet soudní spor** můžete určit dobu trvání držení pro soudní řízení v poli **Doba trvání přidržení** .</span><span class="sxs-lookup"><span data-stu-id="be4c8-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="be4c8-122">Pokud chcete umístit nekonečné blokování, nechte pole prázdné.</span><span class="sxs-lookup"><span data-stu-id="be4c8-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="be4c8-123">Můžete taky přidat poznámky a směrovat vlastníka poštovní schránky na web, možná budete muset vysvětlit Další informace o přístupnosti.</span><span class="sxs-lookup"><span data-stu-id="be4c8-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="be4c8-124">\>**Uložit**.</span><span class="sxs-lookup"><span data-stu-id="be4c8-124">\> **Save**.</span></span>
    
<span data-ttu-id="be4c8-125">**Uchovávání informací:** Můžete povolit zásady uchovávání informací, například zachovat po určitou dobu nebo trvale odstranit obsah na konci období uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="be4c8-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="be4c8-126">Další informace najdete v tématu [Přehled zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="be4c8-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="be4c8-127">Nastavit popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="be4c8-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="be4c8-128">Popisky citlivosti jsou součástí služby Azure Information Protection (AIP) plán 1 a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily použitím popisků.</span><span class="sxs-lookup"><span data-stu-id="be4c8-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="be4c8-129">Štítky můžou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživatelé nebo používají kombinaci, kde jsou uživatelům nabídnuta doporučení.</span><span class="sxs-lookup"><span data-stu-id="be4c8-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="be4c8-130">Pokud chcete nastavit popisky citlivosti, zobrazte si [možnosti vytvořit a spravovat](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video s popisky.</span><span class="sxs-lookup"><span data-stu-id="be4c8-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="be4c8-131">Ruční instalace klienta služby Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="be4c8-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="be4c8-132">Postup ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="be4c8-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="be4c8-133">Stáhněte si **AzinfoProtection_UL.exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="be4c8-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="be4c8-134">Instalaci můžete ověřit tak, že zobrazíte wordový dokument a zajistíte, že je na kartě **Domů** dostupná možnost **Citlivost** .</span><span class="sxs-lookup"><span data-stu-id="be4c8-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="be4c8-135">![Rozevírací seznam karty zámek ve wordovém dokumentu](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="be4c8-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="be4c8-136">Další informace najdete v článku [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="be4c8-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
