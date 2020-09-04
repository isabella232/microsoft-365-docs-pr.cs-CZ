---
title: Funkce zabezpečení a dodržování předpisů v Microsoft 365 Business Premium
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Přečtěte si informace o funkcích zabezpečení, které jsou součástí Microsoft 365 Business Premium, a chrání vaše data na počítačích, telefonech a tabletech.
ms.openlocfilehash: 5e16d4bf297d363b6f9b44ce854c857e7e5464ed
ms.sourcegitcommit: 9ce9001aa41172152458da27c1c52825355f426d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/03/2020
ms.locfileid: "47357312"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Funkce zabezpečení a dodržování předpisů v Microsoft 365 Business Premium

Microsoft 365 Business Premium nabízí zjednodušené funkce zabezpečení, které pomáhají chránit data na počítačích, telefonech a tabletech.
    
## <a name="microsoft-365-admin-center-security-features"></a>Funkce zabezpečení centra pro správu Microsoft 365

V centru pro správu můžete spravovat řadu funkcí zabezpečení Microsoft 365 Business Premium, která vám nabídne zjednodušený způsob, jak tyto funkce zapnout nebo vypnout. V centru pro správu můžete postupovat takto:
  
- Nastavení [správy aplikací pro zařízení s Androidem nebo iOS](app-protection-settings-for-android-and-ios.md) 
    
    Tato nastavení zahrnují odstranění souborů z neaktivního zařízení po nastaveném období, šifrování pracovních souborů, vyžadování a nastavení PIN uživatelů, atd.
    
- Nastavení [ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md) 
    
    Tato nastavení se dají použít u firemních dat ve vlastněném podniku i osobně vlastněných zařízeních.
    
- Nastavení [ochrany zařízení pro zařízení s Windows 10](protection-settings-for-windows-10-pcs.md) 
    
    Šifrování [nástrojem BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) můžete povolit tak, aby chránilo data v případě ztráty nebo odcizení zařízení a aby bylo možné povolit [systém Windows](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) pro ochranu před ransomwaru. 
    
- [Odebrání dat společnosti ze zařízení](remove-company-data.md)
    
    Když se zařízení ztratí, ukraden nebo zaměstnanec opustí vaši společnost, můžete data společnosti vzdáleně vymazat.
    
- [Obnovte tovární nastavení zařízení s Windows 10](reset-devices-to-factory-settings.md) . 
    
    Můžete resetovat všechna zařízení s Windows 10 s aplikovanými nastaveními ochrany zařízení.
    
## <a name="additional-security-features"></a>Další funkce zabezpečení 

Rozšířené funkce v Microsoft 365 Business Premium jsou k dispozici, které vám pomůžou chránit vaše podnikání před internetovými-hrozbami a chránit citlivé informace.
  
- **[Rozšířená ochrana před internetovými útoky v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Rozšířená ochrana před internetovými útoky (ATP) pomáhá chránit vaše podnikání před sofistikovanými útoky typu phishing a ransomwaru, které jsou určené k nazrazení informací o zaměstnancích Funkce zahrnují:
    
  - Sofistikovaná analýza příloh a analýza souborů AI pro zjišťování a zahození nebezpečných zpráv.
    
  - Automatické kontroly odkazů v e-mailu k vyhodnocení, jestli jsou součástí schématu útoků phishing. Tím se vyhnete přístupu k nebezpečným webům.

- **[Úplné možnosti Intune na portálu Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Přístup k centru pro správu v Intune na Azure Portal umožňuje nastavit další funkce zabezpečení, jako je Správa zařízení MacOS, iPhone a zařízení s Androidem, a rozšířené možnosti správy zařízení pro Windows, které nejsou dostupné v centru pro správu Microsoft 365.
- **Stejný [podmíněný přístup](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) jako plán Azure AD Premium P1**


    Podmíněný přístup může pomoci chránit vaši organizaci před přihlášením, pokusem o přístup z neočekávané sítě nebo národního prostředí, pokusit o přístup z typů rizikových zařízení atd. Zásady podmíněného přístupu jsou vynuceny po dokončení prvního ověřování a používají signály z první události ověřování k určení, jestli se má požadovaný přístup schválit, odepřít nebo zda je požadován další důkaz (například druhá forma identifikace).

    K dispozici jsou funkce podmíněného přístupu:

    - Přístup na základě uživatelského jména, skupiny a role
    - Přístup na [základě aplikace](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Přístup na základě umístění](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Povolit přístup jenom z IP adres nebo konkrétních zemí 
    - Vyžadovat MFA pro Access
    - Blokování přístupu k aplikacím, které používají [starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Vyžadovat, aby aplikace TP používaly [ochranu aplikací Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Vlastní ověřování, například MFA s poskytovateli třetích stran, například DUO
   
    Další funkce:
    - [Samoobslužné resetování hesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) pro hybridní Azure AD
    
## <a name="compliance-features"></a>Funkce pro dodržování předpisů

Předplatné Microsoft 365 Business Premium zahrnuje funkce, které vám pomůžou udržovat dodržování předpisů a zákonných standardů.

- **[Přehled zásad](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** ochrany před únikem informací (DLP) 
    
    DLP můžete nastavit tak, aby automaticky zjišťoval citlivé informace, jako jsou čísla kreditních karet, čísla sociálního pojištění atd., aby nedocházelo k jejich nechtěnému sdílení mimo vaši společnost.
    
- **[Exchange Online - archiv](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licence k archivování Exchange Online umožňuje, aby byly zprávy snadno archivované pomocí nepřetržité zálohování dat. Ukládá všechny e-maily uživatelů, včetně odstraněných položek, pro případ, že jsou později potřeba ke zjišťování nebo obnovení. Kromě toho můžete pomocí různých zásad uchovávání informací uchovat e-mailové údaje o podržení, eDiscovery nebo splnit požadavky na dodržování předpisů.
    
- **[Štítky utajení](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium zahrnuje všechny funkce [plánu Azure Information Protection 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Pomocí tohoto plánu můžete vytvářet **popisky citlivosti** , které umožňují řídit přístup k citlivým informacím v e-mailech a dokumentech, pomocí ovládacích prvků jako "Nepředávat dál" a "nekopírovat". Citlivé informace můžete také klasifikovat jako "důvěrné" a určit, jak se mají utajované informace sdílet mimo podnik a uvnitř firmy. Šifrování v rozlehlých sítích se snadno používá u e-mailů a dokumentů pro zachování soukromí. Můžete taky nainstalovat doplněk klienta Azure Information Protection pro aplikace Office. Další informace najdete v článku [jednotný klient pro ochranu informací v Azure](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Pro popisky citlivosti nainstalujte **AzInfoProtection_UL.exe**.

Tyto funkce můžete spravovat v &amp; Centru zabezpečení a centru pro správu Intune. V průběhu času se zjednodušené ovládací prvky přidají do centra pro správu Microsoft 365.
  
    
## <a name="faq"></a>Časté otázky

 ### <a name="are-these-security-features-available-in-all-markets"></a>Jsou tyto funkce zabezpečení k dispozici na všech trzích?
  
Ano, tyto funkce jsou k dispozici na všech trzích, kde se prodává Microsoft 365 Business Premium.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak najdu &amp; centrum dodržování předpisů?
  
1. [Přihlaste se k Microsoft 365 Business Premium](https://portal.microsoft.com/) pomocí přihlašovacích údajů správce. 
    
2. V levém navigačním panelu najděte **centra pro správu** a rozbalte ji. 
    
    ![V levém navigačním panelu centra pro správu Microsoftu 365 zvolte centra pro správu.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Zvolte ** &amp; dodržování předpisů zabezpečení** a přejděte do &amp; centra dodržování předpisů zabezpečení.
