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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Nastavte funkce dodržování předpisů, abyste zabránili ztrátě dat a pomohli zabezpečit citlivé informace vašich zákazníků.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785826"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí dodržování předpisů

Microsoft 365 Business Premium je vybaven funkcemi, které chrání vaše data a zařízení a pomáhají vám zabezpečit citlivé informace vašich i zákazníků.

## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Příklad nastavení zásady ochrany před osobními údaji (PII) najdete v tématu [Vytvoření zásady ochrany před ochranou](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) před ochranou před ochranou proti přístupu k informacím pomocí šablony. 
  
DLP je dodáván s mnoha připravených šablon zásad pro mnoho různých národních prostředí. Například Australia Financial Data, Canada Personal Information Act, US Financial Data atd. Úplný seznam [najdete v tématu Co obsahují šablony zásad ochrany před](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) únikem let. Všechny tyto šablony lze povolit podobně jako příklad šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů pomocí archivace Exchange Online

 Funkce licence **k archivaci Exchange Online** pomáhají udržovat dodržování předpisů a regulační standardy zachováním obsahu e-mailu pro eDiscovery. Pomáhá také snížit riziko, pokud dojde k soudnímu sporu, a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo v případě, že potřebujete obnovit odstraněné položky. Blokování z důvodu soudního sporu můžete použít k zachování veškerého obsahu uživatele nebo pomocí zásad uchovávání informací můžete přizpůsobit, co chcete zachovat.
  
**Soudní řízení blokování:** Obsah poštovní schránky včetně odstraněných položek můžete zachovat tak, že celou poštovní schránku uživatele zadržíte. 
    
Pokud chcete poštovní schránku udát v Centru pro správu, jak se držet v soudních sporech:
    
1. V levém navigačním programu **přejděte** na \> **Uživatelé Aktivní uživatelé**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit do blokování z důvodu soudního sporu. V podokně uživatele rozbalte **položku Nastavení pošty**a vedle položky **Další nastavení**zvolte **Upravit vlastnosti serveru Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** funkce poštovní schránky ** v levém navigačním panelu a pak zvolte odkaz **Povolit** v části **Blokování soudních sporů**.
    
4. V dialogovém okně **blokování soudních sporů** můžete v poli Trvání blokování soudních sporů určit dobu **trvání blokování v soudních sporech.** Pokud chcete umístit nekonečné blokování, ponechte pole prázdné. Můžete také přidat poznámky a nasměrovat vlastníka poštovní schránky na web, který budete muset vysvětlit více o blokování soudních sporů. \>**Uložit**.
    
**Zadržení:** Můžete povolit přizpůsobené zásady uchovávání informací, například zachovat po určitou dobu nebo trvale odstranit obsah na konci doby uchovávání. Další informace najdete v [tématu Přehled zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Nastavení popisků citlivosti

Popisky citlivosti jsou dodávány s plánem Azure Information Protection (AIP) 1 a pomáhají vám klasifikovat a volitelně chránit vaše dokumenty a e-maily použitím štítků. Popisky mohou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživateli nebo pomocí kombinace, kde jsou uživatelům poskytnuta doporučení.

Chcete-li nastavit popisky citlivosti, [zobrazte zobrazení videa vytvořit a spravovat popisky citlivosti.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure Information Protection

Ruční instalace klienta AIP:

1. Stáhněte **siAzinfoProtection_UL.exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018)společnosti Microsoft .
 
2. Můžete ověřit, že instalace fungovala zobrazením dokumentu aplikace Word a ověřením, zda je na kartě **Domů** k dispozici možnost **Citlivost.**
<br/>![Rozevírací panel Ochrany v dokumentu aplikace Word](../media/word-sensitivity.png)

Další informace naleznete [v tématu Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
