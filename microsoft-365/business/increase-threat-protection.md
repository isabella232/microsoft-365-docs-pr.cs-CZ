---
title: Zvyšte ochranu proti ohrožení společnosti Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Nastavení sady Office 365 Pokročilá ochrana proti ohrožení a ochrana citlivých dat
ms.openlocfilehash: 81197a8baf1c4d0cbfd898c41a305c1a99bab57c
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288109"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany proti ohrožení

Tento článek pomáhá zvýšit ochranu předplatného aplikace Microsoft 365, aby bylo možné chránit před útoky typu phishing, škodlivým softwarem a dalšími hrozbami. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebou bezpečnosti, jako jsou právnické kanceláře a zdravotnické kliniky.

Než začnete, zkontrolujte, zda je v sadě Office 365 bezpečné skóre. Sada Office 365 zabezpečené skóre analyzuje zabezpečení organizace Office 365 na základě pravidelných aktivit a nastavení zabezpečení a přiřazuje skóre. Začněte tím, že si budete brát na vědomí aktuální skóre. S ohledem na akce doporučené v tomto článku zvýšíte skóre. Cílem není dosáhnout maximálního skóre, ale uvědomit si možnosti ochrany vašeho prostředí, které negativně neovlivní produktivitu pro uživatele. 

Další informace naleznete v tématu [Microsoft Secure Score](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšit úroveň ochrany proti malwaru v poště

Prostředí sady Office 365 nebo Microsoft 365 obsahuje ochranu proti malwaru, ale tuto ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí pověření účtu pro správu. 
    
2. V centru pro správu zabezpečení &amp; sady Office 365 v levém navigačním podokně v části **řízení hrozeb**zvolte možnost **zásady** \> **ochrany proti malwaru**.
    
3. Chcete-li upravit tuto zásadu pro celou společnost, poklepejte na výchozí zásady.
    
4. Klepněte na tlačítko **Nastavení**.
    
5. V části **společné typy příloh**vyberte možnost **zapnuto**. Blokované typy souborů jsou uvedeny v okně přímo pod tímto ovládacím prvkem.  Ujistěte se, že přidáváte tyto typy souborů:
   - ADE, ADP, ani, bas, bat, CHM, cmd, com, CPL, CRT, HLP, HT, HTA, INF, INS, ISP, Job, js, jse, LNK, MDA, MDB, MDE, MDZ, MSC, MSI, MSP, MST, PCD, reg, SCR, VBS, WSC, WSF, WSH, exe, PIF  <br/> V případě potřeby můžete typy souborů přidat nebo odstranit později.
    
6. Klepněte na tlačítko **Uložit.**
    
Další informace naleznete v části [Ochrana proti malwaru](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Chraňte před Ransomware

Ransomware omezuje přístup k datům pomocí šifrování souborů nebo uzamykání počítačových obrazovek. Poté se pokouší vymárat peníze od obětí tím, že si žádá "výkupné", obvykle ve formě kryptoměn, jako je Bitpeníz, výměnou za přístup k údajům. 
  
Můžete chránit před Ransomware vytvořením jednoho nebo více pravidel pro tok zpráv, která blokují přípony souborů, které se běžně používají pro Ransomware (tyto byly přidány do [zvýšení úrovně ochrany před malwarem v kroku pošty](#raise-the-level-of-protection-against-malware-in-mail) ), nebo varovat uživatele, kteří obdrželi tyto příloh v e-mailu.

Kromě souborů blokovaných v předchozím kroku je také vhodné vytvořit pravidlo pro upozornění uživatelů před otevřením příloh souborů sady Office, které obsahují makra. Ransomware může být skryta uvnitř maker, takže uživatelé nebudou moci otevírat tyto soubory od lidí, které neznají.

Vytvoření pravidla pro přenos pošty:
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> Přejděte do centra pro správu a vyberte možnost **Výměna** **středisek** \> správy.
    
2. V kategorii **toku pošty** klepněte na tlačítko **pravidla**.
    
3. Klikněte **+** na tlačítko a potom na příkaz **vytvořit nové pravidlo**.
    
4. Klepnutím na tlačítko **Další možnosti** v dolní části dialogového okna zobrazíte úplnou sadu možností. 
    
5. Pro pravidlo použijte nastavení v následující tabulce. Ostatní nastavení ponechejte ve výchozím nastavení, pokud je nechcete změnit.
    
6. Klikněte na **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů systému Office**||
|:-----|:-----|:-----|
|Name (Název)  <br/> |Pravidlo anti-Ransomware: upozornit uživatele  <br/>  |
|Použijte toto pravidlo, pokud. . .  <br/> |Žádná příloha. . . shoduje se přípona souboru. . .  <br/> |
|Zadání slov nebo frází  <br/> |Přidat tyto typy souborů:  <br/> dotm, DOCM, XLSM, sltm, XLA, xlam, XLL, PPTM, POTM, PPAM, PPSM, SLDM  <br/>|
|Proveďte následující kroky. . .  <br/> |Upozornit příjemce zprávou  <br/> |
|Zadat text zprávy  <br/> |Neotevírejte tento typ souborů od osob, které neznáte, protože mohou obsahovat makra se škodlivým kódem.  <br/> |
   
Další informace najdete tady:
  
- [Jak se vypořádat s Ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Obnovení aplikace OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Zastavit automatické předávání e-mailu

Hackeři, kteří získají přístup k poštovní schránce uživatele, mohou vaši poštu ukrást nastavením poštovní schránky na automatické předávání e-mailu. K tomu může dojít i bez vědomí uživatele. Tomu lze předejít nakonfigurováním pravidla toku pošty. 
  
Chcete-li vytvořit pravidlo pro přenos pošty, Sledujte [Toto krátké video](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte podle následujících kroků:
  
1. V centru Microsoft 365 Admin Center klepněte na položku **admin Centers** \> **Exchange**.
    
2. V kategorii **toku pošty** klepněte na tlačítko **pravidla**.
    
3. Klikněte **+** na tlačítko a potom na příkaz **vytvořit nové pravidlo**.
    
4. Klepnutím na tlačítko **Další možnosti** v dolní části dialogového okna zobrazíte úplnou sadu možností. 
    
5. Použijte nastavení v následující tabulce. Ostatní nastavení ponechejte ve výchozím nastavení, pokud je nechcete změnit.
    
6. Klikněte na **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů systému Office**|
|:-----|:-----|
|Name (Název)  <br/> |Zakázat automatické zasílání e-mailů do externích domén  <br/> |
|Použít toto pravidlo, pokud...  <br/> |Odesílatel. . . je externí/interní. . . Uvnitř organizace  <br/> |
|Přidat podmínku  <br/> |Vlastnosti zprávy. . . obsahovat typ zprávy. . . Automatický převon  <br/> |
|Proveďte následující kroky...  <br/> |Zablokujte zprávu. . . zprávu odmítne a bude obsahovat vysvětlení.  <br/> |
|Zadat text zprávy  <br/> |Automatické předávání e-mailů mimo tuto organizaci je zabráněno z bezpečnostních důvodů.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrana e-mailů před útoky typu phishing

Pokud jste nakonfigurovali jednu nebo více vlastních domén pro prostředí Office 365 nebo Microsoft 365, můžete nakonfigurovat cílenou ochranu proti podvodné poště. Ochrana proti podvodné poště ATP, součást sady Office 365 Advanced Attack Protection, může pomoci ochránit vaši organizaci před škodlivými útoky typu phishing založenými na zosobnění a jinými útoky typu phishing. Není-li vlastní doména nakonfigurována, není třeba ji provádět.
  
Doporučujeme zahájit tuto ochranu vytvořením zásady pro ochranu nejdůležitějších uživatelů a vlastní domény. 

  
Chcete-li vytvořit protipodvodné zásady ATP, Sledujte [Toto krátké výukové video](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com). 
    
2. V centru pro správu zabezpečení &amp; sady Office 365 v levém navigačním podokně pod položkou **Správa hrozeb**zvolte **zásady**.
    
3. Na stránce **zásad** vyberte položku **ATP anti-phishing**.
    
4. Na stránce **anti-phishing** vyberte možnost **+ Create**. Spustí se průvodce, který vás provede definováním protipodvodných zásad.
    
5. Podle doporučení v následující tabulce zadejte název, popis a nastavení zásad. Další informace naleznete v tématu [informace o možnostech ATP anti-phishing zásad](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) . 
    
6. Po kontrole nastavení zvolte možnost **vytvořit tuto zásadu** nebo ji **uložte**podle potřeby.
    

|**Nastavení nebo možnost**<br/>|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Doména a nejhodnotnější zaměstnanci kampaně  <br/> |
|Popis  <br/> |Zajistěte, aby nejdůležitější zaměstnanci a Naše doména nebyly zosobovány.  <br/> |
|Přidání uživatelů k ochraně  <br/> |Vyberte možnost **+ Přidat podmínku, příjemce je**. Zadejte uživatelská jména nebo zadejte e-mailovou adresu kandidáta, vedoucího kampaně a dalších důležitých zaměstnanců. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobněním.  <br/> |
|Přidat domény k ochraně  <br/> |Vybrat **+ Přidat podmínku, doména příjemce je**. Zadejte vlastní doménu přidruženou k odběru Microsoft 365, pokud jste ji definovali. Můžete zadat více než jednu doménu.  <br/> |
|Vybrat akce  <br/> |Pokud je e-mail odeslán zosobním uživatelem: zvolte **Přesměrovat zprávu na jinou e-mailovou adresu**a zadejte e-mailovou adresu správce zabezpečení; například *Alice<span><span>@contoso. com*.          Pokud je e-mail odeslán zosobovanou doménou: zvolte **zprávu karantény**.  <br/> |
|Informace o poštovní schránce  <br/> |Ve výchozím nastavení je při vytváření nové zásady protiútoku phishing vybrána informace o poštovní schránce. Ponechejte toto nastavení **zapnuto** .  <br/> |
|Přidání důvěryhodných odesílatelů a domén  <br/> |Zde můžete přidat vlastní doménu nebo jiné důvěryhodné domény.  <br/> |
|Použito pro  <br/> |Vyberte **doménu příjemce**. V **některém z těchto kroků**vyberte možnost **Vybrat**. Vyberte možnost **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso.<span> modelu <span>com*, v seznamu a vyberte položku **Přidat**. Vyberte **Hotovo**.  <br/> |
   
Další informace naleznete v tématu [set up Microsoft Office 365 ATP anti-phishing zásady](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrana proti nebezpečným přílohám a souborům s bezpečnými přílohami ATP

Uživatelé pravidelně odesílají, přijímají a sdílejí přílohy, například dokumenty, prezentace, tabulky a další. Při pohledu na e-mailovou zprávu není vždy snadné zjistit, zda je příloha bezpečná nebo škodlivá. Sada Office 365 Pokročilá ochrana proti ohrožení zahrnuje ochranu bezpečného připojení ATP, ale tato ochrana není ve výchozím nastavení zapnuta. Doporučujeme vytvořit nové pravidlo pro zahájení používání této ochrany. Tato ochrana se rozšiřuje na soubory ve službě SharePoint, OneDrive a Microsoft týmy.
  
Chcete-li vytvořit zásadu bezpečného připojení ATP, Sledujte [Toto krátké video](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu pro správu. 
    
2. V centru pro správu zabezpečení &amp; sady Office 365 v levém navigačním podokně pod položkou **Správa hrozeb**zvolte **zásady**.
    
3. Na stránce Zásady zvolte **bezpečné přílohy ATP**.
    
4. Na stránce bezpečné přílohy můžete tuto ochranu široce použít zaškrtnutím políčka **zapnout ATP pro služby SharePoint, OneDrive a Microsoft týmy** . 
    
5. Vyberte **+** , chcete-li vytvořit novou zásadu. 
    
6. Použijte nastavení v následující tabulce. 
    
7. Po kontrole nastavení zvolte možnost **vytvořit tuto zásadu** nebo ji **uložte**podle potřeby.
    

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Blokovat aktuální a budoucí e-maily s odhalzjištěnému malwaru.  <br/> |
|Popis  <br/> |Blokovat aktuální a budoucí e-maily a přílohy s odhalzjištěnému malwaru.  <br/> |
|Uložit přílohy neznámá odezva malwaru  <br/> |Vybrat **blok-blokovat aktuální a budoucí emaily a přílohy s rozpoznazjištěnému malwaru**.  <br/> |
|Přesměrovat přílohu při detekci  <br/> |Povolit přesměrování (toto políčko zaškrtněte) zadejte účet správce nebo nastavení poštovní schránky pro karanténu.          Použijte výše uvedený výběr, pokud dojde k vyhledání chyby v přílohách nebo k chybě (zaškrtněte toto políčko).  <br/> |
|Použito pro  <br/> |Doménou příjemce je. . . Vyberte doménu.  <br/> |
   
Další informace naleznete v tématu [set up Microsoft Office 365 ATP anti-phishing zásady](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrana před útoky typu phishing pomocí bezpečných odkazů ATP

Hackeři někdy skrývají škodlivé weby v odkazech v e-mailech nebo jiných souborech. Sada Office 365 bezpečné odkazy ATP (bezpečné odkazy ATP), část sady Office 365 Pokročilá ochrana proti ohrožení, může pomoci ochránit vaši organizaci tím, že poskytuje kontrolu webových adres (URL) v e-mailových zprávách a dokumentech sady Office po kliknutí na čas. Ochrana je definována pomocí zásad pro bezpečné odkazy ATP.
  
Doporučujeme provádět následující akce:
  
- Úpravou výchozí zásady Zvyšte ochranu.
    
- Přidejte novou zásadu, která je zaměřena na všechny příjemce v doméně.
    
Chcete-li nastavit bezpečné odkazy ATP, Sledujte [Toto krátké výukové video](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu pro správu. 
    
2. V centru pro správu zabezpečení &amp; sady Office 365 v levém navigačním podokně pod položkou **Správa hrozeb**zvolte **zásady**.
    
3. Na stránce Zásady zvolte možnost **bezpečné odkazy ATP**.
    
Změna výchozí zásady:
  
1. Na stránce bezpečné odkazy v části **zásady, které platí pro celou organizaci**, vyberte **výchozí** zásadu. 
    
2. V **nastavení, které se vztahuje k obsahu s výjimkou e-mailu**, vyberte **sadu Office 365 ProPlus, Office for iOS a Android**.
    
3. Klikněte na **Uložit**. 
    
Chcete-li vytvořit novou zásadu zaměřenou na všechny příjemce v doméně, postupujte takto:
  
1. Na stránce bezpečné odkazy v části **zásady, které platí pro celou organizaci**, vytvořte klepnutím **+** novou zásadu. 
    
2. Použijte nastavení uvedená v následující tabulce.
    
3. Klikněte na **Uložit**. 

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Zásady bezpečných odkazů pro všechny příjemce v doméně  <br/> |
|Vyberte akci pro neznámé potenciálně škodlivé adresy URL ve zprávách  <br/> |Vyberete **-li položku on-URL, budou po klepnutí na odkaz znovu zapsány a zkontrolovány se seznamem známých škodlivých odkazů**.  <br/> |
|Kontrola obsahu stahovatelné pomocí bezpečných příloh  <br/> |Zaškrtněte toto políčko.  <br/> |
|Použito pro  <br/> |Doménou příjemce je. . . Vyberte doménu.  <br/> |
   
Další informace naleznete v tématu [Office 365 bezpečné odkazy ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Přejít do centra pro správu Intune

1. Podepište se na [Azure portál](https://portal.azure.com/).

2. Vyberte **všechny služby** a do **vyhledávacího pole**zadejte text v *Intune* .

3. Po zobrazení výsledků klepněte na začátek vedle položky **Microsoft Intune** , abyste jej mohli později snadno najít.

Kromě centra pro správu můžete pomocí nástroje Intune zapsat a spravovat zařízení organizace. Další informace naleznete v tématu [Capabilities pomocí metody zápisu pro zařízení systému Windows](https://docs.microsoft.com/intune/enrollment-method-capabs) a [Možnosti zápisu pro zařízení spravovaná společností Intune](https://docs.microsoft.com/intune/enrollment-options).
