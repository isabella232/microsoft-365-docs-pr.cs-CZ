---
title: Zvýšení ochrany před hrozbou pro Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245078"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí dodržování předpisů

Váš Microsoft 365 Business Premium obsahuje funkce, které chrání vaše data a zařízení a pomáhají vám udržet citlivé informace vašich zákazníků v bezpečí.

## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Příklad [nastavení zásad](../compliance/create-a-dlp-policy-from-a-template.md) pro ochranu před únikem osobních údajů najdete v tématu Vytvoření zásady ochrany před únikem informací ze šablony. 
  
Funkce DLP obsahuje mnoho šablon zásad připravených k použití pro mnoho různých národní prostředí. Například Australia Financial Data, Canada Personal Information Act, US Financial Data a tak dále. Úplný [seznam najdete v tématu Co](../compliance/what-the-dlp-policy-templates-include.md) šablony zásad ochrany před únikem informací obsahují. Všechny tyto šablony můžete povolit podobně jako v příkladu šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů pomocí Exchange Online – archiv

 **Exchange Online – archiv** licenční funkce pomáhají udržovat dodržování předpisů a regulační standardy zachováním e-mailového obsahu pro eDiscovery. Pomáhá také snížit riziko v případě, že dojde k soudnímu sporu, a umožňuje obnovit data po porušení zabezpečení nebo v případě, že potřebujete obnovit odstraněné položky. Blokování soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací můžete přizpůsobit to, co chcete zachovat.
  
**Blokování z důvodu soudního sporu:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte. 
    
Pokud chcete poštovní schránku umístit do blokování soudních sporů, v Centru pro správu:
    
1. V levém navigačním panelu přejděte na **Uživatelé** \> **aktivních uživatelů**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování soudních sporů. V podokně uživatelů rozbalte Nastavení **pošty** a vedle další nastavení **zvolte** Upravit Exchange **vlastností**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** Funkce poštovní schránky ** v levém navigačním panelu a pak zvolte **odkaz** Povolit v části **Blokování soudních sporů**.
    
4. V dialogovém **okně Blokování z** důvodu soudního sporu můžete zadat dobu trvání blokování z důvodu soudního sporu do pole Doba trvání blokování z důvodu **soudního** sporu. Pokud chcete umístit nekonečné blokování, nechejte pole prázdné. Můžete taky přidat poznámky a nasměrováte vlastníka poštovní schránky na web, na který možná budete muset vysvětlit další informace o blokování z důvodu soudního sporu. \>**Uložit**.
    
**Uchovávání informací:** Můžete například povolit přizpůsobené zásady uchovávání informací, které chcete zachovat po určitou dobu, nebo trvale odstranit obsah na konci období uchovávání informací. Další informace najdete v tématu [Přehled zásad uchovávání informací](../compliance/retention.md).

## <a name="set-up-sensitivity-labels"></a>Nastavení popisků citlivosti

Popisky citlivosti jsou vybaveny plánem 1 azure information protection (AIP) a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily použitím štítků. Popisky můžou automaticky používat správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, ve které jsou uživatelům dána doporučení.

Pokud chcete nastavit popisky citlivosti, podívejte se na video o vytváření [a správě popisků](../business-video/create-sensitivity-labels.md) citlivosti.



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure Information Protection

Ruční instalace klienta AIP:

1. Stáhněte **AzinfoProtection_UL.exe** [z webu Stažení softwaru microsoftu](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, že instalace fungovala tak, že  si prohlédněte wordové dokumenty a ujistěte se, že je na **kartě Domů** dostupná možnost Citlivost.
<br/>![Rozevírací seznam Karta Ochrana ve wordovém dokumentu](../media/word-sensitivity.png)

Další informace najdete v tématu [Instalace klienta](/azure/information-protection/infoprotect-tutorial-step3).