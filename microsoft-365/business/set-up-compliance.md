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
# <a name="set-up-compliance-features"></a>Nastavení funkcí kompatibility

Společnost Microsoft 365 Business obsahuje funkce pro ochranu dat a zařízení a pomáhá zabezpečit vaše a citlivé informace zákazníků.

## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Viz [Vytvoření zásady DLP ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) pro příklad, jak nastavit zásady ochrany proti osobním identifikovatelným informacím (PII). 
  
DLP přináší mnoho šablon zásad připravených k použití pro mnoho různých národních prostředí. Například australské finanční údaje, zákon o osobním informování Kanady, finanční data USA atd. Podívejte [se, co šablony zásad DLP obsahují](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) pro úplný seznam. Všechny tyto šablony lze povolit podobným příkladem šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchování e-mailu pomocí archivace online serveru Exchange

 Funkce pro **archivaci online systému Exchange** pomáhá udržovat dodržování a regulační standardy zachováním obsahu e-mailu pro program eDiscovery. Pomáhá také snižovat riziko v případě žaloby a poskytuje způsob, jak obnovit data po porušení zabezpečení nebo kdy je nutné obnovit odstraněné položky. Chcete-li zachovat veškerý obsah uživatele nebo pomocí zásad uchovávání informací upravit, co chcete zachovat, můžete použít blokování sporů.
  
**Soudní spor:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat umístěním celé poštovní schránky uživatele do blokování soudních sporů. 
    
Chcete-li umístit poštovní schránku na soudní řízení, v centru pro správu:
    
1. V levém navigačním poli přejděte na **uživatele** \> **Active Users**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit do soudního sporu, a v uživatelském podokně rozbalte **Nastavení pošty** a vedle **dalších nastavení** zvolte možnost **Upravit vlastnosti serveru Exchange**.
    
3. Na stránce poštovní schránky uživatele zvolte * * funkce poštovní schránky * * na levém navigačním panelu a pak zvolte možnost **Povolit** odkaz v rámci **soudního sporu**.
    
4. V dialogovém okně **soudní spor** můžete určit dobu trvání v poli **Doba trvání soudního** sporu, ponechat pole prázdné, chcete-li umístit nekonečné blokování. Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který bude pravděpodobně nutné objasnit \> **uložení**tohoto sporu.
    
**Uchovávání informací:** Můžete povolit vlastní zásady uchovávání informací, například chcete-li zachovat určitou dobu nebo trvale odstranit obsah na konci retenční periody. Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Nastavení funkcí ochrany informací Azure

Ochrana informací Azure (AIP) vám pomáhá klasifikovat a volitelně chránit své dokumenty a e-maily, použitím štítků. Štítky mohou být automaticky použity správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, v níž jsou uživatelům poskytnuta doporučení.

V aplikaci Outlook na webu můžete použít následující předdefinované popisky a omezení pro e-maily:
  
- **Nepředávat dál**: příjemci mohou zprávu přečíst, ale nemohou předat dál, vytisknout nebo kopírovat obsah
    
- **Šifrovat**: celá zpráva je zašifrována. Příjemci musí před přístupem k šifrovanému obsahu potvrdit svou identitu a nemůže odebrat šifrování.
    
- **Důvěrné**: zaměstnancům v organizaci umožní plná oprávnění k obsahu e-mailu a k přílohám, ale nikoli k osobám mimo vaši organizaci. Vlastníci dat mohou v libovolném bodě sledovat a odvolávat obsah.
    
- **Vysoce důvěrné**: Toto omezení lze použít pro vysoce důvěrná data, což zaměstnancům umožňuje zobrazovat, upravovat a odpovídat, ale ne předávat data dál, tisknout nebo kopírovat. Vlastníci dat mohou v libovolném bodě sledovat a odvolávat obsah.

### <a name="make-sure-azure-information-protection-is-activated"></a>Ujistěte se, že je aktivována ochrana informací Azure

Chcete-li ověřit, zda je AIP aktivován:

1. Podepište se na [Azure portál](https://portal.azure.com/).

2. Vyberte **všechny služby** a do **vyhledávacího pole**zadejte *ochranu informací Azure* .

3. Po zobrazení výsledků klepněte na začátek vedle položky **ochrana informací Azure** , abyste jej mohli později snadno najít.

4. Vyberte možnost \> **Aktivace ochrany** **informací Azure** a zkontrolujte, zda je stav nastaven na aktivováno. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Zobrazit zásadu ochrany informací Azure a výchozí popisky 

Chcete-li zobrazit a upravit existující štítky, postupujte takto:

1. Na řídicím panelu pro ochranu informací vyberte **klasifikace** \> **.** <br/>![Standardní štítky pro ochranu informací Azure.](media/AIPLabels.png)

2. Můžete zvolit libovolný popisek pro zobrazení možností, můžete změnit zobrazované jméno, barvy atd.
 
3. Pokud chcete vytvořit vlastní, viz [Úpravy a vytvoření nových štítků](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) . 

### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta ochrany informací Azure

Ruční instalace klienta AIP:

1. Stáhněte soubor **Azinfoprotection. exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Instalaci můžete ověřit zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **chránit** . <br/>![Rozevírací karta zámku v dokumentu aplikace Word.](media/Word_Protect.png)

Další informace naleznete v části [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
