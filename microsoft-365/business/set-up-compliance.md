---
title: Zvýšení ochrany před hrozbou pro Microsoft 365 Business Premium
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
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a zajistili zabezpečení citlivých informací vašich zákazníků.
ms.openlocfilehash: e210787718025c5df29af8d4a2283291dcecc2a8
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912524"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="777be-103">Nastavení funkcí dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="777be-103">Set up compliance features</span></span>

<span data-ttu-id="777be-104">Microsoft 365 Business Premium obsahuje funkce, které chrání vaše data a zařízení a pomáhají vám udržet citlivé informace vašich zákazníků v bezpečí.</span><span class="sxs-lookup"><span data-stu-id="777be-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="777be-105">Nastavení funkcí DLP</span><span class="sxs-lookup"><span data-stu-id="777be-105">Set up DLP features</span></span>

<span data-ttu-id="777be-106">Příklad [nastavení zásad](../compliance/create-a-dlp-policy-from-a-template.md) pro ochranu před únikem osobních údajů najdete v tématu Vytvoření zásady ochrany před únikem informací ze šablony.</span><span class="sxs-lookup"><span data-stu-id="777be-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="777be-107">Funkce DLP obsahuje mnoho šablon zásad připravených k použití pro mnoho různých národní prostředí.</span><span class="sxs-lookup"><span data-stu-id="777be-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="777be-108">Například Australia Financial Data, Canada Personal Information Act, US Financial Data a tak dále.</span><span class="sxs-lookup"><span data-stu-id="777be-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="777be-109">Úplný [seznam najdete v tématu Co](../compliance/what-the-dlp-policy-templates-include.md) šablony zásad ochrany před únikem informací obsahují.</span><span class="sxs-lookup"><span data-stu-id="777be-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="777be-110">Všechny tyto šablony můžete povolit podobně jako v příkladu šablony PII.</span><span class="sxs-lookup"><span data-stu-id="777be-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="777be-111">Nastavení uchovávání e-mailů pomocí archivace Exchange Online</span><span class="sxs-lookup"><span data-stu-id="777be-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="777be-112">**Funkce licencí pro archivaci Exchange Online** pomáhají udržovat dodržování předpisů a regulační normy zachováním e-mailového obsahu pro eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="777be-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="777be-113">Pomáhá také snížit riziko v případě, že dojde k soudnímu sporu, a umožňuje obnovit data po porušení zabezpečení nebo v případě, že potřebujete obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="777be-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="777be-114">Blokování soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací můžete přizpůsobit to, co chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="777be-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="777be-115">**Blokování z důvodu soudního sporu:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte.</span><span class="sxs-lookup"><span data-stu-id="777be-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="777be-116">Pokud chcete poštovní schránku umístit do blokování soudních sporů, v Centru pro správu:</span><span class="sxs-lookup"><span data-stu-id="777be-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="777be-117">V levém navigačním panelu přejděte na **Uživatelé** \> **aktivních uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="777be-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="777be-118">Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="777be-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="777be-119">V podokně uživatelů rozbalte Nastavení **pošty** a vedle další **nastavení** zvolte **Upravit vlastnosti Exchange.**</span><span class="sxs-lookup"><span data-stu-id="777be-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="777be-120">Na stránce poštovní schránky pro uživatele zvolte \*\* Funkce poštovní schránky \*\* v levém navigačním panelu a pak zvolte **odkaz** Povolit v části **Blokování soudních sporů**.</span><span class="sxs-lookup"><span data-stu-id="777be-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="777be-121">V dialogovém **okně Blokování z** důvodu soudního sporu můžete zadat dobu trvání blokování z důvodu soudního sporu do pole Doba trvání blokování z důvodu **soudního** sporu.</span><span class="sxs-lookup"><span data-stu-id="777be-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="777be-122">Pokud chcete umístit nekonečné blokování, nechejte pole prázdné.</span><span class="sxs-lookup"><span data-stu-id="777be-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="777be-123">Můžete taky přidat poznámky a nasměrováte vlastníka poštovní schránky na web, na který možná budete muset vysvětlit další informace o blokování z důvodu soudního sporu.</span><span class="sxs-lookup"><span data-stu-id="777be-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="777be-124">\>**Uložit**.</span><span class="sxs-lookup"><span data-stu-id="777be-124">\> **Save**.</span></span>
    
<span data-ttu-id="777be-125">**Uchovávání informací:** Můžete například povolit přizpůsobené zásady uchovávání informací, které chcete zachovat po určitou dobu, nebo trvale odstranit obsah na konci období uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="777be-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="777be-126">Další informace najdete v tématu [Přehled zásad uchovávání informací](../compliance/retention.md).</span><span class="sxs-lookup"><span data-stu-id="777be-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="777be-127">Nastavení popisků citlivosti</span><span class="sxs-lookup"><span data-stu-id="777be-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="777be-128">Popisky citlivosti jsou vybaveny plánem 1 azure information protection (AIP) a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily použitím štítků.</span><span class="sxs-lookup"><span data-stu-id="777be-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="777be-129">Popisky můžou automaticky používat správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, ve které jsou uživatelům dána doporučení.</span><span class="sxs-lookup"><span data-stu-id="777be-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="777be-130">Pokud chcete nastavit popisky citlivosti, podívejte se na video o vytváření [a správě popisků](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) citlivosti.</span><span class="sxs-lookup"><span data-stu-id="777be-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="777be-131">Ruční instalace klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="777be-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="777be-132">Ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="777be-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="777be-133">Stáhněte **AzinfoProtection_UL.exe** [z webu Stažení softwaru microsoftu](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="777be-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="777be-134">Můžete ověřit, že instalace fungovala tak, že  si prohlédněte wordové dokumenty a ujistěte se, že je na **kartě Domů** dostupná možnost Citlivost.</span><span class="sxs-lookup"><span data-stu-id="777be-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="777be-135">![Rozevírací seznam Karta Ochrana ve wordovém dokumentu](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="777be-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="777be-136">Další informace najdete v tématu [Instalace klienta](/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="777be-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>