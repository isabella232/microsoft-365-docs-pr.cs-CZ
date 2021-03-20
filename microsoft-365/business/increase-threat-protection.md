---
title: Zvýšení ochrany před hrozbou pro Microsoft 365 pro firmy
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
description: Nastavte si Microsoft Defender pro Office 365 a chraňte citlivá data před útoky phishing, malwarem a dalšími hrozbami.
ms.openlocfilehash: 0424fd56e30477f4e8d9e84b7ac78ba6255781fa
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913280"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany před hrozbou

Tento článek vám pomůže zvýšit ochranu v předplatném Microsoftu 365, abyste chránili před útoky phishing, malwarem a dalšími hrozbami. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebami zabezpečení, jako jsou právní kanceláře a zdravotní péče.

Než začnete, podívejte se na zabezpečené skóre Office 365. Zabezpečené skóre Office 365 analyzuje zabezpečení vaší organizace na základě vašich pravidelných aktivit a nastavení zabezpečení a přiřadí skóre. Začněte tím, že si poznamenejte aktuální skóre. Pokud chcete zvýšit skóre, proveďte akce doporučené v tomto článku. Cílem není dosáhnout maximálního skóre, ale vědět o možnostech ochrany vašeho prostředí, které negativně neovlivňuje produktivitu vašich uživatelů.

Další informace najdete v tématu [Microsoft Secure Score](../security/mtp/microsoft-secure-score.md).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšení úrovně ochrany před malwarem v poště

Vaše prostředí Office 365 nebo Microsoft 365 zahrnuje ochranu před malwarem. Tuto ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:

1. Přejděte na [https://protection.office.com](https://protection.office.com) stránku a přihlaste se pomocí přihlašovacích údajů účtu správce.

2. V Centru dodržování předpisů zabezpečení v levém navigačním podokně &amp; v části Správa **hrozeb** zvolte **Zásady** \> **proti malwaru**.

3. Poklikejte na výchozí zásadu a upravte tuto zásadu pro celou společnost.

4. Vyberte **Nastavení**.

5. V části Common Attachment Types Filter (Filtr **běžných** typů příloh) vyberte **On (V).** Typy souborů, které jsou zablokované, jsou uvedené v okně přímo pod tímto ovládacím prvku. Nezapomeňte přidat tyto typy souborů:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   V případě potřeby můžete později přidat nebo odstranit typy souborů.

6. Vyberte **Uložit.**

Další informace najdete v tématu [Ochrana proti malwaru v EOP](../security/office-365-security/anti-malware-protection.md).

## <a name="protect-against-ransomware"></a>Ochrana před ransomwarem

Ransomware omezuje přístup k datům šifrováním souborů nebo uzamknutím obrazovek počítače. Pak se snaží vydírat peníze od obětí tím, že žádá o "výkupné", obvykle ve formě kryptoměn, jako je Bitcoin, výměnou za přístup k datům.

Pokud chcete chránit před ransomwarem, vytvořte jedno nebo více pravidel toku pošty, která blokují přípony souborů, které se běžně používají pro ransomwar. (Tato pravidla jste přidali v kroku zvýšit úroveň ochrany před [malwarem](#raise-the-level-of-protection-against-malware-in-mail) v kroku pošty.) Uživatele, kteří tyto přílohy dostanou, můžete taky upozornit v e-mailu.

Kromě souborů, které jste zablokovali v předchozím kroku, je vhodné vytvořit pravidlo, které uživatele upozorní před otevřením příloh souborů Office, které obsahují makra. Ransomware může být skrytý uvnitř maker, takže uživatele upozorňte, aby tyto soubory neotevřeli od lidí, které neznají.

Vytvoření pravidla přenosu pošty:

1. Přejděte do Centra pro správu na <https://admin.microsoft.com> stránce a zvolte Centra pro **správu** \> **Exchange**.

2. V **kategorii tok** pošty vyberte **pravidla**.

3. Vyberte **+** a pak vyberte Vytvořit nové **pravidlo**.

4. Pokud **chcete zobrazit** úplnou sadu možností, vyberte v dolní části dialogového okna další možnosti.

5. Pro pravidlo použijte nastavení v následující tabulce. Pokud je nechcete změnit, použijte výchozí hodnoty pro zbytek nastavení.

6. Vyberte **Uložit**.

|Nastavení|Upozornění uživatelů před otevřením příloh souborů Office||
|---|---|---|
|Name (Název)|Anti-ransomware rule: warn users|
|Toto pravidlo použijte, pokud . . .|Jakákoli příloha . . . příponu souboru odpovídá . . .|
|Zadání slov nebo frází|Přidejte tyto typy souborů:  <br/> tečka, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Proveďte následující akce. . .|Oznámení příjemci zprávou|
|Poskytnutí textu zprávy|Tyto typy souborů neotevřete od lidí, které nevíte, protože můžou obsahovat makra se škodlivým kódem.|

Další informace najdete tady:

- [Ransomware: Jak snížit riziko](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Obnovení OneDrivu](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Zastavení automatického přeposílání e-mailů

Hackeři, kteří získají přístup k poštovní schránce uživatele, získají přístup k e-mailu tak, že nastaví poštovní schránku tak, aby automaticky přeposlala e-maily. Může k tomu dojít i bez vědomí uživatele. Pokud tomu chcete zabránit, nakonfigurujte pravidlo toku pošty.

Pokud chcete vytvořit pravidlo přenosu pošty, podívejte se na [toto krátké video](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:

1. V Centru pro správu Microsoftu 365 vyberte **Centra pro správu** \> **Exchange**.

2. V **kategorii tok** pošty vyberte **pravidla**.

3. Vyberte **+** a pak vyberte Vytvořit nové **pravidlo**.

4. Pokud chcete zobrazit všechny možnosti, **vyberte** v dolní části dialogového okna Další možnosti.

5. Použijte nastavení v následující tabulce. Pokud je nechcete změnit, použijte výchozí hodnoty pro zbytek nastavení.

6. Vyberte **Uložit**.

|Nastavení|Upozornění uživatelů před otevřením příloh souborů Office|
|---|---|
|Name (Název)|Zabránění automatickému přeposílání e-mailů do externích domén|
|Toto pravidlo použijte, pokud ...|Odesílatel . . . je externí/interní . . . Uvnitř organizace|
|Přidat podmínku|Vlastnosti zprávy . . zahrnout typ zprávy . . . Automatické přeposílání|
|Proveďte následující kroky...|Zablokujte zprávu . . . odmítnout zprávu a zahrnout vysvětlení.|
|Poskytnutí textu zprávy|Automatické přeposílání e-mailů mimo tuto organizaci je z bezpečnostních důvodů zabráněno.|


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrana e-mailu před útoky phishing

Pokud jste nakonfigurovali jednu nebo více vlastních domén pro prostředí Office 365 nebo Microsoft 365, můžete nakonfigurovat cílenou anti-phishingovou ochranu. Ochrana proti phishingu, která je součástí programu Microsoft Defender pro Office 365, pomáhá chránit vaši organizaci před útoky phishing založenými na zosobnění a dalšími útoky phishing. Pokud jste nenakonfigurovali vlastní doménu, nemusíte to dělat.

Doporučujeme začít s touto ochranou vytvořením zásady, která bude chránit nejdůležitější uživatele a vaši vlastní doménu.

Pokud chcete v Microsoft Defenderu pro Office 365 vytvořit anti-phishingovou zásadu, podívejte se na toto krátké školicí  [video](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)nebo proveďte následující kroky:

1. Přejděte na [https://protection.office.com](https://protection.office.com).

2. V Centru dodržování předpisů zabezpečení v levém navigačním podokně &amp; v části Správa **hrozeb** zvolte **Zásady**.

3. Na stránce **Zásady** zvolte **Anti-phishing**.

4. Na stránce **Anti-phishing** vyberte **+ Vytvořit**. Spustí se průvodce, který vás provede definováním zásad ochrany proti útokům phishing.

5. Podle doporučení v následující tabulce zadejte název, popis a nastavení zásad. Další informace najdete v tématu [Informace o zásadách ochrany před útoky phishing v aplikaci Microsoft Defender pro možnosti Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Po prošetřování nastavení zvolte Podle potřeby **možnost** Vytvořit tuto zásadu nebo Uložit.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Domain and most valuable campaign staff|
|Popis|Ujistěte se, že nejdůležitější zaměstnanci a naše doména se nezosobní.|
|Přidání uživatelů k ochraně|Vyberte **+ Přidat podmínku, příjemce je**. Zadejte uživatelská jména nebo zadejte e-mailovou adresu kandidáta, manažera kampaně a dalších důležitých zaměstnanců. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobněním.|
|Přidání domén k ochraně|Vyberte **+ Přidat podmínku, doména příjemce je**. Pokud jste si jednu definovali, zadejte vlastní doménu přidruženou k vašemu předplatnému Microsoft 365. Můžete zadat víc než jednu doménu.|
|Volba akcí|Pokud e-mail posílá zosobněný uživatel: Zvolte **Přesměrovat** zprávu na jinou e-mailovou adresu a zadejte e-mailovou adresu správce zabezpečení. například *Alice <span> <span> @contoso.com*. Pokud e-mail odesílá zosobněná doména: Zvolte **Karanténní zpráva**.|
|Inteligentní funkce poštovní schránky|Ve výchozím nastavení je při vytváření nové anti-phishingové zásady vybraná inteligentní funkce poštovní schránky. Nejlepších výsledků **dosáhnete, když** toto nastavení necháte na.|
|Přidání důvěryhodných odesílatelů a domén|Tady můžete přidat vlastní doménu nebo jiné důvěryhodné domény.|
|Platí pro|Vyberte **Doména příjemce je**. V **části Kterýkoli z těchto** možností vyberte **Zvolit**. Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso. <span> <span> com*, v seznamu a pak vyberte **Přidat**. Vyberte **Hotovo**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Ochrana před škodlivými přílohami a soubory pomocí bezpečných příloh

Lidé pravidelně posílají, přijímají a sdílejí přílohy, jako jsou dokumenty, prezentace, tabulky a další. Není vždycky snadné zjistit, jestli je příloha bezpečná nebo škodlivá, jenom když se podíváme na e-mailovou zprávu. Program Microsoft Defender pro Office 365 obsahuje ochranu bezpečných příloh, ale tato ochrana není ve výchozím nastavení zapnutá. Doporučujeme vytvořit nové pravidlo, abyste mohli tuto ochranu začít používat. Tato ochrana se vztahuje na soubory v SharePointu, OneDrivu a Microsoft Teams.

Pokud chcete vytvořit zásadu bezpečné přílohy, podívejte se na toto [krátké video](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo proveďte následující kroky:

1. Přejděte na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí svého účtu správce.

2. V Centru dodržování předpisů zabezpečení v levém navigačním podokně &amp; v části Správa **hrozeb** zvolte **Zásady**.

3. Na stránce Zásady zvolte Bezpečné **přílohy**.

4. Na stránce Bezpečné přílohy tuto ochranu obecně použijte zaškrtnutím políčka Zapnout atp pro **SharePoint, OneDrive** a Microsoft Teams.

5. Tuto **+** možnost vyberte, pokud chcete vytvořit novou zásadu.

6. Použijte nastavení v následující tabulce.

7. Po prošetřování nastavení zvolte Podle potřeby **možnost** Vytvořit tuto zásadu nebo Uložit.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Blokování aktuálních a budoucích e-mailů pomocí zjištěného malwaru|
|Popis|Zablokujte aktuální a budoucí e-maily a přílohy pomocí zjištěného malwaru.|
|Uložení příloh s neznámou odpovědí malwaru|Vyberte **Blokovat – blokování aktuálních a budoucích e-mailů a příloh zjištěný malwarem**|
|Přesměrování přílohy při zjišťování|Povolte přesměrování (zaškrtněte toto políčko) Zadejte účet správce nebo nastavení poštovní schránky pro karanténu.          Použijte výše uvedený výběr v případě, že dojde k malwarové kontrole příloh nebo dojde k chybě (zaškrtněte toto políčko).|
|Platí pro|Doména příjemce je . . . vyberte doménu.|

Další informace najdete v tématu [Nastavení zásad ochrany před útoky phishing v programu Microsoft Defender pro Office 365](../security/office-365-security/set-up-anti-phishing-policies.md).

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Ochrana před útoky phishing pomocí bezpečných odkazů

Hackeři někdy skryj škodlivé weby v odkazech v e-mailu nebo jiných souborech. Bezpečné odkazy, které jsou součástí programu Microsoft Defender pro Office 365, pomáhají chránit vaši organizaci tím, že v e-mailových zprávách a dokumentech Office poskytují ověření webových adres (URL) po kliknutí. Ochrana je definovaná prostřednictvím zásad bezpečných odkazů.

Doporučujeme provést následující akce:

- Pokud chcete zvýšit ochranu, změňte výchozí zásadu.

- Přidejte novou zásadu, která je zaměřená na všechny příjemce ve vaší doméně.

Pokud chcete nastavit bezpečné odkazy, podívejte se na [toto krátké](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)školicí video nebo proveďte následující kroky:

1. Přejděte na [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí svého účtu správce.

2. V Centru dodržování předpisů zabezpečení v levém navigačním podokně &amp; v části Správa **hrozeb** zvolte **Zásady**.

3. Na stránce Zásady zvolte Bezpečné **odkazy**.

Změna výchozí zásady:

1. Na stránce Bezpečné odkazy vyberte v části **Zásady,** které platí pro celou organizaci, **výchozí** zásadu.

2. V **části Nastavení, která se vztahují** na obsah kromě e-mailu, vyberte **Microsoft 365 Apps pro podniky, Office pro iOS a Android.**

3. Vyberte **Uložit**.

Vytvoření nové zásady zaměřené na všechny příjemce ve vaší doméně:

1. Na stránce Bezpečné odkazy vyberte v části **Zásady,** které platí pro celou organizaci, **+** novou zásadu.

2. Použijte nastavení uvedená v následující tabulce.

3. Vyberte **Uložit**.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Zásady bezpečných odkazů pro všechny příjemce v doméně|
|Výběr akce pro neznámé potenciálně škodlivé adresy URL ve zprávách|Vyberte **Za– Adresy URL se přepíšou a** zaškrtnou v seznamu známých škodlivých odkazů, když uživatel klikne na odkaz.|
|Použití bezpečných příloh ke skenování obsahu ke stažení|Toto pole vyberte.|
|Platí pro|Doména příjemce je . . . vyberte doménu.|

Další informace najdete v tématu [Bezpečné odkazy](../security/office-365-security/atp-safe-links.md).

## <a name="go-to-intune-admin-center"></a>Přejděte do Centra pro správu Intune.

1. Přihlaste se k [portálu Azure Portal.](https://portal.azure.com/)

2. Vyberte **Všechny služby** a do vyhledávacího pole *zadejte Intune.*

3. Jakmile se zobrazí výsledky, vyberte začátek vedle **Microsoft Intune,** aby byl oblíbený a později ho snadno najdete.

Kromě Centra pro správu můžete pomocí Intune zaregistrovat a spravovat zařízení vaší organizace. Další informace najdete v tématu [Možnosti podle způsobu](/intune/enrollment/enrollment-method-capab) registrace zařízení s Windows a Možnosti registrace zařízení [spravovaných Intune](/intune/enrollment-options).