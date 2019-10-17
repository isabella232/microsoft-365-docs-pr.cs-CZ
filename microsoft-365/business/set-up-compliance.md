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

## <a name="set-up-sensitivity-labels"></a>Nastavit popisky citlivosti

Štítky s citlivostí jsou součástí plánu 1 Azure Information Protection (AIP) a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily pomocí popisků. Štítky mohou být automaticky použity správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, v níž jsou uživatelům poskytnuta doporučení.

Chcete-li nastavit popisky citlivosti, zobrazte [Vytvoření a správu popisků citlivosti](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videa.



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta ochrany informací Azure

Ruční instalace klienta AIP:

1. Stáhněte **AzinfoProtection_UL. exe** z [webu služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Instalaci můžete ověřit zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **Citlivost** .
<br/>![Rozevírací karta zámku v dokumentu aplikace Word.](media/word-sensitivity.png)

Další informace naleznete v části [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
