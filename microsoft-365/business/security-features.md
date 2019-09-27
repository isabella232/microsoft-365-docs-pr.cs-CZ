---
title: Microsoft 365 obchodní zabezpečení a funkce kompatibility
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Seznamte se s funkcemi zabezpečení, které jsou součástí aplikace Microsoft 365 Business.
ms.openlocfilehash: 8e45d5fdb6a78f3966c46542189aa30ddd80998e
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288449"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 obchodní zabezpečení a funkce kompatibility

Společnost Microsoft 365 Business nabízí zjednodušené funkce zabezpečení, které pomáhají chránit data na osobních počítačích, telefonech a tabletách.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Bezpečnostní funkce střediska Microsoft 365 Business Admin Center

[![Popisek vám dá vědět, že se centrum pro správu mění a další podrobnosti naleznete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

V centru pro správu můžete spravovat mnoho funkcí aplikace Microsoft 365 Business Security, což vám umožňuje zjednodušit zapnutí nebo vypnutí těchto funkcí. V centru pro správu můžete provádět následující akce:
  
  
- [Nastavení správy aplikací pro zařízení Android nebo iOS](app-protection-settings-for-android-and-ios.md) . 
    
    Toto nastavení zahrnuje odstranění souborů z neaktivního zařízení po uplynutí nastavené doby, šifrování pracovních souborů, vyžadování, aby uživatelé nastavili kód PIN atd.
    
- Nastavení [ochrany aplikací pro zařízení systému Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Toto nastavení lze použít pro firemní data u zařízení vlastněných nebo osobně vlastněných společností.
    
- Nastavení [ochrany zařízení pro zařízení systému Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Pomocí šifrování [nástroje BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) můžete zajistit ochranu dat v případě ztráty nebo krádeže zařízení a povolení ochrany pomocí [systému Windows](https://go.microsoft.com/fwlink/p/?linkid=871404) , která poskytuje rozšířenou ochranu před Ransomware. 
    
- [Odebrání dat společnosti ze zařízení](remove-company-data.md)
    
    Pokud je zařízení ztraceno, ukradeno nebo pokud zaměstnanec opustí společnost, můžete data společnosti vzdáleně vymazat.
    
- [Resetujte zařízení systému Windows 10 Podle nastavení výrobce](reset-devices-to-factory-settings.md) . 
    
    Můžete obnovit všechna zařízení systému Windows 10, u kterých je použito nastavení ochrany zařízení.
    
## <a name="additional-security-features"></a>Další funkce zabezpečení 

V aplikaci Microsoft 365 Business jsou k dispozici pokročilé funkce, které vám pomohou ochránit váš podnik před internetovými hrozbami a zabezpečit citlivé informace.
  
- **[Office 365 Pokročilá ochrana proti ohrožení](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Funkce pokročilé ochrany proti ohrožení (ATP) pomáhá chránit vaše podnikání před sofistikovaným podvodným útokem a Ransomware, které mají ohrozit informace o zaměstnancích nebo o zákaznících. Mezi funkce patří:
    
  - Důmyslná kontrola příloh a analýza na technologii AI ke zjišťování a likvidace nebezpečných zpráv.
    
  - Automatické kontroly odkazů v e-mailech za účelem vyhodnocení, zda jsou součástí podvodného schématu. Tím zabráníte v bezpečném přístupu k nebezpečným webům.

- **[Plné schopnosti Intune v azurově portálu](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Přístup k centrovému středisku Intune v Azure portálu umožňuje nastavit další zabezpečovací funkce, jako je Správa zařízení MacOS, iPhone a Android, spolu s rozšířenou správou zařízení pro systém Windows, které nejsou dostupné prostřednictvím společnosti Microsoft 365 centrum pro správu podniku.
- **Stejný [podmíněný přístup](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) jako plán Azure AD P1**

    Podmíněný přístup může pomoci ochránit vaši organizaci před svým přístupem, pokusy o přístup z neočekávané sítě nebo národního prostředí, pokusy o přístup vytvářejí rizikové typy zařízení atd. Zásady podmíněného přístupu jsou vynuceny po dokončení prvního ověřování a pomocí signálů z první události ověřování lze určit, zda má být pokus o přístup schválen, odepřen nebo f více důkazů (například druhá forma identifikace) Požadované.

    Mezi zahrnuté funkce podmíněného přístupu patří:

    - Přístup na základě uživatelského jména, skupiny a role
    - Přístup na [základě aplikace](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Přístup na základě umístění](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  Povolit přístup pouze z důvěryhodných rozsahů IP nebo z určitých zemí 
    - Požadovat pro přístup MFA
    - Blokovat přístup k aplikacím, které používají [starší ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Vyžadovat aplikaci TP používat [ochranu aplikací Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Vlastní ověřování, například MFA s poskytovateli třetí strany, například DUO.
   
    Další funkce:
    - [Samoobslužné obnovení hesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) pro hybridní Azure AD
    
## <a name="compliance-features"></a>Funkce kompatibility

Vaše předplatné aplikace Microsoft 365 Business obsahuje funkce, které vám pomohou udržet soulad a regulační standardy.

- **[Přehled zásad prevence ztrát dat](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP můžete nastavit tak, aby automaticky zjišťováním citlivých informací, například čísel kreditních karet, čísel sociálního pojištění atd., zabránil nechtěnému sdílení mimo vaši společnost.
    
- **[Exchange Online - archiv](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Licence online k archivaci umožňuje snadnou archivaci zpráv s nepřetržitou zálohou dat. Ukládá všechny e-mailové zprávy, včetně odstraněných položek, pro případ, že budou později potřebné k odhalení nebo obnovení. Kromě toho můžete použít různé zásady uchovávání informací pro zachování e-mailových dat pro blokování soudních sporů, eDiscovery nebo pro splnění požadavků na shodu.
    
- **[Ochrana informací Azure](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Ochrana informací pomáhá řídit přístup k citlivým informacím v e-mailech a dokumentech s ovládacími prvky jako "Nepředávat dál" a "nekopírovat". Můžete také klasifikovat citlivé informace jako "důvěrné" a určit, jak mohou být tajné informace sdíleny mimo podnik a uvnitř podniku. Pro e-maily a dokumenty je snadné použít šifrování v podnikové třídě, aby byly informace soukromé. Microsoft 365 Business zahrnuje všechny funkce [plánu ochrany informací Azure 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Můžete také nainstalovat doplněk klienta pro ochranu informací Azure pro aplikace sady Office. Další informace naleznete v [příručce správce klienta ochrany informací o Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).

Tyto funkce lze spravovat v centru pro dodržování &amp; zabezpečení a v centru pro správu nástroje Intune. V průběhu času budou zjednodušené ovládací prvky přidány do střediska Microsoft 365 Business Admin Center.
  
    
## <a name="faq"></a>Časté otázky

 ### <a name="are-these-security-features-available-in-all-markets"></a>Jsou tyto bezpečnostní prvky k dispozici na všech trzích?
  
Ano, tyto funkce jsou k dispozici na všech trzích, kde se prodává společnost Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak najdu centrum pro dodržování zabezpečení &amp; ?
  
1. [Přihlaste se k aplikaci Microsoft 365 Business](https://portal.microsoft.com/) pomocí pověření pro správu. 
    
2. V levém navigačním poli vyhledejte **centra pro správu** a rozbalte je. 
    
    ![V levém navigačním středisku v centru Microsoft 365 Admin Center zvolte centrum pro správu.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Zvolte **shodu &amp; zabezpečení** a přejděte do centra &amp; kompatibility zabezpečení.