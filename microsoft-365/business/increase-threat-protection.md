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
search.appverid:
- BCS160
- MET150
description: Nastavte pokročilou ochranu před hrozbami Office 365 a chraňte citlivá data před phishingem, malwarem a dalšími hrozbami.
ms.openlocfilehash: 2dd75b20bf203b9b8f0cdefb2459c45d1d0ccec1
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627120"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany před hrozbami

Tento článek vám pomůže zvýšit ochranu v předplatném Microsoftu 365 a chránit tak před phishingem, malwarem a dalšími hrozbami. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebou bezpečnosti, jako jsou advokátní kanceláře a kliniky zdravotní péče.

Než začnete, zkontrolujte si skóre zabezpečení Office 365. Skóre zabezpečení Office 365 analyzuje zabezpečení vaší organizace na základě vašich běžných aktivit a nastavení zabezpečení a přiřadí skóre. Začněte tím, že vezmete na vědomí své aktuální skóre. Chcete-li zvýšit skóre, proveďte akce doporučené v tomto článku. Cílem není dosáhnout maximálního skóre, ale být si vědom příležitostí k ochraně vašeho prostředí, které nemají negativní vliv na produktivitu pro vaše uživatele. 

Další informace naleznete v tématu [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšení úrovně ochrany proti malwaru v poště

Vaše prostředí Office 365 nebo Microsoft 365 zahrnuje ochranu proti malwaru. Tuto ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:
  
1. Přejděte [https://protection.office.com](https://protection.office.com) na a přihlaste se pomocí přihlašovacích údajů účtu správce. 
    
2. V Centru &amp; dodržování předpisů zabezpečení v levém navigačním podokně v části **Správa hrozeb**zvolte **Ochrana** \> **proti malwaru**.
    
3. Poklepáním na výchozí zásadu upravte tuto celopodnikovou zásadu.
    
4. Vyberte **Nastavení**.
    
5. V části **Common Attachment Types Filter**vyberte **On**. Typy souborů, které jsou blokovány jsou uvedeny v okně přímo pod tímto ovládacím prvkem. Ujistěte se, že přidáte tyto typy souborů:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, CRT, HLP, ht, hta, inf, ins, ISP, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   V případě potřeby můžete typy souborů přidat nebo odstranit později.
    
6. Vyberte **Uložit.**
    
Další informace naleznete [v tématu Anti-malware protection](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrana před ransomwarem

Ransomware omezuje přístup k datům šifrováním souborů nebo zamykáním počítačových obrazovek. Poté se pokusí vydírat oběti o peníze tím, že požádá o "výkupné", obvykle ve formě kryptocurrencí, jako je Bitcoin, výměnou za přístup k datům. 
  
Chcete-li se chránit před ransomwarem, vytvořte jedno nebo více pravidel toku pošty, která blokují přípony souborů, které se běžně používají pro ransomware. (Tato pravidla jste přidali do [zvýšení úrovně ochrany proti malwaru v e-mailovém](#raise-the-level-of-protection-against-malware-in-mail) kroku.) Můžete také upozornit uživatele, kteří obdrží tyto přílohy v e-mailu.

Kromě souborů, které jste zablokovali v předchozím kroku, je vhodné vytvořit pravidlo, které uživatele upozorní před otevřením příloh souborů sady Office, které obsahují makra. Ransomware může být skryt uvnitř maker, takže varujte uživatele, aby tyto soubory neotevírali od lidí, které neznají.

Vytvoření pravidla přenosu pošty:
  
1. Přejděte do Centra <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>pro správu na stránce a zvolte **Centra pro správu** \> **Exchange**.
    
2. V kategorii **toku pošty** vyberte **pravidla**.
    
3. Vyberte **+** a pak vyberte **Vytvořit nové pravidlo**.
    
4. Vyberte **Další volby** v dolní části dialogového okna, abyste viděli úplnou sadu voleb. 
    
5. Použijte nastavení v následující tabulce pro pravidlo. Pokud je nechcete změnit, použijte výchozí hodnoty pro zbývající nastavení.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů Office**||
|:-----|:-----|:-----|
|Name (Název)  <br/> |Pravidlo proti ransomwaru: varovat uživatele  <br/>  |
|Použijte toto pravidlo, pokud . . .  <br/> |Jakýkoli příloha . . . přípona souboru odpovídá . . .  <br/> |
|Určení slov nebo frází  <br/> |Přidejte tyto typy souborů:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Postupujte takto . . .  <br/> |Upozornit příjemce zprávou  <br/> |
|Poskytnout text zprávy  <br/> |Neotevírejte tyto typy souborů od osob, které neznáte, protože mohou obsahovat makra se škodlivým kódem.  <br/> |
   
Další informace najdete tady:
  
- [Jak se vypořádat s ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Obnovení OneDrivu](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zastavení automatického předávání e-mailů

Hackeři, kteří získají přístup k poštovní schránce uživatele, mohou ukrást poštu nastavením poštovní schránky tak, aby automaticky přesměrovala e-maily. K tomu může dojít i bez vědomí uživatele. Chcete-li tomu zabránit, nakonfigurujte pravidlo toku pošty. 
  
Chcete-li vytvořit pravidlo přenosu pošty, podívejte se na [toto krátké video](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:
  
1. V Centru pro správu Microsoftu 365 vyberte **Centra pro správu** \> **Exchange**.
    
2. V kategorii **toku pošty** vyberte **pravidla**.
    
3. Vyberte **+** a pak vyberte **Vytvořit nové pravidlo**.
    
4. Pokud chcete zobrazit všechny možnosti, vyberte **Další volby** v dolní části dialogového okna. 
    
5. Použijte nastavení v následující tabulce. Pokud je nechcete změnit, použijte výchozí hodnoty pro zbývající nastavení.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů Office**|
|:-----|:-----|
|Name (Název)  <br/> |Zabránit automatickému předávání e-mailů do externích domén  <br/> |
|Použít toto pravidlo, pokud ...  <br/> |Odesílatel . . . je externí/interní . . . Uvnitř organizace  <br/> |
|Přidat podmínku  <br/> |Vlastnosti zprávy . . . včetně typu zprávy . . . Automatické přeposílání vpřed  <br/> |
|Proveďte následující ...  <br/> |Blokovat zprávu . . . zprávu odmítnout a uvést vysvětlení.  <br/> |
|Poskytnout text zprávy  <br/> |Automatické předávání e-mailů mimo tuto organizaci je z bezpečnostních důvodů zabráněno.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrana e-mailů před phishingovými útoky

Pokud jste nakonfigurovali jednu nebo více vlastních domén pro prostředí Office 365 nebo Microsoft 365, můžete nakonfigurovat cílenou ochranu proti podvodným zprávám. Ochrana proti phishingu ATP, která je součástí rozšířené ochrany před hrozbami office 365, může pomoci chránit vaši organizaci před škodlivými phishingovými útoky založenými na zosobnění a dalšími phishingovými útoky. Pokud jste vlastní doménu nenakonfigurovali, nemusíte to dělat.
  
Doporučujeme začít s touto ochranou vytvořením zásady na ochranu nejdůležitějších uživatelů a vlastní domény. 

Chcete-li vytvořit zásady ochrany proti phishingu ATP, podívejte se na [toto krátké školicí video](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com). 
    
2. V Centru &amp; dodržování předpisů zabezpečení v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce **Zásady** zvolte **ochrana proti phishingu ATP**.
    
4. Na stránce **Anti-phishing** vyberte **+ Vytvořit**. Spustí se průvodce, který vás provede definováním zásad ochrany proti phishingu.
    
5. Zadejte název, popis a nastavení zásad, jak je doporučeno v následující tabulce. Další podrobnosti naleznete v [tématu Další informace o možnostech zásad ochrany proti phishingu ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby .
    

|**Nastavení nebo možnost**<br/>|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Doména a nejcennější zaměstnanci kampaně  <br/> |
|Popis  <br/> |Zajistěte, aby se z nich nevydávali nejdůležitější zaměstnanci a naše doména.  <br/> |
|Přidání uživatelů k ochraně  <br/> |Vyberte **+ Přidat podmínku, Příjemce je**. Zadejte uživatelská jména nebo e-mailovou adresu kandidáta, manažera kampaně a dalších důležitých zaměstnanců. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobnění.  <br/> |
|Přidání domén k ochraně  <br/> |Vyberte **+ Přidat podmínku, Doména příjemce je**. Pokud jste ji definovali, zadejte vlastní doménu přidruženou k předplatnému Microsoft 365. Můžete zadat více než jednu doménu.  <br/> |
|Výběr akcí  <br/> |Pokud je e-mail odeslán zosobněným uživatelem: Zvolte **Přesměrovat zprávu na jinou e-mailovou adresu**a zadejte e-mailovou adresu správce zabezpečení. například *Alice<span><span>@contoso.com*. Pokud je e-mail odesílán zosobněnou doménou: Zvolte **zprávu karantény**.  <br/> |
|Informace o poštovních schránce  <br/> |Ve výchozím nastavení je při vytváření nové zásady ochrany proti phishingu vybrána inteligentní služba poštovní schránky. Toto nastavení ponechte **zapnuté,** aby bylo k onomu nejlepší.  <br/> |
|Přidání důvěryhodných odesílatelů a domén  <br/> |Zde můžete přidat vlastní doménu nebo jiné důvěryhodné domény.  <br/> |
|Použito na  <br/> |Vyberte **Možnost Doména příjemce je**. V **části Některá z těchto položek**vyberte **zvolit**. Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso.<span> com <span>*, v seznamu a pak vyberte **Přidat**. Vyberte **Hotovo**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrana před škodlivými přílohami a soubory pomocí bezpečných příloh ATP

Uživatelé pravidelně posílají, přijímají a sdílejí přílohy, jako jsou dokumenty, prezentace, tabulky a další. Není vždy snadné zjistit, zda je příloha bezpečná nebo škodlivá pouhým zobrazením e-mailové zprávy. Rozšířená ochrana před internetovými hrozbami office 365 zahrnuje ochranu bezpečného přílohy ATP, ale tato ochrana není ve výchozím nastavení zapnutá. Doporučujeme vytvořit nové pravidlo začít používat tuto ochranu. Tato ochrana se vztahuje i na soubory v SharePointu, OneDrivu a Microsoft Teams.
  
Chcete-li vytvořit zásady bezpečné přílohy ochrany ATP, podívejte se na [toto krátké video](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo proveďte následující kroky:
  
1. Přejděte [https://protection.office.com](https://protection.office.com)na aplikaci a přihlaste se pomocí svého účtu správce. 
    
2. V Centru &amp; dodržování předpisů zabezpečení v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné přílohy ochrany ATP**.
    
4. Na stránce Bezpečné přílohy tuto ochranu obecně použijte zaškrtnutím políčka **Zapnout atp pro SharePoint, OneDrive a Microsoft Teams.** 
    
5. Výběrem **+** této možnosti vytvoříte novou zásadu. 
    
6. Použijte nastavení v následující tabulce. 
    
7. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby.
    

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Blokovat aktuální a budoucí e-maily s detekované malware.  <br/> |
|Popis  <br/> |Blokování aktuálních a budoucích e-mailů a příloh pomocí detekovaného malwaru.  <br/> |
|Uložení příloh neznámý malware odpověď  <br/> |Vyberte **blokovat - Blokovat aktuální a budoucí e-maily a přílohy s detekované malware**.  <br/> |
|Přesměrovat přílohu při zjišťování  <br/> |Povolit přesměrování (vyberte toto pole) Zadejte účet správce nebo nastavení poštovní schránky pro karanténu.          Použijte výše uvedený výběr, pokud dojde k výpadku nebo chybě malwaru pro přílohy (vyberte toto políčko).  <br/> |
|Použito na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace naleznete v [tématu Nastavení zásad ochrany proti podvodným zprávám ochrany proti útokům ochrany proti útokům ochrany před podvodem 265 v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrana před phishingovými útoky pomocí bezpečných odkazů ATP

Hackeři někdy skrývají škodlivé weby v odkazech v e-mailech nebo jiných souborech. Bezpečné odkazy ochrany ATP office 365 (bezpečné odkazy ATP), které jsou součástí rozšířené ochrany před hrozbami office 365, mohou pomoci chránit vaši organizaci tím, že v e-mailových zprávách a dokumentech Office poskytují ověření webových adres (URL) v době kliknutí. Ochrana je definována pomocí zásad atp bezpečné odkazy.
  
Doporučujeme provést následující kroky:
  
- Chcete-li zvýšit ochranu, upravte výchozí zásadu.
    
- Přidejte novou zásadu zaměřenou na všechny příjemce ve vaší doméně.
    
Chcete-li nastavit bezpečné odkazy ATP, podívejte se na [toto krátké školicí video](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)nebo proveďte následující kroky:
  
1. Přejděte [https://protection.office.com](https://protection.office.com)na aplikaci a přihlaste se pomocí svého účtu správce. 
    
2. V Centru &amp; dodržování předpisů zabezpečení v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné odkazy ATP**.
    
Chcete-li změnit výchozí zásadu:
  
1. Na stránce Bezpečné odkazy vyberte v části **Zásady, které platí pro celou organizaci**, **výchozí** zásady. 
    
2. V části **Nastavení, která se vztahují k obsahu kromě e-mailu**, vyberte **Aplikace Microsoft 365 pro podniky, Office pro iOS a Android**.
    
3. Vyberte **Uložit**. 
    
Vytvoření nové zásady cílené na všechny příjemce ve vaší doméně:
  
1. Na stránce Bezpečné odkazy vyberte **+** v části **Zásady, které platí pro celou organizaci**, vytvořit novou zásadu. 
    
2. Použijte nastavení uvedená v následující tabulce.
    
3. Vyberte **Uložit**. 

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Zásady bezpečných odkazů pro všechny příjemce v doméně  <br/> |
|Výběr akce pro neznámé potenciálně škodlivé adresy URL ve zprávách  <br/> |Vyberte **Zapnuto - adresy URL budou přepsány a zkontrolovány podle seznamu známých škodlivých odkazů, když uživatel klikne na odkaz**.  <br/> |
|Skenování stahovatelného obsahu pomocí bezpečných příloh  <br/> |Toto políčko zaškrtněte.  <br/> |
|Použito na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace naleznete v [office 365 ATP bezpečné odkazy](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Přejít na Centrum pro správu Intune

1. Přihlaste se na [portál Azure](https://portal.azure.com/).

2. Vyberte **Všechny služby** a do **vyhledávacího pole**zadejte *Intune* .

3. Jakmile se výsledky zobrazí, vyberte začátek vedle **Microsoft Intune,** aby byl oblíbený a později snadno k nalezení.

Kromě Centra pro správu můžete pomocí Intune zaregistrovat a spravovat zařízení vaší organizace. Další informace najdete [v tématu Capabilities by enrollment method for Windows devices](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) and Enrollment options for devices managed by [Intune](https://docs.microsoft.com/intune/enrollment-options).
