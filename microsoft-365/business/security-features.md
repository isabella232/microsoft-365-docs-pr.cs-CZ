---
title: Funkce zabezpečení a dodržování předpisů microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Přečtěte si o funkcích zabezpečení, které jsou součástí aplikace Microsoft 365 Business.
ms.openlocfilehash: e5f67d70c5a8f22e95b60a229d68ae12574d0036
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064790"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Funkce zabezpečení a dodržování předpisů microsoft 365 Business

Microsoft 365 Business nabízí zjednodušené funkce zabezpečení, které pomáhají chránit vaše data na počítačích, telefonech a tabletech.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkce zabezpečení Centra pro správu Microsoftu 365 Business

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

V Centru pro správu můžete spravovat mnoho funkcí zabezpečení Microsoft 365 Business, což vám poskytuje zjednodušený způsob zapnutí nebo vypnutí těchto funkcí. V Centru pro správu můžete provést následující kroky:
  
- [Nastavte nastavení správy aplikací pro zařízení se systémem Android nebo iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Tato nastavení zahrnují odstranění souborů z neaktivního zařízení po nastaveném období, šifrování pracovních souborů, vyžadování, aby uživatelé nastavili kód PIN a tak dále.
    
- [Nastavte nastavení ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Tato nastavení lze použít pro firemní data na zařízeních vlastněných společností nebo v osobním vlastnictví.
    
- [Nastavte nastavení ochrany zařízení pro zařízení s Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Šifrování [nástroje BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) můžete povolit, abyste ochránili data v případě ztráty nebo odcizení zařízení, a povolit [ochranu zneužití systému Windows,](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) která poskytuje pokročilou ochranu proti ransomwaru. 
    
- [Odebrání dat společnosti ze zařízení](remove-company-data.md)
    
    Pokud dojde ke ztrátě, odcizení nebo odchodu zaměstnance ze společnosti, můžete vzdáleně vymazat firemní data.
    
- [Resetujte zařízení s Windows 10 do továrního nastavení](reset-devices-to-factory-settings.md) . 
    
    Můžete obnovit všechna zařízení s Windows 10, na která je použito nastavení ochrany zařízení.
    
## <a name="additional-security-features"></a>Další funkce zabezpečení 

K dispozici jsou pokročilé funkce v Microsoft365 Business, které vám pomohou chránit vaše podnikání před kybernetickými hrozbami a chránit citlivé informace.
  
- **[Pokročilá ochrana před hrozbami Office 365](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Pokročilá ochrana před hrozbami (ATP) pomáhá chránit vaše podnikání před sofistikovanými phishingovými útoky a útoky ransomwaru, které jsou navrženy tak, aby ohrozily informace o zaměstnancích nebo zákaznících. Mezi funkce patří:
    
  - Sofistikované skenování příloh a analýza napájená umělou aušnou pro detekci a zahození nebezpečných zpráv.
    
  - Automatické kontroly odkazů v e-mailu, abyste zjistili, zda jsou součástí phishingového systému. Tím budete mít v bezpečí přístup k nebezpečným webům.

- **[Plné možnosti Intune na portálu Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Přístup do Centra pro správu Intune na portálu Azure umožňuje nastavit další funkce zabezpečení, jako je správa zařízení MacOS, iPhone a zařízení se systémem Android, spolu s pokročilou správou zařízení pro Windows, které nejsou dostupné prostřednictvím Microsoftu 365 Centrum pro správu firmy.
- **Stejný [podmíněný přístup](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jako plán Azure AD P1**


    Podmíněný přístup může pomoci chránit vaši organizaci před rizikem přihlášení, pokusy o přístup z neočekávané sítě nebo národního prostředí, pokusy o přístup z rizikových typů zařízení a tak dále. Zásady podmíněného přístupu jsou vynuceny po dokončení prvního ověření a používají signály z první události ověřování k určení, zda by pokus o přístup měl být schválen, odepřen nebo zda by měl být další důkaz (například druhá forma identifikace) je vyžadována.

    Zahrnuty funkce podmíněného přístupu jsou:

    - Přístup na základě uživatelského jména, skupiny a role
    - Přístup [založený na aplikaci](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Přístup na základě umístění](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Povolit přístup pouze z důvěryhodných rozsahů IP adres nebo konkrétních zemí 
    - Vyžadovat vícefaktorové čekání pro přístup
    - Blokovat přístup k aplikacím, které používají [starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Vyžadovat aplikace tp používat [Ochranu aplikací Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Vlastní ověřování, jako je vícefaktorové ověřování s poskytovateli třetích stran, například DUO.
   
    Další funkce:
    - [Samoobslužné resetování hesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) pro hybridní Azure AD
    
## <a name="compliance-features"></a>Funkce dodržování předpisů

Vaše předplatné Microsoft 365 Business obsahuje funkce, které vám pomohou udržovat dodržování předpisů a regulační standardy.

- **[Přehled zásad prevence ztráty dat](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Službu DLP můžete nastavit tak, aby automaticky odhalovala citlivé informace, jako jsou čísla kreditních karet, čísla sociálního pojištění a tak dále, aby se zabránilo jejich neúmyslnému sdílení mimo vaši společnost.
    
- **[Exchange Online - archiv](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licence Exchange Online Archivace umožňuje snadnou archivaci zpráv pomocí průběžného zálohování dat. Ukládá všechny e-maily uživatele, včetně odstraněných položek, v případě, že jsou později potřeba pro zjišťování nebo obnovení. Kromě toho můžete použít různé zásady uchovávání k uchování e-mailových dat pro blokování soudních sporů, eDiscovery nebo ke splnění požadavků na dodržování předpisů.
    
- **[Štítky utajení](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business obsahuje všechny funkce [Plánu ochrany informací Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Pomocí tohoto plánu můžete vytvořit **popisky citlivosti,** které vám umožní řídit přístup k citlivým informacím v e-mailech a dokumentech, s ovládacími prvky jako "Nepřesměrujte dál" a "Nekopírovat". Citlivé informace můžete také klasifikovat jako "Důvěrné" a určit, jak lze utajované informace sdílet vně i uvnitř podniku. Šifrování podnikové kvality se snadno aplikuje na e-maily a dokumenty, aby byly vaše informace soukromé. Taky si můžete nainstalovat doplněk klienta Azure Information Protection pro aplikace Office. Další informace naleznete v tématu [Azure Information Protection unified labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Popisky citlivosti nastavíte **soubor AzInfoProtection_UL.exe**.

Tyto funkce můžete spravovat &amp; v Centru dodržování předpisů zabezpečení a v Centru pro správu Intune. V průběhu času budou zjednodušené ovládací prvky přidány do Centra pro správu Microsoft 365 Business.
  
    
## <a name="faq"></a>Časté otázky

 ### <a name="are-these-security-features-available-in-all-markets"></a>Jsou tyto funkce zabezpečení dostupné na všech trzích?
  
Ano, tyto funkce jsou k dispozici na všech trzích, kde se prodává Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak najdu Centrum &amp; dodržování předpisů zabezpečení?
  
1. [Přihlaste se k Microsoftu 365 Business](https://portal.microsoft.com/) pomocí přihlašovacích údajů správce. 
    
2. V levé nav vyhledejte **centra pro správu** a rozbalte je. 
    
    ![V levé nav v Centru pro správu Microsoftu 365 zvolte Centra pro správu.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Zvolte dodržování předpisů &amp; **zabezpečení &amp; ** a přejděte do Centra dodržování předpisů zabezpečení.
