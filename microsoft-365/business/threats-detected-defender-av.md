---
title: Hrozby zjištěné Antivirová ochrana v programu Microsoft Defender
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Zjistěte, Antivirová ochrana v programu Microsoft Defender chrání vaše Windows zařízení před softwarovými hrozbami, jako jsou viry, malware a spyware.
ms.openlocfilehash: 7c5d000e2a8c30e17d1f890cef69fe88beed75bb
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "53465401"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>Hrozby zjištěné Antivirová ochrana v programu Microsoft Defender

Antivirová ochrana v programu Microsoft Defender chrání vaše Windows před softwarovými hrozbami, jako jsou viry, malware a spyware.

- Viry se obvykle šíří připojením kódu k jiným souborům na vašem zařízení nebo v síti a mohou způsobit nesprávnou práci infikovaných programů.
- Malware obsahuje škodlivé soubory, aplikace a kód, které mohou způsobit poškození a narušit normální používání zařízení. Malware také může povolit neoprávněný přístup, používat systémové prostředky, krást hesla a informace o účtu, zamknout vás z počítače a požádat o výkupné a další.
- Spyware shromažďuje data, například aktivitu procházení webu, a odesílá je na vzdálené servery.
 
Pokud chcete zajistit ochranu před hrozbou, Antivirová ochrana v programu Microsoft Defender používá několik metod. Mezi tyto metody patří cloudová ochrana, ochrana v reálném čase a vyhrazené aktualizace ochrany.

- Cloudová ochrana pomáhá zajistit okamžitou detekci a blokování nových a nově vznikajících hrozeb.
- Při kontrole v režimu always-on se používá monitorování chování souborů a procesů a další techniky (označované také jako ochrana *v reálném čase).*
- Vyhrazené aktualizace ochrany jsou založené na strojovém učení, lidské a automatizované analýze velkých dat a hloubkovém výzkumu odolnosti proti hrozbám. 

Další informace o malwaru a Antivirová ochrana v programu Microsoft Defender najdete v následujících článcích: 

- [Principy malwaru & jiných hrozeb](/windows/security/threat-protection/intelligence/understanding-malware)
- [Jak Microsoft identifikuje malware a potenciálně nežádoucí aplikace](/windows/security/threat-protection/intelligence/criteria)
- [Ochrana nové generace v Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>Co se stane, když se používá antivirové řešení jiné než Microsoft? 

Antivirová ochrana v programu Microsoft Defender je součástí operačního systému a je povolený na zařízeních s Windows 10. Pokud ale používáte antivirové řešení, které není od Microsoftu a používáte [Microsoft Defender](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)pro koncový bod , pak Antivirová ochrana v programu Microsoft Defender automaticky přejde do zakázaného režimu.  

Když jsou uživatelé a zákazníci v zakázaném režimu, Antivirová ochrana v programu Microsoft Defender k identifikaci hrozeb používat funkce pro plánované kontroly nebo kontroly na vyžádání. ale Antivirová ochrana v programu Microsoft Defender už nebude:

- použít jako výchozí antivirovou aplikaci.
- aktivně prohledat soubory a hledat hrozby.
- odstranit nebo vyřešit hrozby.

Pokud odinstalujete antivirové řešení, které není od microsoftu, Antivirová ochrana v programu Microsoft Defender automaticky přepne do aktivního režimu, aby vaše zařízení Windows před hrozbami.

> [!TIP]
> - Pokud používáte tento Microsoft 365, zvažte použití Antivirová ochrana v programu Microsoft Defender jako primárního antivirového řešení. Integrace může poskytovat lepší ochranu. Společně [se podívejte na Lepší: Antivirová ochrana v programu Microsoft Defender a Office 365](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus).
> - Nezapomeňte mít Antivirová ochrana v programu Microsoft Defender aktuální, i když používáte antivirové řešení, které není od Microsoftu.

## <a name="what-to-expect-when-threats-are-detected"></a>Co můžete očekávat, když jsou zjištěny hrozby

Když jsou hrozby detekovány Antivirová ochrana v programu Microsoft Defender, dějí se tyto věci:

- Uživatelé dostávají [oznámení v Windows](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e). 
- Zjišťování jsou uvedená v [Zabezpečení Windows na](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center) **stránce Historie** ochrany.  
- Pokud jste zabezpečili zařízení Windows 10 a zaregistrovali je v [Intune](/mem/intune/enrollment/windows-enrollment-methods) [a](secure-win-10-pcs.md) vaše organizace má zaregistrovaná 800 nebo méně zařízení, uvidíte detekce  a přehledy hrozeb v <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Centrum pro správu Microsoftu 365</a> na stránce Hrozby & antivirus, ke kterým se můžete dostat z karty **Antivirová ochrana v programu Microsoft Defender** na domovské stránce (nebo z navigačního podokna tak, že vyberete Antivirová ochrana proti hrozbám &   >  stavu).

    Pokud má vaše organizace v Intune zaregistrovaných víc než 800 zařízení, zobrazí se výzva k zobrazení zjišťování hrozeb a přehledů z [Microsoft Endpoint Manager](/mem/endpoint-manager-overview) místo ze stránky Hrozby a **antivirová** ochrana.
 
    > [!NOTE]
    > Stránka **Antivirová ochrana v programu Microsoft Defender** a **hrozby** a antivirové programy se postupně vysílují, takže k nim možná nemáte okamžitý přístup.

Ve většině případů uživatelé nemusí nic dalšího udělat. Jakmile na zařízení zjistíte škodlivý soubor nebo program, Antivirová ochrana v programu Microsoft Defender zablokuje a zabrání jeho spuštění. Nově zjištěné hrozby se navíc přidávají do antivirového a antimalwarového modulu, aby byla chráněna i další zařízení a uživatelé.  

Pokud uživatel potřebuje provést akci, třeba schválení odebrání škodlivého souboru, uvidí to v oznámení, které obdrží. Další informace o akcích, které Antivirová ochrana v programu Microsoft Defender za uživatele, nebo akce, které uživatelé potřebují udělat, najdete v tématu [Historie ochrany](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708). Pokud se chcete dozvědět, jak spravovat zjišťování hrozeb jako odborník/správce IT, přečtěte si informace v tématu Kontrola zjištěných hrozeb [a akce.](review-threats-take-action.md)

Další informace o různých hrozbách najdete na webu <a href="https://www.microsoft.com/wdsi/threats" target="_blank">Microsoft Bezpečnostní analýza Hrozby,</a>kde můžete provádět následující akce: 

- Zobrazení aktuálních informací o nejvyšších hrozbách
- Podívejte se na nejnovější hrozby pro konkrétní oblast.
- Podrobnosti o konkrétní hrozbě najdete v encyklopedii hrozeb.

## <a name="related-content"></a>Související obsah

[Zabezpečená Windows 10 zařízení](secure-windows-10-devices.md) (článek)\
[Vyhodnocení Antivirová ochrana v programu Microsoft Defender](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (článek)\
[Jak zapnout antivirovou ochranu v reálném čase](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) a cloudovou ochranu (článek)\
[Jak zapnout a používat Antivirová ochrana v programu Microsoft Defender v aplikaci Zabezpečení Windows](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) (článek)\
[Jak zapnout Antivirová ochrana v programu Microsoft Defender pomocí Zásady skupiny](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (článek)\
[Jak aktualizovat definice antivirové ochrany](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (článek)\
[Odeslání malwaru a nemalwaru do Microsoftu k analýze](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (článek)
