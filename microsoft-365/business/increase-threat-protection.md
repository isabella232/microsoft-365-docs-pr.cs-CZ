---
title: Zvýšení ochrany před hrozbami pro Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Nastavte Office 365 Advanced Threat Protection a chraňte citlivá data.
ms.openlocfilehash: 191e1ad301e12ae45fe3a5d6d990d2357c5d0bab
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593875"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany před hrozbami

Tento článek vám pomůže zvýšit ochranu předplatného Microsoft 365, abyste se ochránili před phishingem, malwarem a dalšími hrozbami. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebou bezpečnosti, jako jsou advokátní kanceláře a kliniky zdravotní péče.

Než začnete, zkontrolujte si skóre Office 365 Secure Score. Skóre Zabezpečení Office 365 analyzuje zabezpečení organizace Office 365 na základě vašich běžných aktivit a nastavení zabezpečení a přiřazuje skóre. Začněte tím, že vezmete na vědomí aktuální skóre. Chcete-li zvýšit skóre, dokončete akce doporučené v tomto článku. Cílem není dosáhnout maximálního skóre, ale být si vědom příležitostí k ochraně vašeho prostředí, které nemají negativní vliv na produktivitu uživatelů. 

Další informace naleznete v tématu [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšení úrovně ochrany proti malwaru v poště

Prostředí Office 365 nebo Microsoft 365 zahrnuje ochranu před malwarem. Tuto ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:
  
1. Přejděte [https://protection.office.com](https://protection.office.com) na přihlašovací údaje k účtu správce a přihlaste se pomocí přihlašovacích údajů k účtu správce. 
    
2. V Centru dodržování zabezpečení &amp; Office 365 v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady** \> **Anti-Malware**.
    
3. Poklepáním na výchozí zásady upravte tuto zásadu pro celou společnost.
    
4. Vyberte **Nastavení**.
    
5. V části **Filtr běžných typů příloh**vyberte **Zapnuto**. Typy souborů, které jsou blokovány, jsou uvedeny v okně přímo pod tímto ovládacím prvkem. Ujistěte se, že přidáte tyto typy souborů:
   - ade, adp, ani, bas, netopýr, chm, cmd, com, CPL, CRT, HLP, Ht, HTA, INF, ins, ISP, práce, JS, JSE, Lnk, mda, MDB, MDE, MDZ, MSC, MSI, MSP, Mst, PCD, Reg, SCR, sct, shs, url, VB, vbe, vbs, wsc, wsf, wsh, wsh, exe,  <br/> 
   
   V případě potřeby můžete později přidat nebo odstranit typy souborů.
    
6. Vyberte **Uložit.**
    
Další informace naleznete v [tématu Ochrana proti malwaru](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ochrana před ransomwarem

Ransomware omezuje přístup k datům šifrováním souborů nebo uzamčením počítačových obrazovek. Poté se snaží vydírat oběti o peníze tím, že požádá o "výkupné", obvykle ve formě kryptocurrencí, jako je Bitcoin, výměnou za přístup k datům. 
  
Chcete-li chránit před ransomwarem, vytvořte jedno nebo více pravidel toku pošty, abyste zablokovali přípony souborů, které se běžně používají pro ransomware. (Tato pravidla jste přidali do [zvýšení úrovně ochrany proti malwaru v](#raise-the-level-of-protection-against-malware-in-mail) kroku pošty.) Můžete také upozornit uživatele, kteří obdrží tyto přílohy v e-mailu.

Kromě souborů, které jste zablokovali v předchozím kroku, je vhodné vytvořit pravidlo, které uživatele upozorní před otevřením příloh souborů sady Office, které obsahují makra. Ransomware může být skryt uvnitř maker, takže varovat uživatele, aby tyto soubory neotevírat od lidí, které neznají.

Vytvoření pravidla přenosu pošty:
  
1. Přejděte do Centra <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>pro správu na adrese a zvolte **Správce center** \> **Exchange**.
    
2. V kategorii **tok pošty** vyberte **pravidla**.
    
3. Vyberte **+** a vyberte **Vytvořit nové pravidlo**.
    
4. Vyberte **Další volby** v dolní části dialogového okna, abyste viděli úplnou sadu možností. 
    
5. Použijte nastavení v následující tabulce pro pravidlo. Použijte výchozí hodnoty pro zbytek nastavení, pokud je nechcete změnit.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů Office**||
|:-----|:-----|:-----|
|Name (Název)  <br/> |Pravidlo ochrany proti ransomwaru: varujte uživatele  <br/>  |
|Toto pravidlo použijte, pokud . . .  <br/> |Jakýkoli příloha . . . přípona souboru odpovídá . . .  <br/> |
|Určení slov nebo frází  <br/> |Přidejte tyto typy souborů:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Postupujte takto . . .  <br/> |Upozornit příjemce zprávou  <br/> |
|Poskytnutí textu zprávy  <br/> |Neotevírejte tyto typy souborů od osob, které neznáte, protože mohou obsahovat makra se škodlivým kódem.  <br/> |
   
Další informace najdete tady:
  
- [Jak se vypořádat s ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Obnovení OneDrivu](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zastavení automatického předávání e-mailů

Hackeři, kteří získají přístup k poštovní schránce uživatele, mohou ukrást poštu nastavením poštovní schránky tak, aby automaticky přesměrovala e-maily. K tomu může dojít i bez vědomí uživatele. Chcete-li tomu zabránit, nakonfigurujte pravidlo toku pošty. 
  
Chcete-li vytvořit pravidlo přenosu pošty, podívejte se na [toto krátké video](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:
  
1. V Centru pro správu Microsoftu 365 vyberte Možnost **Správce center** \> **Exchange**.
    
2. V kategorii **tok pošty** vyberte **pravidla**.
    
3. Vyberte **+** a vyberte **Vytvořit nové pravidlo**.
    
4. Chcete-li zobrazit všechny možnosti, vyberte **další volby** v dolní části dialogového okna. 
    
5. Použijte nastavení v následující tabulce. Použijte výchozí hodnoty pro zbytek nastavení, pokud je nechcete změnit.
    
6. Vyberte **Uložit**.
    
|**Nastavení**|**Upozornit uživatele před otevřením příloh souborů Office**|
|:-----|:-----|
|Name (Název)  <br/> |Zabránění automatickému předávání e-mailů do externích domén  <br/> |
|Toto pravidlo použijte, pokud ...  <br/> |Odesílatel . . . je externí/interní . . . Uvnitř organizace  <br/> |
|Přidat podmínku  <br/> |Vlastnosti zprávy . . . zahrňte typ zprávy . . . Automatické přeposílání vpřed  <br/> |
|Postupujte takto ...  <br/> |Zablokujte zprávu . . . zprávu odmítnout a obsahovat vysvětlení.  <br/> |
|Poskytnutí textu zprávy  <br/> |Automatické předávání e-mailů mimo tuto organizaci je z bezpečnostních důvodů zabráněno.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Chraňte svůj e-mail před phishingovými útoky

Pokud jste nakonfigurovali jednu nebo více vlastních domén pro prostředí Office 365 nebo Microsoft 365, můžete nakonfigurovat cílenou ochranu proti phishingu. Ochrana ochrany proti phishingu atp, která je součástí pokročilé ochrany před hrozbami Office 365, může pomoci chránit vaši organizaci před škodlivými phishingovými útoky založenými na zosobnění a dalšími phishingovými útoky. Pokud jste vlastní doménu nenakonfigurovali, nemusíte to dělat.
  
Doporučujeme začít s touto ochranou vytvořením zásady na ochranu nejdůležitějších uživatelů a vlastní domény. 

Chcete-li vytvořit zásady ochrany proti phishingu atp, podívejte se [na toto krátké tréninkové video](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:
  
1. Přejděte na [https://protection.office.com](https://protection.office.com). 
    
2. V Centru dodržování zabezpečení &amp; Office 365 v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce **Zásady** zvolte **ochrana proti phishingu atp**.
    
4. Na stránce **Ochrany proti phishingu** vyberte **+ Vytvořit**. Průvodce spustí, že vás provede definováním zásad ochrany proti phishingu.
    
5. Zadejte název, popis a nastavení zásad, jak je doporučeno v následující tabulce. Další podrobnosti naleznete v tématu Další informace [o možnostech zásad ochrany proti phishingu atp](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby.
    

|**Nastavení nebo možnost**<br/>|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Doména a nejcennější zaměstnanci kampaně  <br/> |
|Popis  <br/> |Ujistěte se, že nejdůležitější zaměstnanci a naše doména nejsou vydávány.  <br/> |
|Přidání uživatelů pro ochranu  <br/> |Vyberte **+ Přidat podmínku, Příjemce je**. Zadejte uživatelská jména nebo zadejte e-mailovou adresu kandidáta, manažera kampaně a dalších důležitých zaměstnanců. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobněním.  <br/> |
|Přidání domén pro ochranu  <br/> |Vyberte **+ Přidat podmínku, doména příjemce je**. Pokud jste ji definovali, zadejte vlastní doménu přidruženou k předplatnému Microsoft 365. Můžete zadat více než jednu doménu.  <br/> |
|Výběr akcí  <br/> |Pokud je e-mail odeslán zosobněným uživatelem: Zvolte **Přesměrovat zprávu na jinou e-mailovou adresu**a zadejte e-mailovou adresu správce zabezpečení. Například *Alice<span><span>@contoso.com*. Pokud je e-mail odeslán zosobněnou doménou: Zvolte **karanténní zprávu**.  <br/> |
|Inteligence poštovní schránky  <br/> |Ve výchozím nastavení je při vytváření nových zásad ochrany proti phishingu vybrána informace o poštovních schránce. Pro dosažení nejlepších výsledků nechte toto nastavení **zapnuto.**  <br/> |
|Přidání důvěryhodných odesílatelů a domén  <br/> |Zde můžete přidat vlastní doménu nebo jiné důvěryhodné domény.  <br/> |
|Použito na  <br/> |Vyberte **Možnost Doména příjemce je**. V **části Některý z nich**vyberte **Zvolit**. Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso.<span> v <span>* seznamu a pak vyberte **Přidat**. Vyberte **Hotovo**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ochrana před škodlivými přílohami a soubory pomocí příloh ATP Safe

Uživatelé pravidelně posílají, přijímali a sdílejí přílohy, jako jsou dokumenty, prezentace, tabulky a další. Není vždy snadné zjistit, zda je příloha bezpečná nebo škodlivá pouhým pohledem na e-mailovou zprávu. Office 365 Advanced Threat Protection obsahuje ochranu bezpečné přílohy ATP, ale tato ochrana není ve výchozím nastavení zapnutá. Doporučujeme vytvořit nové pravidlo pro zahájení používání této ochrany. Tato ochrana se vztahuje i na soubory v SharePointu, OneDrivu a Microsoft Teams.
  
Chcete-li vytvořit zásady bezpečné přílohy atp, podívejte se na [toto krátké video](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo proveďte následující kroky:
  
1. Přejděte [https://protection.office.com](https://protection.office.com)na a přihlaste se pomocí účtu správce. 
    
2. V Centru dodržování zabezpečení &amp; Office 365 v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné přílohy atp**.
    
4. Na stránce Bezpečné přílohy použijte tuto ochranu široce zaškrtnutím políčka **Zapnout atp pro SharePoint, OneDrive a Microsoft Teams.** 
    
5. Výběrem vyberte, **+** že vytvoříte novou zásadu. 
    
6. Použijte nastavení v následující tabulce. 
    
7. Po kontrole nastavení zvolte **Vytvořit tuto zásadu** nebo **Uložit**podle potřeby.
    

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Blokujte současné a budoucí e-maily pomocí zjištěného malwaru.  <br/> |
|Popis  <br/> |Zablokujte aktuální a budoucí e-maily a přílohy pomocí zjištěného malwaru.  <br/> |
|Uložení příloh neznámou odpovědí na malware  <br/> |Vyberte **Blokovat - Blokovat aktuální a budoucí e-maily a přílohy s zjištěným malware**.  <br/> |
|Přesměrování přílohy při detekci  <br/> |Povolit přesměrování (zaškrtněte toto pole) Zadejte účet správce nebo nastavení poštovní schránky pro karanténu.          Pokud dojde k výpadku časového období nebo chybě malwaru nebo chybě ( zaškrtněte toto pole).  <br/> |
|Použito na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace najdete v tématu [Nastavení zásad ochrany proti phishingu office 365 .](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Ochrana před phishingovými útoky pomocí bezpečných odkazů ATP

Hackeři někdy skrývají škodlivé weby v odkazech v e-mailech nebo jiných souborech. Bezpečné odkazy atp (ATP Safe Links) pro Office 365, které jsou součástí rozšířené ochrany hrozeb Office 365, mohou pomoci chránit vaši organizaci tím, že v e-mailových zprávách a dokumentech Office zajistí ověření webových adres (URL) čas od kliknutí. Ochrana je definována prostřednictvím zásad atp safe links.
  
Doporučujeme provést následující kroky:
  
- Upravte výchozí zásady pro zvýšení ochrany.
    
- Přidejte novou zásadu cílí na všechny příjemce ve vaší doméně.
    
Chcete-li nastavit bezpečné odkazy atp, podívejte se [na toto krátké tréninkové video](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)nebo proveďte následující kroky:
  
1. Přejděte [https://protection.office.com](https://protection.office.com)na a přihlaste se pomocí účtu správce. 
    
2. V Centru dodržování zabezpečení &amp; Office 365 v levém navigačním podokně v části **Správa hrozeb**zvolte **Zásady**.
    
3. Na stránce Zásady zvolte **bezpečné odkazy ATP**.
    
Změna výchozí zásady:
  
1. Na stránce Bezpečné odkazy vyberte v části **Zásady, které se vztahují k celé organizaci,** **výchozí** zásady. 
    
2. V **části Nastavení, která se vztahují k obsahu kromě e-mailu**, vyberte **Office 365 ProPlus, Office pro iOS a Android**.
    
3. Vyberte **Uložit**. 
    
Vytvoření nové zásady cílené na všechny příjemce ve vaší doméně:
  
1. Na stránce Bezpečné odkazy vyberte v části **Zásady, které se vztahují k celé organizaci,** **+** a vytvořte novou zásadu. 
    
2. Použijte nastavení uvedená v následující tabulce.
    
3. Vyberte **Uložit**. 

|**Nastavení nebo možnost**|**Doporučené nastavení** <br/>|
|:-----|:-----|
|Name (Název)  <br/> |Zásady bezpečných odkazů pro všechny příjemce v doméně  <br/> |
|Vyberte akci pro neznámé potenciálně škodlivé adresy URL ve zprávách  <br/> |Vyberte **Zapnuto - adresy URL budou přepsány a kontrolovány podle seznamu známých škodlivých odkazů, když uživatel klikne na odkaz**.  <br/> |
|Kontrola obsahu ke stažení pomocí bezpečných příloh  <br/> |Toto pole zaškrtněte.  <br/> |
|Použito na  <br/> |Doména příjemce je . . . vyberte svou doménu.  <br/> |
   
Další informace naleznete v [tématu bezpečné odkazy na ochrana ATP pro Office 365](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Přejít na Centrum pro správu Intune

1. Přihlaste se na [portál Azure](https://portal.azure.com/).

2. Vyberte **Všechny služby** a do **vyhledávacího pole**zadejte *Intune* .

3. Jakmile se výsledky zobrazí, vyberte start vedle **Microsoft Intune,** aby bylo oblíbené a snadno najít později.

Kromě Centra pro správu můžete pomocí Intune zaregistrovat a spravovat zařízení vaší organizace. Další informace naleznete v [tématu Možnosti podle metody registrace pro zařízení s Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) a [možnosti registrace pro zařízení spravovaná intune](https://docs.microsoft.com/intune/enrollment-options).
