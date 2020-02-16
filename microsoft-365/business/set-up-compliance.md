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
search.appverid:
- BCS160
- MET150
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a popisek citlivých dat.
ms.openlocfilehash: d569ff8d84faf82881035f0ed54e5d175605776f
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064693"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí dodržování předpisů

Microsoft 365 Business je vybaven funkcemi, které chrání vaše data a zařízení a pomáhají vám zabezpečit vaše a citlivé informace vašich zákazníků.

## <a name="set-up-dlp-features"></a>Nastavení funkcí dlp

Viz [Vytvoření zásady dlp ze šablony,](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) kde najdete příklad nastavení zásady ochrany před osobně identifikovatelnými informacemi. 
  
DLP je dodáván s mnoha šablonami zásad připravených k použití pro mnoho různých národních prostředí. Například Austrálie Finanční údaje, Kanada osobní údaje zákona, americké finanční údaje, a tak dále. Úplný seznam najdete v [tématu Co obsahují šablony zásad dlp.](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) Všechny tyto šablony mohou být povoleny podobně jako příklad šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů pomocí archivace Exchange Online

 Funkce licencí **Exchange Online Archivační** licence pomáhají udržovat dodržování předpisů a regulační standardy tím, že zachovávají e-mailový obsah pro eDiscovery. Pomáhá také snížit riziko, pokud dojde k soudnímu sporu, a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo když potřebujete obnovit odstraněné položky. Blokování soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo k přizpůsobení toho, co chcete zachovat, pomocí zásad uchovávání.
  
**Soudní spory drží:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte. 
    
Umístění poštovní schránky na blokování soudních sporů v Centru pro správu:
    
1. V levé nav přejděte na **Uživatelé** \> **Aktivní uživatelé**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování soudních sporů. V podokně uživatelů rozbalte **nastavení pošty**a vedle části **Další nastavení**zvolte **Upravit vlastnosti serveru Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** funkce poštovní schránky ** na levé nav a pak zvolte **odkaz Povolit** v části **Blokování soudních sporů**.
    
4. V dialogovém okně **blokování soudních sporů** můžete určit dobu trvání blokování soudních sporů v poli **Doba trvání blokování soudních sporů.** Pole ponechejte prázdné, pokud chcete umístit nekonečné držení. Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který budete muset vysvětlit více o blokování soudních sporů. \>**Uložit**.
    
**Uchovávání:** Můžete povolit vlastní zásady uchovávání, například zachovat po určitou dobu nebo odstranit obsah trvale na konci období uchovávání. Další informace naleznete v [tématu Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Nastavení popisků citlivosti

Popisky citlivosti jsou dodávány s plánem Ochrany informací Azure (AIP) 1 a pomáhají klasifikovat a volitelně chránit vaše dokumenty a e-maily použitím štítků. Popisky mohou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, kde jsou uživatelům poskytnuta doporučení.

Chcete-li nastavit popisky citlivosti, zobrazte a spravujte video [popisků citlivosti.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure Information Protection

Ruční instalace klienta AIP:

1. Stáhněte si **AzinfoProtection_UL.exe** z [Centra pro stahování společnosti Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, zda instalace fungovala zobrazením dokumentu aplikace Word a zajištěním, že možnost **Citlivost** je dostupná na kartě **Domů.**
<br/>![Rozevírací zpráva karta Ochrana v dokumentu aplikace Word](../media/word-sensitivity.png)

Další informace naleznete v [tématu Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
