---
title: Funkce zabezpečení aplikace Microsoft Business 365
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Další informace o funkcích zabezpečení, které jsou součástí Microsoft 365 Business.
ms.openlocfilehash: 17bcc57d57e837f18b05f66cfd54185324f3cad8
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983171"
---
# <a name="microsoft-365-business-security-features"></a>Funkce zabezpečení aplikace Microsoft Business 365

Microsoft 365 Business nabízí zjednodušený bezpečnostní prvky pro ochranu dat na počítače, telefony a tablety.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Funkce zabezpečení aplikace Microsoft 365 Business admin center

Můžete spravovat mnoho funkcí zabezpečení Microsoft 365 Business ve středisku pro správce, který poskytuje zjednodušený způsob, jak tyto funkce zapnout, nebo vypnout. Ve středisku pro správce provádět následující akce:
  
![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
- [Nastavení správy aplikace pro Android nebo iOS zařízení](app-protection-settings-for-android-and-ios.md) . 
    
    Tato nastavení zahrnují odstranění souborů z neaktivní zařízení po určité nastavené době, šifrování souborů práce, které vyžadují, aby uživatelé nastavit kód PIN, atd.
    
- [Nastavení ochrany aplikací pro zařízení Windows 10](protection-settings-for-windows-10-devices.md) . 
    
    Toto nastavení lze použít data společnosti na obou vlastněných nebo osobní vlastnictví zařízení.
    
- [Nastavení ochrany zařízení pro zařízení Windows 10](protection-settings-for-windows-10-pcs.md) . 
    
    Můžete povolit šifrování [nástrojem BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) , chcete-li pomoci chránit data v případě ztráty nebo krádeže zařízení a povolit [Guard zneužití systému Windows](https://go.microsoft.com/fwlink/p/?linkid=871404) poskytovat rozšířenou ochranu před ransomware. 
    
- [Odebrání dat společnosti ze zařízení](remove-company-data.md)
    
    Můžete vzdálené vymazání dat společnosti, pokud zařízení dojde ke ztrátě, odcizení, nebo zaměstnanec opustí společnost.
    
- [Zařízení Windows 10 obnovit tovární nastavení](reset-devices-to-factory-settings.md) . 
    
    Můžete obnovit Windows 10 zařízení, jejichž ochrana nastavení zařízení je použita.
    
## <a name="additional-security-features"></a>Další funkce zabezpečení 

Rozšířené funkce v Microsoft 365 Business lze chránit vaši firmu před internetovými hrozbami a chránit citlivé informace.
  
- **[Office 365 Advanced Threat Protection](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Advanced Threat Protection (ATP) pomáhá chránit své podnikání proti útokům ransomware navržen tak, aby napadnout zaměstnance nebo informace o zákaznících a sofistikované útoky typu phishing. Funkce:
    
  - Prohledávání příloh propracované a technologii AI analýzy zjistit a odstranit nebezpečné zprávy.
    
  - Automatické kontroly webových odkazů v e-mailu pro hodnocení jsou součástí podvodného postupu. To umožňuje bezpečný přístup k nebezpečným webům.
    
- **[Přehled zásad prevence ztráty dat](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP můžete nastavit na automatické zjištění citlivé informace, například čísla kreditních karet, čísla sociálního pojištění, atd., proti jejich neúmyslnému sdílení mimo organizaci.
    
- **[Exchange Online - archiv](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online archivaci licence umožňuje snadno archivovat data průběžné zálohování. Uloží všechny e-maily uživatele, včetně odstraněných položek v případě, že jsou později potřebné pro zjištění nebo obnovení. Navíc můžete použít zásady uchovávání informací různých zachovat data e-mailu pro blokování sporu, služba eDiscovery, nebo splnit požadavky na shodu.
    
- **[Ochrana údajů v Azure](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Informace ochrana pomáhá řídit přístup k důvěrným informacím v e-mailu a dokumentů s ovládacími prvky, stejně jako "není dopředu" a "Nekopírujte." Můžete také klasifikovat jako "Důvěrné" citlivé informace a určit, jak utajované informace mohou být sdíleny mimo a uvnitř podniku. Enterprise třída šifrování je snadno použitelná e-maily a dokumenty, které chcete zachovat soukromí vašich informací. Microsoft 365 Business zahrnuje všechny funkce [Azure informace ochrana plán 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Můžete také nainstalovat Azure ochrana údajů klient doplněk pro aplikace sady Office. Další podrobnosti naleznete v [příručce neznáte klienta Azure ochrana údajů](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).
    
- **[Veškeré funkce Intune na portálu Azure](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Přístup k Intune center admin na portálu Azure umožňuje nastavit další funkce zabezpečení, například správu zařízení, iPhone a Android zařízení a Správa rozšířeného zařízení pro Windows, MacOS, nejsou k dispozici prostřednictvím společnosti Microsoft 365 business admin center.
    
Následující části popisují, jak lze spravovat tyto funkce zabezpečení &amp; souladu a Centrum správce Intune. Zjednodušené ovládací prvky budou časem přidány Microsoft 365 Business centru pro správu.
  
## <a name="set-up-advanced-threat-protection-features"></a>Nastavení funkce rozšířené ochrany ohrožení

- **Ochrana proti nebezpečným přílohám:** ATP identifikován škodlivý obsah otevírání příloh e-mailů ve virtuálním prostředí a provádění analýzy výsledné chování. Obsah je posoudit a určit svůj záměr (ať už normální nebo nebezpečný), a ATP blokuje dodání nebezpečné přílohy, pomáhá chránit před podvodnými postupy typu phishing a ransomware infekcemi. Aktivaci ochrany přílohy naleznete v tématu [nastavení zásad bezpečné přílohy ATP Office 365](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775).
    
- Ochranu vašeho prostředí po kliknutí škodlivé odkazy: ATP také kontroluje odkazy v e-mailu v okamžiku kliknutí na ně. Pokud odkaz není bezpečné, uživatel je varován, aby na webu nebo informován, že webu byl zablokován. To pomáhá chránit před podvodnými postupy typu phishing. Můžete [nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) nebo [nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
## <a name="set-up-dlp-features"></a>Nastavení funkcí DLP

Příklad, jak nastavit zásady na ochranu proti osobně identifikovatelných informací (PII), viz [Vytvoření DLP zásady ze šablony](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) . 
  
DLP je dodávána s mnoha šablon připravených k použití zásad pro mnoho různá národní prostředí. Například finanční Data Austrálie, Kanada osobní informace Act, USA finanční Data, atd. Úplný seznam naleznete v tématu [šablony zásad DLP co patří](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Všechny tyto šablony lze povolit podobný příklad šablony PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Nastavení uchovávání e-mailů s Exchange Online archivaci

 Funkce **Exchange Online archivaci** licence poskytnout možnost zachovat dodržování předpisů a norem email zachováním obsahu pro účely služba eDiscovery. Také pomáhá snížit riziko v případě soudních sporů a poskytuje způsob, jak obnovit data po narušení zabezpečení nebo potřebujete obnovit odstraněné položky. Chcete-li aktivovat tyto funkce, můžete použít blokování sporu zachovat veškerý obsah uživatelského nebo použít zásady uchovávání informací pro větší možnosti přizpůsobení. 
  
**Soudní spory podržte:** Můžete zachovat veškerý obsah poštovní schránky včetně odstraněných položek vložením celé poštovní schránky uživatele na soudní spory podržte. 
    
Chcete-li umístit poštovní schránky blokované sporu ve středisku pro správce:
    
1. V navigace vlevo, go **uživatelům** \> **aktivních uživatelů**.
    
2. Vyberte uživatele, jejichž poštovní schránky, které chcete umístit na soudní spory podržte a rozbalte v podokně uživatelské **Nastavení e-mailu** a v oblasti **Další nastavení** zvolte **Vlastnosti upravit Exchange**.
    
3. Na stránce poštovní schránky pro uživatele zvolte ** funkce poštovní schránky ** na navigace vlevo a pak zvolte **Povolit** odkaz pod **soudní spory podržte**.
    
4. Dialogové okno můžete určit sporu **podržte soudní spory** podržte trvání v poli **Doba trvání podržte soudní spory** , ponechte pole prázdné, pokud chcete umístit nekonečné blokování. Můžete přidat poznámky a přímý vlastník pole mail na webu, bude pravděpodobně nutné vysvětlit více o sporu podržte \> **Uložit**.
    
**Uchovávání informací:** Můžete povolit zásady uchovávání informací vlastní, například má být zachována po určitou dobu nebo trvale odstranit obsah na konci období uchování. Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
## <a name="set-up-azure-information-protection-features"></a>Nastavení funkcí Azure ochrana údajů

Ochrana Azure informace (AIP) je cloudové řešení, které pomáhá organizaci ke klasifikaci a volitelně chránit své dokumenty a e-maily s použitím štítků. Popisky lze automaticky správce, kteří definují pravidla a podmínky ručně podle uživatele nebo jejich kombinace, kde uživatelé jsou uvedena doporučení.

Schopnost použít následující omezení při odesílání e-mailů v aplikaci Outlook na webu je automaticky povolena pro všechny uživatele:
  
- **Dál**: příjemci mohou zprávu číst, ale jejich nelze předat dál, vytisknout nebo kopírování obsahu
    
- **Šifrování**: celá zpráva je šifrovaná. Příjemci musí přijmout další kroky k potvrzení své identity před přístupem k obsahu zašifrované a nelze odebrat šifrování.
    
- **Důvěrné**: dává zaměstnanců ve vaší organizaci úplná oprávnění k obsahu e-mailů a příloh, ale nikoli osoby mimo organizaci. Vlastníci dat můžete sledovat a obsah kdykoli odvolat.
    
- **Vysoce důvěrné**: Toto omezení lze použít vysoce důvěrné údaje, umožňující zaměstnancům, aby zobrazit, upravit a odpovědět, ale není dál, vytisknout nebo zkopírovat data. Vlastníci dat můžete sledovat a obsah kdykoli odvolat.

### <a name="make-sure-azure-information-protection-is-activated"></a>Zkontrolujte, zda že je aktivován Azure ochrana údajů

Chcete-li ověřit, zda je aktivován AIP:

1. Přihlášení k [portálu Azure](https://portal.azure.com/).

2. Vyberte **všechny služby** a typ *Ochrany informace Azure* do **Vyhledávacího pole**.

3. Po zobrazení výsledků, klepněte na tlačítko start Další **Ochrana informací Azure** Chcete-li oblíbenou položku a možné později snáze najít.

4. **Ochrana informací Azure** vyberte \> **Aktivace ochrany** a zkontrolujte zda je nastaven stav na aktivovaný. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Zobrazit popisky zásad a výchozí ochrana informací Azure 

Chcete-li zobrazit a upravit existující štítky:

1. Na panelu Digital dashboard ochrana informací Azure vyberte **klasifikace** \> **štítky**. <br/>![Standardní popisky pro ochranu informací Azure.](media/AIPLabels.png)

2. Můžete zvolit libovolný popisek chcete-li zobrazit možnosti, můžete změnit zobrazovaný název barvy, např.
 
3. Viz [změnit a vytvořit nové štítky s](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Pokud chcete vytvořit vlastní. 

### <a name="install-the-azure-information-protection-client-manually"></a>Ruční instalace klienta Azure ochrana údajů

Chcete-li ručně nainstalovat klienta AIP:

1. **AzInfoProtection.exe** lze stáhněte z [webu služby Stažení softwaru](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Můžete ověřit, že instalace odpracovaných zobrazení dokumentu aplikace Word a přesvědčíte se, že je k dispozici na kartě **Domů** na možnost **chránit** . <br/>![Kartu Zámek rozevíracího seznamu v dokumentu Word.](media/Word_Protect.png)

Pro další informace naleznete v tématu [Instalace klienta](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)

## <a name="go-to-intune-admin-center"></a>Přejít do centra pro správu Intune

1. Přihlášení k [portálu Azure](https://portal.azure.com/).

2. Vyberte **všechny služby** a typ v *Intune* do **Vyhledávacího pole**.

3. Po zobrazení výsledků, klepněte na tlačítko start Další **Microsoft Intune** Chcete-li oblíbenou položku a možné později snáze najít.
 
Pomocí Intune můžete zapisovat a spravovat zařízení v organizaci. Další informace naleznete v tématu [funkce pomocí metody zápisu zařízení systému Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) a [Možnosti zápisu zařízení spravuje Intune](https://docs.microsoft.com/intune/enrollment-options).
    
## <a name="faq"></a>Časté otázky

 ### <a name="are-these-security-features-available-in-all-markets"></a>Jsou k dispozici tyto funkce zabezpečení na všech trzích?
  
Ano, tyto funkce jsou k dispozici na všech trzích, kde se prodává Microsoft 365 Business.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Jak najít zabezpečení &amp; centra kompatibility?
  
1. [Microsoft 365 Business přihlásit](https://portal.microsoft.com/) pomocí pověření správce. 
    
2. V levá navigace vyhledejte **Admin Center** a rozbalte ji. 
    
    ![V navigace vlevo ve středisku pro správce služeb Microsoft 365 zvolte Admin Center.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Zvolte **zabezpečení &amp; souladu** přejdete na zabezpečení &amp; centra kompatibility.