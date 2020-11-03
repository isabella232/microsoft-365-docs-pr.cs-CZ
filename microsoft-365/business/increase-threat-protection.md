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
description: Nastavení Microsoft Defenderu pro Office 365 a ochrana citlivých dat proti podvodným zprávám, malwaru a dalším hrozbám
ms.openlocfilehash: 2f1a26b5a2c5678871502d441b6ba64c9b011e1c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842250"
---
# <a name="increase-threat-protection"></a>Zvýšení ochrany před hrozbami

Tento článek vám pomůže zvýšit ochranu předplatného Microsoft 365 a chránit tak ochranu před útoky typu phishing, malware a další. Tato doporučení jsou vhodná pro organizace se zvýšenou potřebou zabezpečení, jako jsou třeba právní úřady a zdravotní péče.

Než začnete, zkontrolujte bezpečnostní skóre Office 365. Zabezpečené skóre Office 365 analyzuje zabezpečení vaší organizace na základě pravidelných aktivit a nastavení zabezpečení a přiřadí skóre. Začněte tím, že si poznamenejte aktuální skóre. Chcete-li zvýšit skóre, proveďte kroky doporučené v tomto článku. Cílem není dosáhnout maximálního skóre, ale mějte na paměti možnosti ochrany životního prostředí, které nepříznivě ovlivňují produktivitu uživatelů.

Další informace najdete v tématu [Microsoft Secure skore](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Zvýšení úrovně ochrany proti malwaru v poště

Prostředí Office 365 nebo Microsoft 365 obsahuje ochranu proti malwaru. Ochranu můžete zvýšit blokováním příloh s typy souborů, které se běžně používají pro malware. Zvýšení ochrany proti malwaru v e-mailu:

1. Přejděte na stránku [https://protection.office.com](https://protection.office.com) s přihlašovacími údaji účtu správce a přihlaste se.

2. V centru zabezpečení &amp; dodržování předpisů klikněte v levém navigačním podokně v části **Správa hrozeb** na **Policy** \> **anti-malware** zásad.

3. Poklikáním na výchozí zásadu upravte tuto zásadu celé společnosti.

4. Vyberte **Nastavení**.

5. V části **Common Types Filter (běžné typy příloh** ) vyberte **zapnuto**. Blokované typy souborů jsou uvedené v okně přímo pod tímto ovládacím prvkem. Nezapomeňte přidat tyto typy souborů:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   V případě potřeby můžete později přidat nebo odstranit typy souborů.

6. Vyberte **Uložit.**

Další informace najdete v tématu [Ochrana proti malwaru v EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection).

## <a name="protect-against-ransomware"></a>Ochrana proti ransomwaru

Ransomwaru omezuje přístup k datům šifrováním souborů nebo uzamknutím počítačových obrazovek. Potom se pokusí extort peníze od obětí tím, že požádají o "Ransom", obvykle ve formě cryptocurrencies jako Bitcoinu, v Exchangi pro Access k datům.

Chcete-li chránit před ransomwaru, vytvořte jedno nebo více pravidel toku pošty a zablokujte tak přípony souborů používané pro ransomwaru. (Tato pravidla jste přidali v kroku [zvýšení úrovně ochrany proti malwaru v poště](#raise-the-level-of-protection-against-malware-in-mail) .) Můžete také varovat uživatele, kteří tyto přílohy přijímají v e-mailu.

Kromě souborů blokovaných v předchozím kroku je vhodné vytvořit pravidlo pro upozornění uživatelů před otevřením souborů, které obsahují makra. Ransomwaru můžou být skryté v makrech, takže upozorněte uživatele, aby neotevírali tyto soubory od lidí, které neznají.

Vytvoření pravidla přenosu pošty:

1. Přejděte do centra pro správu <https://admin.microsoft.com> a zvolte Exchange **Center Centre** \> **Exchange**.

2. V kategorii **tok pošty** vyberte **pravidla**.

3. Vyberte **+** a pak vyberte **vytvořit nové pravidlo**.

4. V dolní části dialogového okna vyberte **Další možnosti** , abyste viděli úplnou sadu možností.

5. Pro pravidlo použijte nastavení uvedené v následující tabulce. Pokud chcete, aby se zbývající nastavení nezměnilo, použijte výchozí hodnoty.

6. Vyberte **Uložit**.

|Nastavení|Varovat uživatele před otevřením příloh souborů Office||
|---|---|---|
|Name (Název)|Pravidlo ochrany proti ransomwaru: varovat uživatelů|
|Použijte toto pravidlo, pokud. . .|Libovolná příloha. . . Přípona souboru odpovídá. . .|
|Zadejte slova nebo fráze.|Přidejte tyto typy souborů:  <br/> dotm, DOCM, XLSM, sltm, XLA, xlam, XLL, PPTM, POTM, PPAM, PPSM, SLDM|
|Postupujte takto: . .|Upozornění příjemce zprávou|
|Zadání textu zprávy|Neotevírejte tyto typy souborů od lidí, které neznáte, protože by mohly obsahovat makra se škodlivým kódem.|

Další informace najdete tady:

- [Ransomwaru: jak snížit riziko](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Obnovení OneDrivu](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Ukončení automatického přeposílání e-mailů

Hackeři, kteří mají přístup k poštovní schránce uživatele, můžou pomocí poštovní schránky nastavit automatické přeposílání e-mailů. K tomu může dojít i bez vědomí uživatele. Aby k tomu nedocházelo, nakonfigurujte pravidlo toku pošty.

Pokud chcete vytvořit pravidlo přenosu pošty, podívejte se na [Toto krátké video](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) nebo postupujte takto:

1. V centru pro správu Microsoft 365 vyberte **centra pro správu** \> **Exchange**.

2. V kategorii **tok pošty** vyberte **pravidla**.

3. Vyberte **+** a pak vyberte **vytvořit nové pravidlo**.

4. Pokud chcete zobrazit všechny možnosti, v dolní části dialogového okna vyberte **Další možnosti** .

5. Použijte nastavení uvedené v následující tabulce. Pokud chcete, aby se zbývající nastavení nezměnilo, použijte výchozí hodnoty.

6. Vyberte **Uložit**.

|Nastavení|Varovat uživatele před otevřením příloh souborů Office|
|---|---|
|Name (Název)|Zabránění automatickému přeposílání e-mailů do externích domén|
|Použít toto pravidlo, pokud...|Odesílatele. . . je externí/interní. . . V organizaci|
|Přidat podmínku|Vlastnosti zpráv . . Uveďte typ zprávy. . . Automaticky přeposílat|
|Postupujte takto:|Zablokujte zprávu. . . odmítne zprávu a uveďte vysvětlení.|
|Zadání textu zprávy|Automatické přesměrování e-mailu mimo tuto organizaci brání z bezpečnostních důvodů.|


## <a name="protect-your-email-from-phishing-attacks"></a>Ochrana e-mailu před útoky typu phishing

Pokud jste pro Office 365 nebo Microsoft 365 nakonfigurovali jednu nebo víc vlastních domén, můžete nakonfigurovat cílovou ochranu proti podvodným zprávám. Ochrana proti podvodným zprávám, která je součástí Microsoft Defenderu pro Office 365, může pomoci ochránit vaši organizaci před útoky phishing a dalšími útoky phishing. Pokud jste nenakonfigurovali vlastní doménu, není nutné to udělat.

Doporučujeme, abyste tuto ochranu zahájili vytvořením zásad pro ochranu nejdůležitějších uživatelů a vlastní domény.

Pokud chcete v Microsoft Defenderu pro Office 365 vytvořit zásadu ochrany proti podvodným zprávám, podívejte se na  [Toto krátké video](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)a udělejte toto:

1. Přejděte na [https://protection.office.com](https://protection.office.com).

2. V centru zabezpečení &amp; dodržování předpisů klikněte v levém navigačním podokně v části **Správa hrozeb** na **zásady**.

3. Na stránce **zásady** zvolte **anti-phishing**.

4. Na stránce **anti-phishing** vyberte **+ vytvořit**. Průvodce vás provede postupem definování zásad ochrany před útoky phishing.

5. V následující tabulce zadejte název, popis a nastavení zásad. Další informace najdete v článku [informace o zásadách anti-phishingu v Microsoft Defenderu pro Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

6. Po kontrole nastavení zvolte možnost **vytvořit tuto zásadu** nebo **Uložit**.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Doména a nejdůležitější zaměstnanci kampaně|
|Popis|Zajistěte, aby většina důležitých pracovníků a domény nebyly zosobněny.|
|Přidání uživatelů pro ochranu|Vyberte **+ Přidat podmínku, příjemce**. Zadejte uživatelská jména nebo zadejte e-mailovou adresu kandidáta, manažera kampaně a další důležité zaměstnance. Můžete přidat až 20 interních a externích adres, které chcete chránit před zosobněním.|
|Přidání domén pro ochranu|Vyberte **+ Přidat podmínku a doménu příjemce**. Zadejte vlastní doménu přidruženou k předplatnému Microsoft 365, pokud jste ji definovali. Můžete zadat víc než jednu doménu.|
|Zvolte akce|Pokud e-mail odešle zosobněným uživatelem: zvolte **Přesměrovat zprávu na jinou e-mailovou adresu** a zadejte e-mailovou adresu správce zabezpečení. například *Alice <span> <span> @contoso. com*. Pokud je e-mailem odeslána zosobněná doména: zvolte **karanténa**.|
|Zpravodajské zpravodajství|Při vytváření nových zásad ochrany proti útokům phishing je ve výchozím nastavení vybraná možnost zpravodajské zprávy. Abyste dosáhli nejlepších výsledků, **Toto nastavení nechte** .|
|Přidání důvěryhodných odesílatelů a domén|Zde můžete přidat vlastní doménu nebo jakékoli jiné důvěryhodné domény.|
|Použito na|Vyberte **doménu příjemce**. V **některém z těchto** vyberte **Vybrat.** Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény, například *contoso. <span> <span> com* , v seznamu a potom vyberte **Přidat**. Vyberte **Hotovo**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Ochrana před škodlivými přílohami a soubory pomocí bezpečných příloh

Lidé pravidelně odesílají, přijímají a sdílejí přílohy, jako jsou dokumenty, prezentace, tabulky a další. Je to vždy snadné zjistit, zda je příloha bezpečná nebo škodlivá pouhým zobrazením e-mailové zprávy. Microsoft Defender pro Office 365 zahrnuje bezpečný ochranu příloh, ale ve výchozím nastavení není tato ochrana zapnutá. Doporučujeme vytvořit nové pravidlo, které začne používat tuto ochranu. Tato ochrana se rozšiřuje na soubory na SharePointu, OneDrivu a Microsoft Teams.

Chcete-li vytvořit zásady bezpečné přílohy, Sledujte [Toto krátké video](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nebo udělejte následující kroky:

1. Přejděte na stránku [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu správce.

2. V centru zabezpečení &amp; dodržování předpisů klikněte v levém navigačním podokně v části **Správa hrozeb** na **zásady**.

3. Na stránce Zásady vyberte **zabezpečené přílohy**.

4. Na stránce Bezpeční přílohy zaškrtněte políčko **zapnout ATP pro SharePoint, OneDrive a Microsoft Teams** .

5. Výběrem **+** vytvoříte novou zásadu.

6. Použijte nastavení uvedené v následující tabulce.

7. Po kontrole nastavení zvolte možnost **vytvořit tuto zásadu** nebo **Uložit**.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Blokovat aktuální a budoucí e-maily pomocí zjištěného malwaru|
|Popis|Blokovat aktuální a budoucí e-maily a přílohy zjištěným malwarem.|
|Uložit přílohy neznámá odpověď malwaru|Select **Block-zablokuje aktuální a budoucí e-maily a přílohy se zjištěným malwarem**.|
|Přesměrování přílohy při zjišťování|Povolit přesměrování (zaškrtněte toto políčko) zadejte účet správce nebo nastavení poštovní schránky karantény.          Výše uvedený výběr použijte, pokud se při hledání v přílohách vyprší časový limit nebo došlo k chybě (zaškrtněte toto políčko).|
|Použito na|Doména příjemce je. . . Vyberte svoji doménu.|

Další informace najdete v článku [nastavení zásad ochrany před útoky phishing v Microsoft Defenderu pro Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Ochrana před útoky typu phishing pomocí bezpečných odkazů

Hackeři někdy skrývají škodlivé weby v odkazech v e-mailu nebo jiných souborech. Bezpečné odkazy, součást programu Microsoft Defender pro Office 365, může pomoci ochránit vaši organizaci tím, že vám poskytne ověřování webových adres (URL) v e-mailových zprávách a dokumentech Office. Ochrana je definována zásadami bezpečných odkazů.

Doporučujeme postupovat takto:

- Změňte výchozí zásadu na zvýšit ochranu.

- Přidejte nové zásady cílené na všechny příjemce ve vaší doméně.

Pokud chcete nastavit bezpečné odkazy, podívejte se na [Toto krátké video](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)a udělejte toto:

1. Přejděte na stránku [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí účtu správce.

2. V centru zabezpečení &amp; dodržování předpisů klikněte v levém navigačním podokně v části **Správa hrozeb** na **zásady**.

3. Na stránce Zásady zvolte **Bezpeční odkazy**.

Změna výchozí zásady:

1. Na stránce Bezpeční odkazy v části **zásady, které platí pro celou organizaci** , vyberte **výchozí** zásadu.

2. V části **nastavení týkající se obsahu s výjimkou e-mailu** vyberte aplikace **Microsoft 365 pro podnik, Office pro iOS a Android**.

3. Vyberte **Uložit**.

Vytvoření nové zásady cílené na všechny příjemce ve vaší doméně:

1. Na stránce Bezpeční odkazy klikněte v části **zásady, které se týkají celé organizace** , **+** a vytvořte novou zásadu.

2. Použijte nastavení uvedená v následující tabulce.

3. Vyberte **Uložit**.

|Nastavení nebo možnost|Doporučené nastavení|
|---|---|
|Name (Název)|Zásady bezpečných odkazů pro všechny příjemce v doméně|
|Výběr akce pro neznámé potencionálně škodlivé adresy URL ve zprávách|**Po kliknutí na odkaz budou přepsány adresy URL a budou vráceny se seznamem známých nebezpečných odkazů**.|
|Použití bezpečných příloh ke skenování obsahu ke stažení|Zaškrtněte toto políčko.|
|Použito na|Doména příjemce je. . . Vyberte svoji doménu.|

Další informace najdete v článku [Bezpeční odkazy](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links).

## <a name="go-to-intune-admin-center"></a>Přejít na centrum pro správu Intune

1. Přihlaste se na [Azure Portal](https://portal.azure.com/).

2. V **poli Hledat** vyberte **všechny služby** a zadejte do *Intune* .

3. Po zobrazení výsledků vyberte spustit vedle **Microsoft Intune** , abyste ho mohli mít oblíbenou a snadno najít později.

Kromě centra pro správu můžete k registraci a správě zařízení organizace použít Intune. Další informace najdete v tématu [možnosti podle metody zápisu pro zařízení s Windows](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) a [Možnosti zápisu pro zařízení spravovaná v Intune](https://docs.microsoft.com/intune/enrollment-options).
