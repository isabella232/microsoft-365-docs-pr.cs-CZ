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
description: Nastavení funkcí pro dodržování předpisů pro ochranu před ztrátou dat a zachování důvěrných informací a vašich zákazníků.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841167"
---
# <a name="set-up-compliance-features"></a>Nastavení funkcí pro dodržování předpisů

Společnost Microsoft 365 Business Premium přichází s funkcemi pro ochranu vašich dat a zařízení a pomáhá zabezpečit citlivé informace a vaše zákazníky.

## <a name="set-up-dlp-features"></a>Nastavení funkcí ochrany před únikem informací

Další informace o tom, jak nastavit zásadu pro ochranu před ztrátou osobních údajů, najdete v tématu [Vytvoření zásad DLP ze šablony](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) . 
  
Technologie DLP přináší mnoho šablon zásad připravených k použití pro mnoho různých národních prostředí. Například Austrálie finanční data, Kanada – osobní údaje, finanční údaje USA a další. Podívejte [se, jaké jsou šablony zásad DLP](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) pro úplný seznam. Všechny tyto šablony můžou být povolené v příkladu šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů s archivací Exchange Online

 Funkce **archivace licencí na Exchange Online** pomáhají udržovat dodržování předpisů v e-mailu pro eDiscovery na základě souladu s pravidly pro správu shody. Pomáhá také snížit vaše riziko, pokud se jedná o soudní řízení a způsob, jak obnovit data po porušení zabezpečení nebo když potřebujete obnovit odstraněné položky. Chcete-li zachovat veškerý obsah uživatele, můžete použít podržení sporu, nebo můžete pomocí zásad uchovávání informací přizpůsobit, co chcete zachovat.
  
**Držení sporu:** Všechny poštovní schránky, včetně odstraněných položek, můžete zachovat tak, že zadáte celou poštovní schránku uživatele na blokování soudního sporu. 
    
Umístění poštovní schránky v centru pro správu – blokování soudního sporu:
    
1. V levém navigačním panelu přejděte na **Uživatelé** \> **aktivní uživatelé**.
    
2. Vyberte uživatele, jehož poštovní schránku chcete umístit na přihlášeného. V podokně uživatel rozbalte položku **Nastavení pošty** a vedle **Možnosti další nastavení** zvolte **Upravit vlastnosti Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte * * funkce poštovní schránky * * na levém navigačním panelu a pak zvolte **Povolit** odkaz v části **pozdržení sporu**.
    
4. V dialogovém okně **podržet soudní spor** můžete určit dobu trvání držení pro soudní řízení v poli **Doba trvání přidržení** . Pokud chcete umístit nekonečné blokování, nechte pole prázdné. Můžete taky přidat poznámky a směrovat vlastníka poštovní schránky na web, možná budete muset vysvětlit Další informace o přístupnosti. \>**Uložit**.
    
**Uchovávání informací:** Můžete povolit zásady uchovávání informací, například zachovat po určitou dobu nebo trvale odstranit obsah na konci období uchovávání informací. Další informace najdete v tématu [Přehled zásad uchovávání informací](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Nastavit popisky citlivosti

Popisky citlivosti jsou součástí služby Azure Information Protection (AIP) plán 1 a pomáhají klasifikovat a volitelně chránit dokumenty a e-maily použitím popisků. Štítky můžou automaticky použít správci, kteří definují pravidla a podmínky, ručně uživatelé nebo používají kombinaci, kde jsou uživatelům nabídnuta doporučení.

Pokud chcete nastavit popisky citlivosti, zobrazte si [možnosti vytvořit a spravovat](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video s popisky.



### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta služby Azure Information Protection

Postup ruční instalace klienta AIP:

1. Stáhněte si **AzinfoProtection_UL.exe** ze [služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Instalaci můžete ověřit tak, že zobrazíte wordový dokument a zajistíte, že je na kartě **Domů** dostupná možnost **Citlivost** .
<br/>![Rozevírací seznam karty zámek ve wordovém dokumentu](../media/word-sensitivity.png)

Další informace najdete v článku [instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
