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
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a pomohli zabezpečit citlivé informace vašich zákazníků.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785826"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="0e1be-103">Nastavení funkcí dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="0e1be-103">Set up compliance features</span></span>

<span data-ttu-id="0e1be-104">Microsoft 365 Business Premium je vybaven funkcemi, které chrání vaše data a zařízení a pomáhají vám zabezpečit citlivé informace vašich i zákazníků.</span><span class="sxs-lookup"><span data-stu-id="0e1be-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="0e1be-105">Nastavení funkcí DLP</span><span class="sxs-lookup"><span data-stu-id="0e1be-105">Set up DLP features</span></span>

<span data-ttu-id="0e1be-106">Příklad nastavení zásady ochrany před osobními údaji (PII) najdete v tématu [Vytvoření zásady ochrany před ochranou](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) před ochranou před ochranou proti přístupu k informacím pomocí šablony.</span><span class="sxs-lookup"><span data-stu-id="0e1be-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="0e1be-107">DLP je dodáván s mnoha připravených šablon zásad pro mnoho různých národních prostředí.</span><span class="sxs-lookup"><span data-stu-id="0e1be-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="0e1be-108">Například Australia Financial Data, Canada Personal Information Act, US Financial Data atd.</span><span class="sxs-lookup"><span data-stu-id="0e1be-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="0e1be-109">Úplný seznam [najdete v tématu Co obsahují šablony zásad ochrany před](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) únikem let.</span><span class="sxs-lookup"><span data-stu-id="0e1be-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="0e1be-110">Všechny tyto šablony lze povolit podobně jako příklad šablony PII.</span><span class="sxs-lookup"><span data-stu-id="0e1be-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="0e1be-111">Nastavení uchovávání e-mailů pomocí archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="0e1be-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="0e1be-112">Funkce licence **k archivaci Exchange Online** pomáhají udržovat dodržování předpisů a regulační standardy zachováním obsahu e-mailu pro eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="0e1be-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="0e1be-113">Pomáhá také snížit riziko, pokud dojde k soudnímu sporu, a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo v případě, že potřebujete obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="0e1be-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="0e1be-114">Blokování z důvodu soudního sporu můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací můžete přizpůsobit, co chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="0e1be-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="0e1be-115">**Soudní řízení blokování:** Obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte.</span><span class="sxs-lookup"><span data-stu-id="0e1be-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="0e1be-116">Pokud chcete poštovní schránku udát v Centru pro správu, jak se držet v soudních sporech:</span><span class="sxs-lookup"><span data-stu-id="0e1be-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="0e1be-117">V levém navigačním programu **přejděte** na \> **Uživatelé Aktivní uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="0e1be-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="0e1be-118">Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování z důvodu soudního sporu.</span><span class="sxs-lookup"><span data-stu-id="0e1be-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="0e1be-119">V podokně uživatele rozbalte **položku Nastavení pošty**a vedle položky **Další nastavení**zvolte **Upravit vlastnosti serveru Exchange**.</span><span class="sxs-lookup"><span data-stu-id="0e1be-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="0e1be-120">Na stránce poštovní schránky pro uživatele zvolte \*\* funkce poštovní schránky \*\* v levém navigačním panelu a pak zvolte odkaz **Povolit** v části **Blokování soudních sporů**.</span><span class="sxs-lookup"><span data-stu-id="0e1be-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="0e1be-121">V dialogovém okně **blokování soudních sporů** můžete v poli Trvání blokování soudních sporů určit dobu **trvání blokování v soudních sporech.**</span><span class="sxs-lookup"><span data-stu-id="0e1be-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="0e1be-122">Pokud chcete umístit nekonečné blokování, ponechte pole prázdné.</span><span class="sxs-lookup"><span data-stu-id="0e1be-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="0e1be-123">Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který budete muset vysvětlit více o blokování soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="0e1be-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="0e1be-124">\>**Uložit**.</span><span class="sxs-lookup"><span data-stu-id="0e1be-124">\> **Save**.</span></span>
    
<span data-ttu-id="0e1be-125">**Zadržení:** Můžete povolit přizpůsobené zásady uchovávání informací, například zachovat po určitou dobu nebo trvale odstranit obsah na konci doby uchovávání.</span><span class="sxs-lookup"><span data-stu-id="0e1be-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="0e1be-126">Další informace najdete v [tématu Přehled zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="0e1be-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="0e1be-127">Nastavení popisků citlivosti</span><span class="sxs-lookup"><span data-stu-id="0e1be-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="0e1be-128">Popisky citlivosti jsou dodávány s plánem Azure Information Protection (AIP) 1 a pomáhají vám klasifikovat a volitelně chránit vaše dokumenty a e-maily použitím štítků.</span><span class="sxs-lookup"><span data-stu-id="0e1be-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="0e1be-129">Popisky mohou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, kde jsou uživatelům poskytnuta doporučení.</span><span class="sxs-lookup"><span data-stu-id="0e1be-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="0e1be-130">Chcete-li nastavit popisky citlivosti, [zobrazte zobrazení videa vytvořit a spravovat popisky citlivosti.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="0e1be-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="0e1be-131">Ruční instalace klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0e1be-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="0e1be-132">Ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="0e1be-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="0e1be-133">Stáhněte **siAzinfoProtection_UL.exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018)společnosti Microsoft .</span><span class="sxs-lookup"><span data-stu-id="0e1be-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="0e1be-134">Můžete ověřit, že instalace fungovala zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **Citlivost.**</span><span class="sxs-lookup"><span data-stu-id="0e1be-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="0e1be-135">![Rozevírací panel Ochrany v dokumentu aplikace Word](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="0e1be-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="0e1be-136">Další informace naleznete [v tématu Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="0e1be-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
