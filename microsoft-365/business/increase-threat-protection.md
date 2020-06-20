---
title: Zvýšení ochrany před hrozbami pro Microsoft 365 pro firmy
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
description: Nastavte pokročilou ochranu před hrozbami Office 365 a chraňte citlivá data před phishingem, malwarem a dalšími hrozbami.
ms.openlocfilehash: d5510cdc082781fd9a1776e86b1bab1d8a2723d6
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "44786200"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany před hrozbami

Tento článek vám pomůže zvýšit ochranu v předplatném Microsoft 365 a chránit je před phishingem, malwarem a dalšími hrozbami. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebou bezpečnosti, jako jsou advokátní kanceláře a zdravotnické kliniky.

Než začnete, zkontrolujte si zabezpečené skóre Office 365. Zabezpečené skóre Office 365 analyzuje zabezpečení vaší organizace na základě vašich pravidelných aktivit a nastavení zabezpečení a přiřadí skóre. Začněte tím, že vezmete na vědomí své aktuální skóre. Chcete-li zvýšit skóre, proveďte akce doporučené v tomto článku. Cílem není dosáhnout maximálního skóre, ale být si vědom příležitostí k ochraně vašeho prostředí, které nemají negativní vliv na produktivitu vašich uživatelů. 

Další informace naleznete v tématu [Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšení úrovně ochrany proti malwaru v poště

Vaše prostředí Office 365 nebo Microsoft 365 zahrnuje ochranu proti malwaru. Tuto ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) adresu a přihlaste se pomocí přihlašovacích údajů k účtu správce. 
    
2. V &amp; Centru dodržování předpisů zabezpečení v levém navigačním podokně v části Správa **hrozeb**zvolte **Zásady** \> **ochrany proti malwaru**.
    
3. Poklepáním na výchozí zásadu upravte tuto zásadu pro celou společnost.
    
4. Vyberte **Nastavení**.
    
5. V části **Filtr běžných typů příloh**vyberte možnost **Zapnuto**. Typy souborů, které jsou blokovány jsou uvedeny v okně přímo pod tímto ovládacím prvkem. Ujistěte se, že přidáte tyto typy souborů:
   - ade, adp, ani, bas, bat, chm, cmd, com, CPL, CRT, HLP, HT, HTA, INF, ins, ISP, práce, JS, JSE, LNK, MDA, MDB, MDE, MDZ, MSC, MSI, MSP, MST, PCD, reg, scr, SCT, SHS, url, VB, VBE, VBS, WSC, WSF, WSH, exe, pif  <br/> 
   
   V případě potřeby můžete později přidat nebo odstranit typy souborů.
    
6. Vyberte **Uložit.**
    
Další informace naleznete v [tématu Anti-malware protection](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrana před ransomwarem

Ransomware omezuje přístup k datům šifrováním souborů nebo zamykáním počítačových obrazovek. Poté se snaží vydírat oběti tím, že požádá o "výkupné", obvykle ve formě kryptocurrencí, jako je Bitcoin, výměnou za přístup k datům. 
  
Chcete-li chránit před ransomwarem, vytvořte jedno nebo více pravidel toku pošty a blokujte přípony souborů, které se běžně používají pro ransomware. (Tato pravidla jste přidali v [kroku zvýšení úrovně ochrany proti malwaru v kroku pošty.)](#raise-the-level-of-protection-against-malware-in-mail) Můžete také upozornit uživatele, kteří obdrží tyto přílohy v e-mailu.

Kromě souborů, které jste zablokovali v předchozím kroku, je vhodné vytvořit pravidlo upozorňované uživatele před otevřením příloh souborů sady Office, které obsahují makra. Ransomware může být skryt uvnitř maker, takže varují uživatele, aby tyto soubory neotevírali od lidí, které neznají.

Vytvoření pravidla přenosu pošty:
  
1. Přejděte do centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> a zvolte **Centrum pro správu** \> **Exchange**.
    
2. V kategorii **tok pošty** vyberte **pravidla**.
    
3. Vyberte **+** a pak vyberte **Vytvořit nové pravidlo**.
    
4. **Chcete-li** zobrazit úplnou sadu voleb, vyberte v dolní části dialogového okna možnost Další volby. 
    
5. Použijte nastavení pravidla v následující tabulce. Výchozí hodnoty použijte pro zbytek nastavení, pokud je nechcete změnit.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornění uživatelů před otevřením příloh souborů Office**||
|:-----|:-----|:-----|
|Name (Název)  <br/> |Pravidlo ochrany proti ransomwaru: upozorňujte uživatele  <br/>  |
|Toto pravidlo použijte, pokud . . .  <br/> |Jakákoli příloha . . . přípona souboru odpovídá . . .  <br/> |
|Určení slov nebo frází  <br/> |Přidejte tyto typy souborů:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Do následujících . . .  <br/> |Upozornit příjemce zprávou  <br/> |
|Zadejte text zprávy  <br/> |Neotevírejte tyto typy souborů od osob, které neznáte, protože mohou obsahovat makra se škodlivým kódem.  <br/> |
   
Další informace najdete tady:
  
- [Jak se vypořádat s ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Obnovení OneDrivu](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zastavení automatického přeposílání e-mailů

Hackeři, kteří získají přístup k poštovní schránce uživatele, mohou ukrást poštu nastavením poštovní schránky tak, aby automaticky přesměrovávala e-maily. K tomu může dojít i bez vědomí uživatele. Chcete-li tomu zabránit, nakonfigurujte pravidlo toku pošty. 
  
Chcete-li vytvořit pravidlo přenosu pošty, podívejte se na [toto krátké video](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:
  
1. V Centru pro správu Microsoftu 365 vyberte Exchange **Centra pro správu** \> **Exchange**.
    
2. V kategorii **tok pošty** vyberte **pravidla**.
    
3. Vyberte **+** a pak vyberte **Vytvořit nové pravidlo**.
    
4. Chcete-li zobrazit všechny možnosti, vyberte v dolní části dialogového okna **další volby.** 
    
5. Použijte nastavení v následující tabulce. Výchozí hodnoty použijte pro zbytek nastavení, pokud je nechcete změnit.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornění uživatelů před otevřením příloh souborů Office**|
|:-----|:-----|
|Name (Název)  <br/> |Zabránit automatickému předávání e-mailů do externích domén  <br/> |
|Toto pravidlo použijte, pokud ...  <br/> |Odesílatel . . . je externí/interní . . . Uvnitř organizace  <br/> |
|Přidat podmínku  <br/> |Vlastnosti zprávy . . . obsahovat typ zprávy . . . Automatické přeposílání  <br/> |
|Do následujících ...  <br/> |Blokovat zprávu . . . odmítnout zprávu a uvést vysvětlení.  <br/> |
|Zadejte text zprávy  <br/> |Automatické předávání e-mailů mimo tuto organizaci je z bezpečnostních důvodů zabráněno.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrana e-mailů před phishingovými útoky

Pokud jste pro prostředí Office 365 nebo Microsoft 365 nakonfigurovali jednu nebo více vlastních domén, můžete nakonfigurovat cílenou ochranu proti phishingu. Ochrana proti phishingu atp, která je součástí rozšířené ochrany před internetovými útoky office 365, může pomoci chránit vaši organizaci před škodlivými phishingovými útoky založenými na zosobnění a jinými phishingovými útoky. Pokud jste nenakonfigurovali vlastní doménu, nemusíte to dělat.
  
Doporučujeme začít s touto ochranou vytvořením zásady pro ochranu nejdůležitějších uživatelů a vlastní domény. 

Chcete-li vytvořit zásady ochrany proti podvodným zprávám ATP, podívejte se na [toto krátké školicí video](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com). 
    
2. V &amp; Centru dodržování předpisů zabezpečení v levém navigačním podokně v části Správa **hrozeb**zvolte **Zásady**.
    
3. Na stránce **Zásady** zvolte **ATP anti-phishing**.
    
4. Na stránce **Anti-phishing** vyberte **+ Vytvořit**. Průvodce spustí, který vás provede definováním zásad ochrany proti phishingu.
    
5. Zadejte název, popis a nastavení zásad, jak je doporučeno v následující tabulce. Další podrobnosti naleznete [v tématu Informace o zásadách ochrany proti podvodným zprávám ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby.
    

|**Nastavení nebo možnost**<br/>|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Doména a nejcennější zaměstnanci kampaně  <br/> |
|Popis  <br/> |Zajistěte, aby se nejdůležitější zaměstnanci a naše doména nezosobili.  <br/> |
|Přidání uživatelů k ochraně  <br/> |Vyberte **+ Přidat podmínku, Příjemce je**. Zadejte uživatelská jména nebo zadejte e-mailovou adresu kandidáta, manažera kampaně a dalších důležitých zaměstnanců. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobněním.  <br/> |
|Přidání domén k ochraně  <br/> |Vyberte **+ Přidat podmínku, Doména příjemce je**. Pokud jste ji definovali, zadejte vlastní doménu přidruženou k vašemu předplatnému Microsoft 365. Můžete zadat více než jednu doménu.  <br/> |
|Výběr akcí  <br/> |Pokud e-mail odesílá zosobněný uživatel: Zvolte **Přesměrovat zprávu na jinou e-mailovou adresu**a zadejte e-mailovou adresu správce zabezpečení. například *Alice <span> <span> @contoso.com*. Pokud je e-mail odesílán zosobněnou doménou: Zvolte **zprávu Karanténa**.  <br/> |
|Inteligence poštovní schránky  <br/> |Ve výchozím nastavení je při vytváření nové zásady ochrany proti podvodným zprávám vybrána informace o poštovní schránce. Ponechejte toto nastavení **zapnuto,** pokud nejlepší.  <br/> |
|Přidání důvěryhodných odesílatelů a domén  <br/> |Zde můžete přidat vlastní doménu nebo jiné důvěryhodné domény.  <br/> |
|Aplikuje se na  <br/> |Vyberte **Doména příjemce je**. V části **Některý z těchto**vyberte **Vybrat**. Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso. <span> <span> com*, v seznamu a pak vyberte **Přidat**. Vyberte **Hotovo**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrana před škodlivými přílohami a soubory pomocí bezpečných příloh ATP

Lidé pravidelně odesílají, přijímají a sdílejí přílohy, jako jsou dokumenty, prezentace, tabulky a další. Není vždy snadné zjistit, zda je příloha bezpečná nebo škodlivá pouhým pohledem na e-mailovou zprávu. Ochrana office 365 Advanced Threat Protection obsahuje ochranu bezpečné přílohy ATP, ale tato ochrana není ve výchozím nastavení zapnutá. Doporučujeme vytvořit nové pravidlo začít používat tuto ochranu. Tato ochrana se vztahuje na soubory v SharePointu, OneDrivu a Microsoft Teams.
  
Chcete-li vytvořit zásady bezpečné přílohy atp, podívejte se na [toto krátké video](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) aplikaci a přihlaste se pomocí účtu správce. 
    
2. V &amp; Centru dodržování předpisů zabezpečení v levém navigačním podokně v části Správa **hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné přílohy ATP**.
    
4. Na stránce Bezpečné přílohy můžete tuto ochranu široce použít zaškrtnutím políčka **Zapnout atp pro SharePoint, OneDrive a Microsoft Teams.** 
    
5. Tuto možnost **+** vyberte, chcete-li vytvořit novou zásadu. 
    
6. Použijte nastavení v následující tabulce. 
    
7. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby.
    

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Blokovat aktuální a budoucí e-maily s detekované malware.  <br/> |
|Popis  <br/> |Zablokujte aktuální a budoucí e-maily a přílohy pomocí zjištěných malwaru.  <br/> |
|Uložení příloh neznámé odpovědi malwaru  <br/> |Vyberte **Blokovat - Blokovat aktuální a budoucí e-maily a přílohy s detekované malware**.  <br/> |
|Přesměrovat přílohu při zjišťování  <br/> |Povolit přesměrování (zaškrtněte toto políčko) Zadejte účet správce nebo nastavení poštovní schránky pro karanténu.          Pokud dojde k výpadku časového času nebo chybě, použijte výše uvedený výběr , pokud dojde k výpadku časového období nebo chybě malwaru (toto políčko zaškrtněte).  <br/> |
|Aplikuje se na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace naleznete v [tématu Nastavení zásad ochrany proti phishingu ochrany proti phishingu v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrana před phishingovými útoky pomocí bezpečných odkazů ATP

Hackeři někdy skrývají škodlivé weby v odkazech v e-mailu nebo jiných souborech. Bezpečné odkazy na ochranu ATP (ATP) office 365, které jsou součástí rozšířené ochrany před internetovými hrozbami Office 365, mohou pomoci chránit vaši organizaci tím, že v e-mailových zprávách a dokumentech Office poskytují ověření času kliknutí na webové adresy (URL). Ochrana je definována prostřednictvím zásad bezpečného propojení ATP.
  
Doporučujeme provést následující akce:
  
- Upravte výchozí zásadu a zvyšte ochranu.
    
- Přidejte novou zásadu cílenou pro všechny příjemce ve vaší doméně.
    
Chcete-li nastavit bezpečné odkazy ATP, podívejte se na [toto krátké školicí video](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com) aplikaci a přihlaste se pomocí účtu správce. 
    
2. V &amp; Centru dodržování předpisů zabezpečení v levém navigačním podokně v části Správa **hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné odkazy ATP**.
    
Změna výchozích zásad:
  
1. Na stránce Bezpečné odkazy vyberte v části **Zásady, které platí pro celou organizaci**, **výchozí** zásady. 
    
2. V **části Nastavení, která se vztahují na obsah kromě e-mailu**, vyberte **Microsoft 365 Apps pro podniky, Office pro iOS a Android**.
    
3. Vyberte **Uložit**. 
    
Vytvoření nové zásady cílené na všechny příjemce ve vaší doméně:
  
1. Na stránce Bezpečné odkazy vyberte v části **Zásady, které platí pro celou organizaci**, **+** vytvořte novou zásadu. 
    
2. Použijte nastavení uvedená v následující tabulce.
    
3. Vyberte **Uložit**. 

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Zásady bezpečných odkazů pro všechny příjemce v doméně  <br/> |
|Výběr akce pro neznámé potenciálně škodlivé adresy URL ve zprávách  <br/> |Vyberte **Zapnuto - adresy URL budou přepsány a porovnány se seznamem známých škodlivých odkazů, když uživatel klikne na odkaz**.  <br/> |
|Použití bezpečných příloh ke skenování obsahu ke stažení  <br/> |Toto pole vyberte.  <br/> |
|Aplikuje se na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace naleznete v [tématu Bezpečné odkazy na zabezpečení ATP Office 365](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Přejděte do Centra pro správu Intune

1. Přihlaste se na [portál Azure](https://portal.azure.com/).

2. Vyberte **Všechny služby** a zadejte *Intune* do **vyhledávacího pole**.

3. Jakmile se výsledky zobrazí, vyberte start vedle **Microsoft Intune,** aby bylo oblíbené a snadno k nalezení později.

Kromě Centra pro správu můžete pomocí Intune zaregistrovat a spravovat zařízení vaší organizace. Další informace najdete v [tématu Možnosti podle metody registrace pro zařízení s Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) a [možnosti registrace pro zařízení spravovaná službou Intune](https://docs.microsoft.com/intune/enrollment-options).
