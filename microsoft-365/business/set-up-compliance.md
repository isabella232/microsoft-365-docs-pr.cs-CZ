---
title: Zvýšení ochrany před hrozbami pro Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a zajistili bezpečnost citlivých informací vašich zákazníků.
ms.openlocfilehash: 6f4520b052c2e7acb8748d3c9d6e26777cb56d4b
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561234"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="2f9e6-103">Nastavení funkcí dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="2f9e6-103">Set up compliance features</span></span>

<span data-ttu-id="2f9e6-104">Microsoft 365 Business je vybaven funkcemi, které chrání vaše data a zařízení a pomáhají vám zabezpečit citlivé informace vašich i zákazníků.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="2f9e6-105">Nastavení funkcí programu DLP</span><span class="sxs-lookup"><span data-stu-id="2f9e6-105">Set up DLP features</span></span>

<span data-ttu-id="2f9e6-106">Příklad, jak nastavit zásadu ochrany před únikem informací ze šablony, najdete v tématu [Vytvoření zásady ochrany před únikem](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) informací(PII).</span><span class="sxs-lookup"><span data-stu-id="2f9e6-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="2f9e6-107">DLP je dodáván s mnoha připravenými šablonami zásad pro mnoho různých národních prostředí.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="2f9e6-108">Například Australia Financial Data, Canada Personal Information Act, U.S. Financial Data a tak dále.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="2f9e6-109">Podívejte se [na informace o tom, co šablony zásad ochrany před únikem dat obsahují](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pro úplný seznam.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="2f9e6-110">Všechny tyto šablony lze povolit podobně jako příklad šablony PII.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="2f9e6-111">Nastavení uchovávání e-mailů pomocí archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="2f9e6-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="2f9e6-112">Funkce licencí **Exchange Online Archiving** pomáhají udržovat dodržování předpisů a regulační standardy zachováním e-mailového obsahu pro eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="2f9e6-113">Pomáhá také snížit riziko, pokud dojde k soudnímu sporu, a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo když potřebujete obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="2f9e6-114">Blokování z důvodu soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací k přizpůsobení toho, co chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="2f9e6-115">**Blokování ze soudních sporů:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat blokováním celé poštovní schránky uživatele.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="2f9e6-116">Umístění poštovní schránky pro blokování z důvodu soudních sporů v Centru pro správu:</span><span class="sxs-lookup"><span data-stu-id="2f9e6-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="2f9e6-117">V levém nav, přejděte na **uživatele** \> **aktivní uživatele**.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="2f9e6-118">Vyberte uživatele, jehož poštovní schránku chcete umístit jako blokování z důvodu soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="2f9e6-119">V uživatelském podokně rozbalte **nastavení pošty**a vedle **položky Další nastavení**zvolte Upravit **vlastnosti Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="2f9e6-120">Na stránce poštovní schránky pro uživatele zvolte \*\* funkce poštovní schránky \*\* v levém nav a pak zvolte odkaz **Povolit** v části **Blokování z držení soudního sporu**.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="2f9e6-121">V dialogovém okně **blokování soudních sporů** můžete určit dobu trvání blokování soudních sporů v poli **Doba trvání blokování soudních sporů.**</span><span class="sxs-lookup"><span data-stu-id="2f9e6-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="2f9e6-122">Pokud chcete pole ponechat prázdné, ponechejte nekonečné blokování.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="2f9e6-123">Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který budete muset vysvětlit více o blokování z důvodu soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="2f9e6-124">\>**Uložit**.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-124">\> **Save**.</span></span>
    
<span data-ttu-id="2f9e6-125">**Uchovávání informací:** Můžete povolit vlastní zásady uchovávání informací, například zachovat po určitou dobu nebo odstranit obsah trvale na konci období uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="2f9e6-126">Další informace naleznete v [tématu Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="2f9e6-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="2f9e6-127">Nastavení popisků citlivosti</span><span class="sxs-lookup"><span data-stu-id="2f9e6-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="2f9e6-128">Popisky citlivosti jsou dodávány s plánem Azure Information Protection (AIP) 1 a pomáhají vám klasifikovat a volitelně chránit vaše dokumenty a e-maily použitím štítků.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="2f9e6-129">Popisky mohou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, kde jsou uživatelům poskytnuta doporučení.</span><span class="sxs-lookup"><span data-stu-id="2f9e6-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="2f9e6-130">Chcete-li nastavit popisky citlivosti, [zobrazte video vytvoření a správu popisků citlivosti.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="2f9e6-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="2f9e6-131">Ruční instalace klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="2f9e6-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="2f9e6-132">Ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="2f9e6-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="2f9e6-133">Stáhněte si **soubor AzinfoProtection_UL.exe** ze [služby Stažení softwaru společnosti Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="2f9e6-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="2f9e6-134">Můžete ověřit, zda instalace fungovala zobrazením dokumentu aplikace Word a ověřením, zda je možnost **Citlivost** dostupná na kartě **Domů.**</span><span class="sxs-lookup"><span data-stu-id="2f9e6-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="2f9e6-135">![Rozevírací přehled karta Ochrana v dokumentu aplikace Word](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="2f9e6-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="2f9e6-136">Další informace naleznete [v tématu Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="2f9e6-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
