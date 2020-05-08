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
search.appverid:
- BCS160
- MET150
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a zajistili bezpečnost citlivých informací vašich zákazníků.
ms.openlocfilehash: a3405207cd7d2d6565807ef0f3a51acbcb80409a
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165731"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí dodržování předpisů

Microsoft 365 Business Premium je vybaven funkcemi, které chrání vaše data a zařízení a pomáhají vám zabezpečit citlivé informace vašich i zákazníků.

## <a name="set-up-dlp-features"></a>Nastavení funkcí programu DLP

Příklad, jak nastavit zásadu ochrany před únikem informací ze šablony, najdete v tématu [Vytvoření zásady ochrany před únikem](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) informací(PII). 
  
DLP je dodáván s mnoha připravenými šablonami zásad pro mnoho různých národních prostředí. Například Australia Financial Data, Canada Personal Information Act, U.S. Financial Data a tak dále. Podívejte se [na informace o tom, co šablony zásad ochrany před únikem dat obsahují](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) pro úplný seznam. Všechny tyto šablony lze povolit podobně jako příklad šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů pomocí archivace Exchange Online

 Funkce licencí **Exchange Online Archiving** pomáhají udržovat dodržování předpisů a regulační standardy zachováním e-mailového obsahu pro eDiscovery. Pomáhá také snížit riziko, pokud dojde k soudnímu sporu, a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo když potřebujete obnovit odstraněné položky. Blokování z důvodu soudních sporů můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací k přizpůsobení toho, co chcete zachovat.
  
**Blokování ze soudních sporů:** Veškerý obsah poštovní schránky včetně odstraněných položek můžete zachovat blokováním celé poštovní schránky uživatele. 
    
Umístění poštovní schránky pro blokování z důvodu soudních sporů v Centru pro správu:
    
1. V levém nav, přejděte na **uživatele** \> **aktivní uživatele**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit jako blokování z důvodu soudních sporů. V uživatelském podokně rozbalte **nastavení pošty**a vedle **položky Další nastavení**zvolte Upravit **vlastnosti Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** funkce poštovní schránky ** v levém nav a pak zvolte odkaz **Povolit** v části **Blokování z držení soudního sporu**.
    
4. V dialogovém okně **blokování soudních sporů** můžete určit dobu trvání blokování soudních sporů v poli **Doba trvání blokování soudních sporů.** Pokud chcete pole ponechat prázdné, ponechejte nekonečné blokování. Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který budete muset vysvětlit více o blokování z důvodu soudních sporů. \>**Uložit**.
    
**Uchovávání informací:** Můžete povolit vlastní zásady uchovávání informací, například zachovat po určitou dobu nebo odstranit obsah trvale na konci období uchovávání informací. Další informace naleznete v [tématu Přehled zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Nastavení popisků citlivosti

Popisky citlivosti jsou dodávány s plánem Azure Information Protection (AIP) 1 a pomáhají vám klasifikovat a volitelně chránit vaše dokumenty a e-maily použitím štítků. Popisky mohou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, kde jsou uživatelům poskytnuta doporučení.

Chcete-li nastavit popisky citlivosti, [zobrazte video vytvoření a správu popisků citlivosti.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure Information Protection

Ruční instalace klienta AIP:

1. Stáhněte si **soubor AzinfoProtection_UL.exe** ze [služby Stažení softwaru společnosti Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, zda instalace fungovala zobrazením dokumentu aplikace Word a ověřením, zda je možnost **Citlivost** dostupná na kartě **Domů.**
<br/>![Rozevírací přehled karta Ochrana v dokumentu aplikace Word](../media/word-sensitivity.png)

Další informace naleznete [v tématu Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
