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
ms.openlocfilehash: c0accc37d3dcda9ba75813f01a98a3233c5a8369
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579948"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí dodržování předpisů

Microsoft 365 Business Premium obsahuje funkce, které chrání vaše data a zařízení a pomáhají vám udržet citlivé informace vašich zákazníků v bezpečí.

## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Příklad [nastavení zásad](../compliance/create-a-dlp-policy-from-a-template.md) pro ochranu před únikem osobních údajů najdete v tématu Vytvoření zásady ochrany před únikem informací ze šablony. 
  
Funkce DLP obsahuje mnoho šablon zásad připravených k použití pro mnoho různých národní prostředí. Například Australia Financial Data, Canada Personal Information Act, US Financial Data a tak dále. Úplný [seznam najdete v tématu Co](../compliance/what-the-dlp-policy-templates-include.md) šablony zásad ochrany před únikem informací obsahují. Všechny tyto šablony můžete povolit podobně jako v příkladu šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů pomocí archivace Exchange Online

 **Funkce licencí pro archivaci Exchange Online** pomáhají udržovat dodržování předpisů a regulační normy zachováním e-mailového obsahu pro eDiscovery. Pomáhá také snížit riziko v případě, že dojde k soudnímu sporu, a umožňuje obnovit data po porušení zabezpečení nebo v případě, že potřebujete obnovit odstraněné položky. Blokování soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací můžete přizpůsobit to, co chcete zachovat.
  
**Blokování z důvodu soudního sporu:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte. 
    
Pokud chcete poštovní schránku umístit do blokování soudních sporů, v Centru pro správu:
    
1. V levém navigačním panelu přejděte na **Uživatelé** \> **aktivních uživatelů**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování soudních sporů. V podokně uživatelů rozbalte Nastavení **pošty** a vedle další **nastavení** zvolte **Upravit vlastnosti Exchange.**
    
3. Na stránce poštovní schránky pro uživatele zvolte ** Funkce poštovní schránky ** v levém navigačním panelu a pak zvolte **odkaz** Povolit v části **Blokování soudních sporů**.
    
4. V dialogovém **okně Blokování z** důvodu soudního sporu můžete zadat dobu trvání blokování z důvodu soudního sporu do pole Doba trvání blokování z důvodu **soudního** sporu. Pokud chcete umístit nekonečné blokování, nechejte pole prázdné. Můžete taky přidat poznámky a nasměrováte vlastníka poštovní schránky na web, na který možná budete muset vysvětlit další informace o blokování z důvodu soudního sporu. \>**Uložit**.
    
**Uchovávání informací:** Můžete například povolit přizpůsobené zásady uchovávání informací, které chcete zachovat po určitou dobu, nebo trvale odstranit obsah na konci období uchovávání informací. Další informace najdete v tématu [Přehled zásad uchovávání informací](../compliance/retention.md).

## <a name="set-up-sensitivity-labels"></a>Nastavení popisků citlivosti

Popisky citlivosti jsou vybaveny plánem 1 azure information protection (AIP) a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily použitím štítků. Popisky můžou automaticky používat správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, ve které jsou uživatelům dána doporučení.

Pokud chcete nastavit popisky citlivosti, podívejte se na video o vytváření [a správě popisků](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) citlivosti.



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure Information Protection

Ruční instalace klienta AIP:

1. Stáhněte **AzinfoProtection_UL.exe** [z webu Stažení softwaru microsoftu](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, že instalace fungovala tak, že  si prohlédněte wordové dokumenty a ujistěte se, že je na **kartě Domů** dostupná možnost Citlivost.
<br/>![Rozevírací seznam Karta Ochrana ve wordovém dokumentu](../media/word-sensitivity.png)

Další informace najdete v tématu [Instalace klienta](/azure/information-protection/infoprotect-tutorial-step3).