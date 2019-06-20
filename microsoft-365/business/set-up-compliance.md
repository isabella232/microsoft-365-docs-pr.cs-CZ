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
# <a name="set-up-compliance-features"></a>Nastavení funkcí kompatibility

Váš podnik 365 Microsoft obsahuje funkce pro ochranu dat a zařízení a zabezpečení vás a vaše zákazníky citlivé informace.

## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Příklad, jak nastavit zásady na ochranu proti osobně identifikovatelných informací (PII), viz [Vytvoření DLP zásady ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) . 
  
DLP je dodávána s mnoha šablon připravených k použití zásad pro mnoho různá národní prostředí. Například finanční Data Austrálie, Kanada osobní informace Act, USA finanční Data, atd. Úplný seznam naleznete v tématu [šablony zásad DLP co patří](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Všechny tyto šablony lze povolit podobný příklad šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů s Exchange Online archivaci

 Funkce **Exchange Online archivaci** licenční pomáhá zachovat dodržování předpisů a norem o zachování e-mailů obsahu pro služba eDiscovery. Také pomáhá snížit riziko v případě probíhající soudní řízení a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo potřebujete obnovit odstraněné položky. Můžete použít blokování sporu zachovat veškerý obsah uživatele nebo pomocí zásad uchovávání informací upravit, co chcete zachovat.
  
**Soudní spory podržte:** Můžete zachovat veškerý obsah poštovní schránky včetně odstraněných položek vložením celé poštovní schránky uživatele na soudní spory podržte. 
    
Chcete-li umístit poštovní schránky blokované sporu ve středisku pro správce:
    
1. V navigace vlevo, go **uživatelům** \> **aktivních uživatelů**.
    
2. Vyberte uživatele, jejichž poštovní schránky, které chcete umístit na soudní spory podržte a rozbalte v podokně uživatelské **Nastavení e-mailu** a v oblasti **Další nastavení** zvolte **Vlastnosti upravit Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** funkce poštovní schránky ** na navigace vlevo a pak zvolte **Povolit** odkaz pod **soudní spory podržte**.
    
4. Dialogové okno můžete určit sporu **podržte soudní spory** podržte trvání v poli **Doba trvání podržte soudní spory** , ponechte pole prázdné, pokud chcete umístit nekonečné blokování. Můžete přidat poznámky a přímý vlastník pole mail na webu, bude pravděpodobně nutné vysvětlit více o sporu podržte \> **Uložit**.
    
**Uchovávání informací:** Můžete povolit zásady uchovávání informací vlastní, například má být zachována po určitou dobu nebo trvale odstranit obsah na konci období uchování. Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Nastavení funkcí Azure ochrana údajů

Klasifikaci a volitelně chránit dokumenty a e-maily, použitím štítků Azure pomáhá ochrany informací (AIP). Popisky lze použít automaticky správce, kteří definují pravidla a podmínky, ručně uživatelem nebo pomocí kombinace, kde uživatelé jsou uvedena doporučení.

V aplikaci Outlook na webu lze použít následující vestavěné popisy a omezení na vaše e-maily:
  
- **Dál**: příjemci mohou zprávu číst, ale jejich nelze předat dál, vytisknout nebo kopírování obsahu
    
- **Šifrování**: celá zpráva je šifrovaná. Příjemci musí potvrdit svou identitu před přístupem k obsahu zašifrované a nelze odebrat šifrování.
    
- **Důvěrné**: dává zaměstnanců ve vaší organizaci úplná oprávnění k obsahu e-mailů a příloh, ale nikoli osoby mimo organizaci. Vlastníci dat můžete sledovat a obsah kdykoli odvolat.
    
- **Vysoce důvěrné**: Toto omezení lze použít vysoce důvěrné údaje, umožňující zaměstnancům, aby zobrazit, upravit a odpovědět, ale není dál, vytisknout nebo zkopírovat data. Vlastníci dat můžete sledovat a obsah kdykoli odvolat.

### <a name="make-sure-azure-information-protection-is-activated"></a>Zkontrolujte, zda že je aktivován Azure ochrana údajů

Chcete-li ověřit, zda je aktivován AIP:

1. Přihlášení k [portálu Azure](https://portal.azure.com/).

2. Vyberte **všechny služby** a typ *Ochrany informace Azure* do **Vyhledávacího pole**.

3. Po zobrazení výsledků, klepněte na tlačítko start Další **Ochrana informací Azure** Chcete-li oblíbenou položku a možné později snáze najít.

4. **Ochrana informací Azure** vyberte \> **Aktivace ochrany** a zkontrolujte zda je nastaven stav na aktivovaný. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Zobrazit popisky zásad a výchozí ochrana informací Azure 

Chcete-li zobrazit a upravit existující štítky:

1. Na panelu Digital dashboard ochrana informací Azure vyberte **klasifikace** \> **štítky**. <br/>![Standardní popisky pro ochranu informací Azure.](media/AIPLabels.png)

2. Můžete zvolit libovolný popisek chcete-li zobrazit možnosti, můžete změnit zobrazovaný název barvy, např.
 
3. Viz [změnit a vytvořit nové štítky s](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Pokud chcete vytvořit vlastní. 

### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure ochrana údajů

Chcete-li ručně nainstalovat klienta AIP:

1. **AzInfoProtection.exe** lze stáhněte z [webu služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, že instalace odpracovaných zobrazení dokumentu aplikace Word a přesvědčíte se, že je k dispozici na kartě **Domů** na možnost **chránit** . <br/>![Kartu Zámek rozevíracího seznamu v dokumentu Word.](media/Word_Protect.png)

Další informace viz [Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
