---
title: Zvýšit ochranu před hrozbami pro Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Nastavení Office 365 rozšířené ohrožení ochrany a chránit citlivá data.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086286"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="2b234-103">Nastavení funkcí kompatibility</span><span class="sxs-lookup"><span data-stu-id="2b234-103">Set up compliance features</span></span>

<span data-ttu-id="2b234-104">Váš podnik 365 Microsoft obsahuje funkce pro ochranu dat a zařízení a zabezpečení vás a vaše zákazníky citlivé informace.</span><span class="sxs-lookup"><span data-stu-id="2b234-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="2b234-105">Nastavení funkcí DLP</span><span class="sxs-lookup"><span data-stu-id="2b234-105">Set up DLP features</span></span>

<span data-ttu-id="2b234-106">Příklad, jak nastavit zásady na ochranu proti osobně identifikovatelných informací (PII), viz [Vytvoření DLP zásady ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) .</span><span class="sxs-lookup"><span data-stu-id="2b234-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="2b234-107">DLP je dodávána s mnoha šablon připravených k použití zásad pro mnoho různá národní prostředí.</span><span class="sxs-lookup"><span data-stu-id="2b234-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="2b234-108">Například finanční Data Austrálie, Kanada osobní informace Act, USA finanční Data, atd. Úplný seznam naleznete v tématu [šablony zásad DLP co patří](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) .</span><span class="sxs-lookup"><span data-stu-id="2b234-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="2b234-109">Všechny tyto šablony lze povolit podobný příklad šablony PII.</span><span class="sxs-lookup"><span data-stu-id="2b234-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="2b234-110">Nastavení uchovávání e-mailů s Exchange Online archivaci</span><span class="sxs-lookup"><span data-stu-id="2b234-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="2b234-111">Funkce **Exchange Online archivaci** licenční pomáhá zachovat dodržování předpisů a norem o zachování e-mailů obsahu pro služba eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="2b234-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="2b234-112">Také pomáhá snížit riziko v případě probíhající soudní řízení a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo potřebujete obnovit odstraněné položky.</span><span class="sxs-lookup"><span data-stu-id="2b234-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="2b234-113">Můžete použít blokování sporu zachovat veškerý obsah uživatele nebo pomocí zásad uchovávání informací upravit, co chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="2b234-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="2b234-114">**Soudní spory podržte:** Můžete zachovat veškerý obsah poštovní schránky včetně odstraněných položek vložením celé poštovní schránky uživatele na soudní spory podržte.</span><span class="sxs-lookup"><span data-stu-id="2b234-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="2b234-115">Chcete-li umístit poštovní schránky blokované sporu ve středisku pro správce:</span><span class="sxs-lookup"><span data-stu-id="2b234-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="2b234-116">V navigace vlevo, go **uživatelům** \> **aktivních uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="2b234-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="2b234-117">Vyberte uživatele, jejichž poštovní schránky, které chcete umístit na soudní spory podržte a rozbalte v podokně uživatelské **Nastavení e-mailu** a v oblasti **Další nastavení** zvolte **Vlastnosti upravit Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2b234-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="2b234-118">Na stránce poštovní schránky pro uživatele zvolte \*\* funkce poštovní schránky \*\* na navigace vlevo a pak zvolte **Povolit** odkaz pod **soudní spory podržte**.</span><span class="sxs-lookup"><span data-stu-id="2b234-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="2b234-119">Dialogové okno můžete určit sporu **podržte soudní spory** podržte trvání v poli **Doba trvání podržte soudní spory** , ponechte pole prázdné, pokud chcete umístit nekonečné blokování.</span><span class="sxs-lookup"><span data-stu-id="2b234-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="2b234-120">Můžete přidat poznámky a přímý vlastník pole mail na webu, bude pravděpodobně nutné vysvětlit více o sporu podržte \> **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="2b234-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="2b234-121">**Uchovávání informací:** Můžete povolit zásady uchovávání informací vlastní, například má být zachována po určitou dobu nebo trvale odstranit obsah na konci období uchování.</span><span class="sxs-lookup"><span data-stu-id="2b234-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="2b234-122">Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="2b234-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="2b234-123">Nastavení funkcí Azure ochrana údajů</span><span class="sxs-lookup"><span data-stu-id="2b234-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="2b234-124">Klasifikaci a volitelně chránit dokumenty a e-maily, použitím štítků Azure pomáhá ochrany informací (AIP).</span><span class="sxs-lookup"><span data-stu-id="2b234-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="2b234-125">Popisky lze použít automaticky správce, kteří definují pravidla a podmínky, ručně uživatelem nebo pomocí kombinace, kde uživatelé jsou uvedena doporučení.</span><span class="sxs-lookup"><span data-stu-id="2b234-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="2b234-126">V aplikaci Outlook na webu lze použít následující vestavěné popisy a omezení na vaše e-maily:</span><span class="sxs-lookup"><span data-stu-id="2b234-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="2b234-127">**Dál**: příjemci mohou zprávu číst, ale jejich nelze předat dál, vytisknout nebo kopírování obsahu</span><span class="sxs-lookup"><span data-stu-id="2b234-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="2b234-128">**Šifrování**: celá zpráva je šifrovaná.</span><span class="sxs-lookup"><span data-stu-id="2b234-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="2b234-129">Příjemci musí potvrdit svou identitu před přístupem k obsahu zašifrované a nelze odebrat šifrování.</span><span class="sxs-lookup"><span data-stu-id="2b234-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="2b234-130">**Důvěrné**: dává zaměstnanců ve vaší organizaci úplná oprávnění k obsahu e-mailů a příloh, ale nikoli osoby mimo organizaci.</span><span class="sxs-lookup"><span data-stu-id="2b234-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="2b234-131">Vlastníci dat můžete sledovat a obsah kdykoli odvolat.</span><span class="sxs-lookup"><span data-stu-id="2b234-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="2b234-132">**Vysoce důvěrné**: Toto omezení lze použít vysoce důvěrné údaje, umožňující zaměstnancům, aby zobrazit, upravit a odpovědět, ale není dál, vytisknout nebo zkopírovat data.</span><span class="sxs-lookup"><span data-stu-id="2b234-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="2b234-133">Vlastníci dat můžete sledovat a obsah kdykoli odvolat.</span><span class="sxs-lookup"><span data-stu-id="2b234-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="2b234-134">Zkontrolujte, zda že je aktivován Azure ochrana údajů</span><span class="sxs-lookup"><span data-stu-id="2b234-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="2b234-135">Chcete-li ověřit, zda je aktivován AIP:</span><span class="sxs-lookup"><span data-stu-id="2b234-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="2b234-136">Přihlášení k [portálu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2b234-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="2b234-137">Vyberte **všechny služby** a typ *Ochrany informace Azure* do **Vyhledávacího pole**.</span><span class="sxs-lookup"><span data-stu-id="2b234-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="2b234-138">Po zobrazení výsledků, klepněte na tlačítko start Další **Ochrana informací Azure** Chcete-li oblíbenou položku a možné později snáze najít.</span><span class="sxs-lookup"><span data-stu-id="2b234-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="2b234-139">**Ochrana informací Azure** vyberte \> **Aktivace ochrany** a zkontrolujte zda je nastaven stav na aktivovaný.</span><span class="sxs-lookup"><span data-stu-id="2b234-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="2b234-140">Zobrazit popisky zásad a výchozí ochrana informací Azure</span><span class="sxs-lookup"><span data-stu-id="2b234-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="2b234-141">Chcete-li zobrazit a upravit existující štítky:</span><span class="sxs-lookup"><span data-stu-id="2b234-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="2b234-142">Na panelu Digital dashboard ochrana informací Azure vyberte **klasifikace** \> **štítky**.</span><span class="sxs-lookup"><span data-stu-id="2b234-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="2b234-143">![Standardní popisky pro ochranu informací Azure.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="2b234-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="2b234-144">Můžete zvolit libovolný popisek chcete-li zobrazit možnosti, můžete změnit zobrazovaný název barvy, např.</span><span class="sxs-lookup"><span data-stu-id="2b234-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="2b234-145">Viz [změnit a vytvořit nové štítky s](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Pokud chcete vytvořit vlastní.</span><span class="sxs-lookup"><span data-stu-id="2b234-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="2b234-146">Ruční instalace klienta Azure ochrana údajů</span><span class="sxs-lookup"><span data-stu-id="2b234-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="2b234-147">Chcete-li ručně nainstalovat klienta AIP:</span><span class="sxs-lookup"><span data-stu-id="2b234-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="2b234-148">**AzInfoProtection.exe** lze stáhněte z [webu služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="2b234-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="2b234-149">Můžete ověřit, že instalace odpracovaných zobrazení dokumentu aplikace Word a přesvědčíte se, že je k dispozici na kartě **Domů** na možnost **chránit** .</span><span class="sxs-lookup"><span data-stu-id="2b234-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="2b234-150">![Kartu Zámek rozevíracího seznamu v dokumentu Word.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="2b234-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="2b234-151">Další informace viz [Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="2b234-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
