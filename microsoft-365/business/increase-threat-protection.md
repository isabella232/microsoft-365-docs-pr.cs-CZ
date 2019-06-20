---
title: Zvýšit ochranu před hrozbami pro Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Nastavení Office 365 rozšířené ohrožení ochrany a chránit citlivá data.
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086287"
---
# <a name="increase-threat-protection"></a>Zvýšit ochranu před hrozbami

Tento článek pomáhá zvýšit ochranu předplatné Microsoft 365 pro ochranu před útoky typu phishing, malware a dalšími hrozbami. Tato doporučení jsou vhodné pro organizace s zvýšenou potřebu zabezpečení jako právní kanceláří a zdravotní péče kliniky.

Než začnete, zkontrolujte váš Office 365 zabezpečené skóre. Office 365 zabezpečené skóre analyzuje zabezpečení organizaci služeb Office 365, které jsou založené na pravidelných aktivit a nastavení zabezpečení a přiřadí skóre. Začněte tím, že bere na vědomí aktuální skóre. Vaše skóre se zvýší akcí doporučené v tomto článku. Cílem je dosažení maximální skóre, ale být vědomi příležitostí k ochraně prostředí, které negativně ovlivnit produktivitu uživatelů. 

Další informace naleznete v tématu [Microsoft zabezpečení skóre](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšit úroveň ochrany proti malwaru v mailu

Prostředí služeb Office 365 nebo Microsoft 365 zahrnuje ochranu proti malwaru, ale zvýšíte ochranu o blokování příloh s typy souborů, které jsou běžně používány pro malware. Ke zvýšení ochrany proti malwaru v e-mailu:
  
1. Přejít na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí pověření účtu správce. 
    
2. V zabezpečení Office 365 &amp; centra kompatibility v levém navigačním podokně v části **Správa ohrožení**zvolte **zásady** \> **Proti malwaru**.
    
3. Poklepejte na položku Výchozí zásady chcete-li upravit tuto zásadu pro celou společnost.
    
4. Klepněte na tlačítko **Nastavení**.
    
5. Ve skupinovém rámečku **Běžné typy filtr příloha**vyberte **v**. Blokované typy souborů jsou uvedeny v okně přímo pod tento ovládací prvek.  Zkontrolujte, zda že přidat typ těchto souborů:
   - ADE, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, úlohy, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> Můžete přidat nebo odstranit typy souborů později podle potřeby.
    
6. Klepněte na tlačítko **Uložit.**
    
Další informace naleznete v tématu [Ochrana proti malwaru](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Chránit před ransomware

Ransomware omezuje přístup k dat pomocí šifrování souborů nebo při uzamčení obrazovky počítače. Potom pokusí se extort peníze z obětí požádá o "ransom", obvykle v podobě cryptocurrencies jako Bitcoin, výměnou za přístup k datům. 
  
Můžete chránit před ransomware vytvořením jednoho nebo více mail toku pravidla blokování přípon souborů, které se běžně používají pro ransomware (tyto byly přidány v kroku [zvýšit úroveň ochrany proti malwaru v mail](#raise-the-level-of-protection-against-malware-in-mail) ) nebo varovat uživatele, kteří tyto přílohy v e-mailu.

Vedle souborů, které jste zablokovali v předchozím kroku je také vhodné vytvořit pravidlo, chcete-li upozornit uživatele před otevřením přílohy souborů sady Office, které obsahují makra. Ransomware může být skryté uvnitř makra, takže jsme bude varovat uživatele Chcete-li otevřít tyto soubory od uživatelů, které neznáte.

Chcete-li vytvořit pravidlo přenosu pošty:
  
1. Přejděte na stránku Správce na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> a zvolte **Admin Center** \> **Exchange**.
    
2. V kategorii **tok e-mailů** klepněte na tlačítko **pravidla**.
    
3. Klepněte na **+** a potom klepněte na tlačítko **vytvořit nové pravidlo**.
    
4. Klepněte na tlačítko **Další možnosti** v dolní části dialogového okna, chcete-li zobrazit úplnou sadu možností. 
    
5. Použijte nastavení v následující tabulce pro pravidlo. Ponechejte zbývající nastavení ve výchozím nastavení, pokud chcete změnit.
    
6. Klikněte na **Uložit**.
    
|**Nastavení**|**Varovat uživatele před otevřením přílohy souborů sady Office**||
|:-----|:-----|:-----|
|Name (Název)  <br/> |Pravidla Anti-ransomware: varovat uživatele  <br/>  |
|Použít toto pravidlo, pokud. . .  <br/> |Všechny přílohy. . . Přípona souboru. . .  <br/> |
|Zadejte slovo nebo spojení  <br/> |Přidáte tyto typy souborů:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Postupujte následujícím způsobem. . .  <br/> |Příjemce se zobrazí zpráva upozornění  <br/> |
|Zadejte text zprávy  <br/> |Nelze otevřít tyto typy souborů od uživatelů, které neznáte, protože mohou obsahovat makra pomocí škodlivého kódu.  <br/> |
   
Další informace najdete tady:
  
- [Jak zacházet s ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Obnovení aplikace OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Zastavit automatické přeposílání e-mailů

Hackeři, kteří získat přístup k poštovní schránce tohoto uživatele můžete nastavením poštovní schránky automaticky předávat e-mailové ukrást poštu. K tomu může dojít i bez vědomí uživatele. Lze tomu zabránit konfigurací pravidlo toku pošty. 
  
Chcete-li vytvořit pravidlo dopravy pošty, sledujte [Toto krátké video](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:
  
1. Ve středisku pro správce služeb Microsoft 365, klepněte na tlačítko **Admin Center** \> **Exchange**.
    
2. V kategorii **tok e-mailů** klepněte na tlačítko **pravidla**.
    
3. Klepněte na **+** a potom klepněte na tlačítko **vytvořit nové pravidlo**.
    
4. Klepněte na tlačítko **Další možnosti** v dolní části dialogového okna, chcete-li zobrazit úplnou sadu možností. 
    
5. Použijte nastavení v následující tabulce. Ponechejte zbývající nastavení ve výchozím nastavení, pokud chcete změnit.
    
6. Klikněte na **Uložit**.
    
|**Nastavení**|**Varovat uživatele před otevřením přílohy souborů sady Office**|
|:-----|:-----|
|Name (Název)  <br/> |Zabránit automatické předávání e-mailových zpráv do externích domén  <br/> |
|Použít toto pravidlo, pokud...  <br/> |Odesílatel. . . je externí nebo interní. . . Uvnitř organizace.  <br/> |
|Přidat podmínku  <br/> |Vlastnosti zprávy. . . Zahrnout typ zprávy. . . Automatické dopředu  <br/> |
|Postupujte podle následujících pokynů...  <br/> |Blokovat zprávy. . . odmítnout zprávu a zahrnout vysvětlení.  <br/> |
|Zadejte text zprávy  <br/> |Z bezpečnostních důvodů je zakázáno automatické přeposílání e-mailů mimo tuto organizaci.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Chránit před útoky typu phishing e-mail

Pokud nakonfigurujete jeden nebo více vlastních domén pro vaše prostředí služeb Office 365 nebo Microsoft 365 nakonfigurujete cílené ochrany proti útokům typu phishing. Ochrana proti útokům typu phishing ATP, součástí Office 365 Advanced ochranu před hrozbami, chránit organizaci z nebezpečného na základě zosobnění útoky typu phishing a jiné útoky typu phishing. Pokud jste nenakonfigurovali vlastní domény, není nutné provést.
  
Společnost Microsoft doporučuje, že můžete začít s touto ochranou vytvořením zásad ochrany uživatele nejdůležitější a vaší vlastní domény. 

  
Chcete-li vytvořit zásadu ATP anti-phishing, sledujte [Toto krátké video školení](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com). 
    
2. V zabezpečení Office 365 &amp; centra kompatibility v levém navigačním podokně v části **Správa ohrožení**zvolte **zásady**.
    
3. Na stránce **zásady** zvolte **podvodným ATP**.
    
4. Vyberte na stránce **Anti-phishing** , **+ vytvořit**. Spustí průvodce, který vás provede definování zásad anti-phishing.
    
5. Zadejte název, popis a nastavení zásady doporučené v grafu níže. Další informace naleznete v tématu [informace o možnostech zásady anti-phishing ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) . 
    
6. Po kontrole nastavení, zvolte **vytvořit tuto zásadu** nebo **Uložit**, podle potřeby.
    

|**Nastavení nebo možnosti**<br/>|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Domény a nejcennějších kampaně zaměstnanci  <br/> |
|Popis  <br/> |Ujistěte se, nejdůležitější, že personál a naše domény nejsou zosobňován.  <br/> |
|Přidat uživatele k ochraně  <br/> |Vyberte možnost **+ Přidat podmínku příjemce je**. Zadejte uživatelská jména nebo e-mailová adresa zájemce, Správce kampaně a ostatní důležité zaměstnanci. Můžete přidat až 20 interní a externí adresy, které chcete zabránit zosobnění.  <br/> |
|Přidání domén k ochraně  <br/> |Vyberte možnost **+ Přidat podmínku doméně příjemce je**. Pokud jste definovali jeden, zadejte vlastní domény spojené s předplatným Microsoft 365. Můžete zadat více než jednu doménu.  <br/> |
|Zvolte Akce  <br/> |Pokud je e-mail odeslán pomocí zosobněného uživatele: vyberte **přesměrovat zprávy na jinou e-mailovou adresu**a potom zadejte e-mailovou adresu správce zabezpečení; například *Alice<span><span>@contoso.com*.          Pokud zosobněného domény zasílá e-mailem: Zvolte **karantény zprávy**.  <br/> |
|Poštovní schránka intelligence  <br/> |Standardně je vybrané řady poštovní schránky při vytváření nové zásady anti-phishing. Ponechte toto nastavení **na** nejlepších výsledků.  <br/> |
|Přidání důvěryhodných odesílatelů a domén  <br/> |Zde můžete přidat své vlastní doméně nebo jiných důvěryhodných doménách.  <br/> |
|Chcete-li použít  <br/> |Vyberte položku **příjemce domény**. Pro **některá z těchto**vyberte **Zvolit**. Vyberte možnost **+ Přidat**. Zaškrtněte políčko u názvu domény, například contoso *.<span> <span>com*, v seznamu a potom vyberte možnost **Přidat**. Vyberte možnost **provést**.  <br/> |
   
Další informace naleznete v tématu [nastavení zásad anti-phishing Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrana proti nebezpečné přílohy a soubory s přílohami bezpečné ATP

Lidé pravidelně odesílat, přijímat a sdílet příloh, například dokumenty, prezentace, tabulky a další. Není vždy snadné zjistit, zda příloha je bezpečné nebo nebezpečné podle vzhledu e-mailové zprávě. Ochranu před hrozbami Advanced Office 365 zahrnuje ochranu bezpečná příloha ATP, ale tato ochrana není ve výchozím nastavení zapnuta. Doporučujeme vytvořit nové pravidlo, chcete-li začít používat tuto ochranu. Tato Ochrana sahá soubory služby SharePoint, OneDrive a Microsoft Teams.
  
Vytvoření zásady bezpečné připevnění ATP, sledujte [Toto krátké video](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo postupujte podle následujících pokynů:
  
1. Přejít na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu správce. 
    
2. V zabezpečení Office 365 &amp; centra kompatibility v levém navigačním podokně v části **Správa ohrožení**zvolte **zásady**.
    
3. Na stránce zásady zvolte **bezpečné přílohy ATP**.
    
4. Na stránce bezpečné přílohy vztahuje tato ochrana obecně zaškrtnutím políčka **Zapnout ATP pro SharePoint, OneDrive a týmy společnosti Microsoft** . 
    
5. Vyberte **+** Chcete-li vytvořit novou zásadu. 
    
6. Použijte nastavení v následující tabulce. 
    
7. Po kontrole nastavení, zvolte **vytvořit tuto zásadu** nebo **Uložit**, podle potřeby.
    

|**Nastavení nebo možnosti**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Blokuje současné i budoucí e-maily s zjištěných malware.  <br/> |
|Popis  <br/> |Blokuje současné i budoucí e-maily a přílohy s zjištěných malware.  <br/> |
|Uložit přílohy Neznámý malware odpověď  <br/> |Vyberte **blok - blok současných a budoucích e-mailů a příloh se zjištěné malware**.  <br/> |
|Příloha k přesměrování na detekci  <br/> |Povolit přesměrování (políčko) zadejte účet správce nebo nastavení poštovní schránky pro karanténní.          Použít výběr výše, pokud vyprší malware prohledávání příloh nebo dojde k chybě (políčko).  <br/> |
|Chcete-li použít  <br/> |Je doméně příjemce. . . Zadejte název domény.  <br/> |
   
Další informace naleznete v tématu [nastavení zásad anti-phishing Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Chránit před útoky typu phishing s bezpečné odkazy ATP

Hackeři někdy skrýt škodlivé weby v části odkazy v e-mailu nebo jiné soubory. Office 365 ATP bezpečné odkazy (odkazy ATP bezpečné), součástí Office 365 Advanced ochranu před hrozbami, můžete chránit vaše organizace poskytnutím čas klepněte ověřování webových adres (URL) v e-mailových zpráv a dokumentů sady Office. Ochrana je definována prostřednictvím zásad bezpečné odkazy ATP.
  
Doporučujeme provést následující:
  
- Změňte výchozí zásady ke zvýšení ochrany.
    
- Přidáte novou zásadu určen všem příjemcům v doméně.
    
Chcete-li nastavit bezpečné odkazy ATP, sledujte [Toto krátké video školení](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)nebo proveďte následující kroky:
  
1. Přejít na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu správce. 
    
2. V zabezpečení Office 365 &amp; centra kompatibility v levém navigačním podokně v části **Správa ohrožení**zvolte **zásady**.
    
3. Na stránce zásady zvolte **Bezpečné odkazy ATP**.
    
Chcete-li změnit výchozí zásady:
  
1. Na stránce bezpečné odkazy v části **zásady, které platí pro celou organizaci**vyberte **výchozí** zásady. 
    
2. V části **nastavení, jež platí pro obsah kromě e-mailů**vyberte **Office 365 ProPlus, Office pro iOS a Android**.
    
3. Klikněte na **Uložit**. 
    
Chcete-li vytvořit novou zásadu určen všem příjemcům v doméně:
  
1. Na stránce bezpečné odkazy v části **zásady, které platí pro celou organizaci**klepněte na **+** Chcete-li vytvořit novou zásadu. 
    
2. Použije nastavení uvedené v následující tabulce.
    
3. Klikněte na **Uložit**. 

|**Nastavení nebo možnosti**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Zásady bezpečné vazby pro všechny příjemce v doméně  <br/> |
|Výběr akce pro neznámé potenciálně škodlivé adresy URL ve zprávách  <br/> |Vyberte **na - URL přepsána a zkontrolována podle seznamu známé škodlivé odkazy, když uživatel klepne na odkaz**.  <br/> |
|Používat bezpečné přílohy k prohledávání obsahu ke stažení  <br/> |Zaškrtněte toto políčko.  <br/> |
|Chcete-li použít  <br/> |Je doméně příjemce. . . Zadejte název domény.  <br/> |
   
Další informace naleznete v tématu [bezpečné propojení Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Přejít do centra pro správu Intune

1. Přihlášení k [portálu Azure](https://portal.azure.com/).

2. Vyberte **všechny služby** a typ v *Intune* do **Vyhledávacího pole**.

3. Po zobrazení výsledků, klepněte na tlačítko start Další **Microsoft Intune** Chcete-li oblíbenou položku a možné později snáze najít.

Kromě admin center můžete Intune zapisovat a spravovat zařízení v organizaci. Další informace naleznete v tématu [funkce pomocí metody zápisu zařízení systému Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) a [Možnosti zápisu zařízení spravuje Intune](https://docs.microsoft.com/intune/enrollment-options).
