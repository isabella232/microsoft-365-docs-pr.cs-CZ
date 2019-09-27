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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Nastavení sady Office 365 Pokročilá ochrana proti ohrožení a ochrana citlivých dat
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288739"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="a579f-103">Nastavení funkcí kompatibility</span><span class="sxs-lookup"><span data-stu-id="a579f-103">Set up compliance features</span></span>

<span data-ttu-id="a579f-104">Společnost Microsoft 365 Business obsahuje funkce pro ochranu dat a zařízení a pomáhá zabezpečit vaše a citlivé informace zákazníků.</span><span class="sxs-lookup"><span data-stu-id="a579f-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="a579f-105">Nastavení funkcí DLP</span><span class="sxs-lookup"><span data-stu-id="a579f-105">Set up DLP features</span></span>

<span data-ttu-id="a579f-106">Viz [Vytvoření zásady DLP ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) pro příklad, jak nastavit zásady ochrany proti osobním identifikovatelným informacím (PII).</span><span class="sxs-lookup"><span data-stu-id="a579f-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="a579f-107">DLP přináší mnoho šablon zásad připravených k použití pro mnoho různých národních prostředí.</span><span class="sxs-lookup"><span data-stu-id="a579f-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="a579f-108">Například australské finanční údaje, zákon o osobním informování Kanady, finanční data USA atd. Podívejte [se, co šablony zásad DLP obsahují](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pro úplný seznam.</span><span class="sxs-lookup"><span data-stu-id="a579f-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="a579f-109">Všechny tyto šablony lze povolit podobným příkladem šablony PII.</span><span class="sxs-lookup"><span data-stu-id="a579f-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="a579f-110">Nastavení uchování e-mailu pomocí archivace online serveru Exchange</span><span class="sxs-lookup"><span data-stu-id="a579f-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="a579f-111">Funkce pro **archivaci online systému Exchange** pomáhá udržovat dodržování a regulační standardy zachováním obsahu e-mailu pro program eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="a579f-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="a579f-112">Pomáhá také snižovat riziko v případě žaloby a poskytuje způsob, jak obnovit data po porušení zabezpečení nebo kdy je nutné obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="a579f-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="a579f-113">Chcete-li zachovat veškerý obsah uživatele nebo pomocí zásad uchovávání informací upravit, co chcete zachovat, můžete použít blokování sporů.</span><span class="sxs-lookup"><span data-stu-id="a579f-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="a579f-114">**Soudní spor:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat umístěním celé poštovní schránky uživatele do blokování soudních sporů.</span><span class="sxs-lookup"><span data-stu-id="a579f-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="a579f-115">Chcete-li umístit poštovní schránku na soudní řízení, v centru pro správu:</span><span class="sxs-lookup"><span data-stu-id="a579f-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="a579f-116">V levém navigačním poli přejděte na **uživatele** \> **Active Users**.</span><span class="sxs-lookup"><span data-stu-id="a579f-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="a579f-117">Vyberte uživatele, jehož poštovní schránku chcete umístit do soudního sporu, a v uživatelském podokně rozbalte **Nastavení pošty** a vedle **dalších nastavení** zvolte možnost **Upravit vlastnosti serveru Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a579f-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="a579f-118">Na stránce poštovní schránky uživatele zvolte \* \* funkce poštovní schránky \* \* na levém navigačním panelu a pak zvolte možnost **Povolit** odkaz v rámci **soudního sporu**.</span><span class="sxs-lookup"><span data-stu-id="a579f-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="a579f-119">V dialogovém okně **soudní spor** můžete určit dobu trvání v poli **Doba trvání soudního** sporu, ponechat pole prázdné, chcete-li umístit nekonečné blokování.</span><span class="sxs-lookup"><span data-stu-id="a579f-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="a579f-120">Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který bude pravděpodobně nutné objasnit \> **uložení**tohoto sporu.</span><span class="sxs-lookup"><span data-stu-id="a579f-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="a579f-121">**Uchovávání informací:** Můžete povolit vlastní zásady uchovávání informací, například chcete-li zachovat určitou dobu nebo trvale odstranit obsah na konci retenční periody.</span><span class="sxs-lookup"><span data-stu-id="a579f-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="a579f-122">Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="a579f-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="a579f-123">Nastavení funkcí ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="a579f-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="a579f-124">Ochrana informací Azure (AIP) vám pomáhá klasifikovat a volitelně chránit své dokumenty a e-maily, použitím štítků.</span><span class="sxs-lookup"><span data-stu-id="a579f-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="a579f-125">Štítky mohou být automaticky použity správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, v níž jsou uživatelům poskytnuta doporučení.</span><span class="sxs-lookup"><span data-stu-id="a579f-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="a579f-126">V aplikaci Outlook na webu můžete použít následující předdefinované popisky a omezení pro e-maily:</span><span class="sxs-lookup"><span data-stu-id="a579f-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="a579f-127">**Nepředávat dál**: příjemci mohou zprávu přečíst, ale nemohou předat dál, vytisknout nebo kopírovat obsah</span><span class="sxs-lookup"><span data-stu-id="a579f-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="a579f-128">**Šifrovat**: celá zpráva je zašifrována.</span><span class="sxs-lookup"><span data-stu-id="a579f-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="a579f-129">Příjemci musí před přístupem k šifrovanému obsahu potvrdit svou identitu a nemůže odebrat šifrování.</span><span class="sxs-lookup"><span data-stu-id="a579f-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="a579f-130">**Důvěrné**: zaměstnancům v organizaci umožní plná oprávnění k obsahu e-mailu a k přílohám, ale nikoli k osobám mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="a579f-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="a579f-131">Vlastníci dat mohou v libovolném bodě sledovat a odvolávat obsah.</span><span class="sxs-lookup"><span data-stu-id="a579f-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="a579f-132">**Vysoce důvěrné**: Toto omezení lze použít pro vysoce důvěrná data, což zaměstnancům umožňuje zobrazovat, upravovat a odpovídat, ale ne předávat data dál, tisknout nebo kopírovat.</span><span class="sxs-lookup"><span data-stu-id="a579f-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="a579f-133">Vlastníci dat mohou v libovolném bodě sledovat a odvolávat obsah.</span><span class="sxs-lookup"><span data-stu-id="a579f-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="a579f-134">Ujistěte se, že je aktivována ochrana informací Azure</span><span class="sxs-lookup"><span data-stu-id="a579f-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="a579f-135">Chcete-li ověřit, zda je AIP aktivován:</span><span class="sxs-lookup"><span data-stu-id="a579f-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="a579f-136">Podepište se na [Azure portál](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="a579f-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="a579f-137">Vyberte **všechny služby** a do **vyhledávacího pole**zadejte *ochranu informací Azure* .</span><span class="sxs-lookup"><span data-stu-id="a579f-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="a579f-138">Po zobrazení výsledků klepněte na začátek vedle položky **ochrana informací Azure** , abyste jej mohli později snadno najít.</span><span class="sxs-lookup"><span data-stu-id="a579f-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="a579f-139">Vyberte možnost \> **Aktivace ochrany** **informací Azure** a zkontrolujte, zda je stav nastaven na aktivováno.</span><span class="sxs-lookup"><span data-stu-id="a579f-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="a579f-140">Zobrazit zásadu ochrany informací Azure a výchozí popisky</span><span class="sxs-lookup"><span data-stu-id="a579f-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="a579f-141">Chcete-li zobrazit a upravit existující štítky, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="a579f-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="a579f-142">Na řídicím panelu pro ochranu informací vyberte **klasifikace** \> **.**</span><span class="sxs-lookup"><span data-stu-id="a579f-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="a579f-143">![Standardní štítky pro ochranu informací Azure.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="a579f-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="a579f-144">Můžete zvolit libovolný popisek pro zobrazení možností, můžete změnit zobrazované jméno, barvy atd.</span><span class="sxs-lookup"><span data-stu-id="a579f-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="a579f-145">Pokud chcete vytvořit vlastní, viz [Úpravy a vytvoření nových štítků](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) .</span><span class="sxs-lookup"><span data-stu-id="a579f-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="a579f-146">Ruční instalace klienta ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="a579f-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="a579f-147">Ruční instalace klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="a579f-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="a579f-148">Stáhněte soubor **Azinfoprotection. exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="a579f-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="a579f-149">Instalaci můžete ověřit zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **chránit** .</span><span class="sxs-lookup"><span data-stu-id="a579f-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="a579f-150">![Rozevírací karta zámku v dokumentu aplikace Word.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="a579f-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="a579f-151">Další informace naleznete v části [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="a579f-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
