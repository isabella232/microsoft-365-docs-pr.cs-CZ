---
title: Microsoft 365 Business Premium zabezpečení a dodržování předpisů
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Přečtěte si o funkcích zabezpečení, které jsou součástí Microsoft 365 Business Premium, které pomáhají chránit vaše data na počítačích, telefonech a tabletech.
ms.openlocfilehash: 974204e100d3228f78406aca4acce67a889b08c3
ms.sourcegitcommit: 05f40904f8278f53643efa76a907968b5c662d9a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "52113460"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium zabezpečení a dodržování předpisů

Microsoft 365 Business Premium nabízí zjednodušené funkce zabezpečení, které pomáhají chránit vaše data na počítačích, telefonech a tabletech.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 zabezpečení Centra pro správu

V Centru pro správu můžete spravovat Microsoft 365 Business Premium funkcí zabezpečení, které vám umožní tyto funkce zjednodušeně zapnout nebo vypnout. V Centru pro správu můžete udělat toto:
  
- [Nastavení správy aplikací pro zařízení s Androidem nebo iOS](app-protection-settings-for-android-and-ios.md) 
    
    Tato nastavení zahrnují odstranění souborů z neaktivního zařízení po nastaveném období, šifrování pracovních souborů, které vyžadují, aby uživatelé nastavili PIN kód a tak dále.
    
- [Nastavení ochrany aplikací pro Windows 10 zařízení](protection-settings-for-windows-10-devices.md) . 
    
    Tato nastavení můžete použít na firemní data na zařízeních vlastněných společností nebo v osobním vlastnictví.
    
- [Nastavení ochrany zařízení pro Windows 10 zařízení](protection-settings-for-windows-10-pcs.md) . 
    
    Můžete povolit šifrování [nástroj BitLocker,](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) které pomáhá chránit data v případě ztráty nebo odcizení zařízení, a povolit Windows [Exploit Guard](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) poskytovat pokročilou ochranu před ransomwarem. 
    
- [Odebrání dat společnosti ze zařízení](remove-company-data.md)
    
    Data společnosti můžete vzdáleně vymazat, pokud dojde ke ztrátě, odcizení zařízení nebo pokud zaměstnanec opustí vaši společnost.
    
- [Resetujte Windows 10 zařízení do továrního nastavení](reset-devices-to-factory-settings.md) . 
    
    Můžete resetovat všechna Windows 10 zařízení, u které je použito nastavení ochrany zařízení.
    
## <a name="additional-security-features"></a>Další funkce zabezpečení 

Pokročilé funkce v Microsoft 365 Business Premium jsou dostupné, aby vám pomohly chránit vaši firmu před kybernetickými hrozbami a chránit citlivé informace.
  
- **[Microsoft Defender pro Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    Microsoft Defender pro Office 365 pomáhá chránit vaši firmu před propracovanými útoky phishing a ransomwaru navrženými tak, aby ohrozil informace o zaměstnancích nebo zákaznících. Mezi funkce patří:
    
  - Sofistikované vyhledávání příloh a analýza využívající AI pro zjišťování a zahození nebezpečných zpráv.
    
  - Automatické kontroly odkazů v e-mailu za účelem posouzení, jestli jsou součástí phishingového schématu. Díky tomu budete v bezpečí před přístupem k nebezpečným webům.

- **[Úplné možnosti Intune na portálu Azure Portal](/mem/intune/fundamentals/what-is-intune)**
    
    Přístup k Centru pro správu Intune na portálu Azure Portal umožňuje nastavit další funkce zabezpečení, jako je správa zařízení s MacOS, iPhone Microsoft 365 zařízení s Androidem a pokročilá správa zařízení pro Windows, které nejsou dostupné prostřednictvím Centra pro správu Microsoft 365.
- **Stejný [podmíněný přístup jako](/azure/active-directory/conditional-access/overview) plán Azure AD Premium P1**


    Podmíněný přístup pomáhá chránit vaši organizaci před riziky přihlášení, pokusy o přístup z neočekávané sítě nebo národního prostředí, pokusy o přístup z ohrožených typů zařízení a tak dále. Zásady podmíněného přístupu se vynucují po dokončení prvního ověřování a pomocí signálů z první události ověřování určí, jestli by měl být pokus o přístup schválen, zamítnut nebo jestli je nutný další důkaz (například druhá forma identifikace).

    Zahrnuté funkce podmíněného přístupu:

    - Access založený na uživatelském jménu, skupině a roli
    - Access [založený na aplikaci](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Přístup na základě umístění](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Povolit přístup jenom z důvěryhodných rozsahů IP adres nebo konkrétních zemí 
    - Vyžadovat MFA pro přístup
    - Blokování přístupu k aplikacím, které používají [starší ověřování](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Vyžadování aplikací k používání [ochrany aplikací Intune](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Vlastní ověřování, například MFA s zprostředkovateli třetích stran, například DUO.
   
    Další funkce:
    - [Samoobslužné resetování hesla pro](/azure/active-directory/authentication/concept-sspr-customization) hybridní Azure AD
    
## <a name="compliance-features"></a>Funkce dodržování předpisů

Vaše Microsoft 365 Business Premium zahrnuje funkce, které vám pomůžou udržovat dodržování předpisů a regulační standardy.

- **[Další informace o prevenci ztráty dat](../compliance/dlp-learn-about-dlp.md))** (DLP). 
    
    Pomocí funkce DLP můžete nastavit automatické zjišťování citlivých informací, jako jsou čísla osobních karet, čísla sociálního zabezpečení atd., aby se zabránilo jejich neúmyslnému sdílení mimo vaši společnost.
    
- **[Exchange Online - archiv](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online – archiv umožňuje snadno archivovat zprávy pomocí nepřetržitého zálohování dat. Ukládá všechny e-maily uživatele, včetně odstraněných položek, pro případ, že je budete později potřebovat pro zjišťování nebo obnovení. Kromě toho můžete k zachování e-mailových dat pro blokování soudních sporů, eDiscovery nebo splnění požadavků na dodržování předpisů použít různé zásady uchovávání informací.
    
- **[Štítky utajení](../compliance/sensitivity-labels.md)**

   Microsoft 365 Business Premium obsahuje všechny funkce [plánu Azure Information Protection 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Pomocí tohoto plánu můžete  vytvořit popisky citlivosti, které vám umožní řídit přístup k citlivým informacím v e-mailu a dokumentech s ovládacími prvky, jako je "Neposílání" a "Nekopírovat". Můžete také klasifikovat citlivé informace jako důvěrné a určit, jak se budou utajované informace sdílet mimo firmu i uvnitř firmy. Enterprise šifrování se snadno používá u e-mailů a dokumentů, aby vaše informace byly soukromé. Můžete si taky nainstalovat doplněk klienta Azure Information Protection pro Office aplikace. Další informace najdete v článku sjednocený klient [štítků Azure Information Protection](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). U štítků citlivosti nainstalujte **AzInfoProtection_UL.exe**.

Tyto funkce můžete spravovat v Centru dodržování předpisů zabezpečení a &amp; v Centru pro správu Intune. V průběhu času se zjednodušené ovládací prvky přidávají do centra Microsoft 365 správy.
  
    
## <a name="faq"></a>Časté otázky

 ### <a name="are-these-security-features-available-in-all-markets"></a>Jsou tyto funkce zabezpečení dostupné na všech trzích?
  
Ano, tyto funkce jsou dostupné na všech trzích, kde se Microsoft 365 Business Premium prodává.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak najdu Centrum dodržování &amp; předpisů zabezpečení?
  
1. [Přihlaste se k Microsoft 365 Business Premium](https://portal.microsoft.com/) pomocí přihlašovacích údajů správce. 
    
2. V levém navigačním panelu najděte **Centra pro správu** a rozbalte ji. 
    
    ![V levém navigačním panelu v Centru Microsoft 365 správy zvolte Centra pro správu.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Zvolte **Dodržování &amp; předpisů zabezpečení** a přejděte do Centra dodržování předpisů &amp; zabezpečení.
