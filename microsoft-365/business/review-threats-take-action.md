---
title: Kontrola zjištěných hrozeb a akce
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Zjistěte, jak zkontrolovat a spravovat hrozby zjištěné Antivirová ochrana v programu Microsoft Defender na Windows 10 zařízeních.
ms.openlocfilehash: 15e99fb75e4a3ac1af842ca7d0b900e02cbc6bd4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "53465399"
---
# <a name="review-detected-threats-and-take-action"></a>Kontrola zjištěných hrozeb a akce

Jakmile zjistíte škodlivý soubor nebo software, Antivirová ochrana v programu Microsoft Defender zablokuje a zabrání jeho spuštění. A když je zapnutá cloudová ochrana, nově zjištěné hrozby se přidávají do antivirového a antimalwarového modulu, aby byla chráněna i vaše další zařízení a uživatelé.

Antivirová ochrana v programu Microsoft Defender rozpozná a chrání před následujícími typy hrozeb:

- Viry, malware a webové hrozby na zařízeních
- Pokusy o útok phishing
- Pokusy o odcizení dat

Jako it profesionál/správce můžete zobrazit informace o zjišťování hrozeb na Windows 10 zařízeních, která jsou zaregistrovaná v [Intune](/mem/intune/enrollment/device-enrollment) v Centrum pro správu Microsoftu 365. Zobrazí se souhrnné informace, například:

- Kolik zařízení potřebuje antivirovou ochranu
- Kolik zařízení není v souladu se zásadami zabezpečení
- Kolik hrozeb je aktuálně aktivních, zmírněných nebo vyřešených

Máte několik možností, jak zobrazit konkrétní informace o detekcích hrozeb a zařízeních:

- Stránka **Aktivní zařízení** v <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Centrum pro správu Microsoftu 365</a>. Podívejte [se na článek Správa zjišťování hrozeb na stránce Aktivní](#manage-threat-detections-on-the-active-devices-page) zařízení v tomto článku.
- Stránka **Aktivní** hrozby v <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Centrum pro správu Microsoftu 365</a>. Podívejte [se na článek Správa zjišťování hrozeb na stránce Aktivní hrozby](#manage-threat-detections-on-the-active-threats-page) v tomto článku.
- Stránka **Antivirus** v <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Microsoft Endpoint Manager</a>. Podívejte se na článek Správa zjišťování [hrozeb Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) v tomto článku.

Další informace najdete v tématu [Hrozby zjištěné Antivirová ochrana v programu Microsoft Defender](threats-detected-defender-av.md).

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Správa zjišťování hrozeb na **stránce Aktivní** zařízení

Následující postup platí pro zákazníky, kteří Microsoft 365 Business Premium.

1. Přejděte na Centrum pro správu Microsoftu 365 a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> přihlaste se.

2. Na navigační stránce vyberte **Zařízení**  >  **Aktivní zařízení**. Zobrazí se seznam aktivních zařízení a podrobností, jako je stav ochrany, stav antivirové ochrany (AV) a počet zjištěných aktivních hrozeb.

3. Výběrem zařízení zobrazíte další podrobnosti o tomto zařízení a dostupných akcích. Otevře se plovoucí panel s doporučeními a dostupnými akcemi, jako jsou třeba Zásady aktualizace **,** Aktualizace antivirového **softwaru,** Spustit rychlou **kontrolu,** Spustit **úplnou** kontrolu a další.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Správa zjišťování hrozeb na **stránce Aktivní hrozby**

Následující postup platí pro zákazníky, kteří Microsoft 365 Business Premium. [Windows 10 musí být zabezpečená a](./secure-win-10-pcs.md) [zaregistrovaná v Intune](/mem/intune/enrollment/windows-enrollment-methods).

> [!NOTE]
> Stránka **Antivirová ochrana v programu Microsoft Defender** karty a  aktivních hrozeb se zakřížuje ve fázích, takže k nim možná nemáte okamžitý přístup.

1. Přejděte na Centrum pro správu Microsoftu 365 a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> přihlaste se.

2. Na kartě **Antivirová ochrana v programu Microsoft Defender** vyberte **Zobrazit aktivní hrozby**. (Případně v navigačním podokně vyberte **Stav.**  >  **Hrozby & antivirovou** ochranu .)

3. Na stránce **Aktivní** hrozby vyberte zjištěnou hrozbu, abyste se o ní dozvěděli víc. Otevře se plovoucí okno s podrobnostmi o této hrozbě, včetně zařízení, která jsou ovlivněná.

4. V plovoucím panelu vyberte zařízení, které zobrazí dostupné akce, jako jsou třeba Zásady aktualizace **,** Aktualizace antivirového **softwaru,** Spustit **rychlou** kontrolu a další.

## <a name="actions-you-can-take"></a>Akce, které můžete udělat

Když si zobrazíte podrobnosti o konkrétních hrozbách nebo zařízeních, zobrazí se vám doporučení a jedna nebo více akcí, které můžete udělat. Následující tabulka popisuje akce, které se můžou zobrazit.<br><br>

| Akce | Popis |
|--|--|
| Konfigurace ochrany | Vaše zásady ochrany před hrozbou je potřeba nakonfigurovat. Výběrem odkazu přejděte na stránku konfigurace zásad.<br><br>Potřebujete pomoct? Viz [Správa zabezpečení zařízení pomocí zásad zabezpečení koncových bodů v Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Zásady aktualizace | Vaše antivirová ochrana a zásady ochrany v reálném čase je potřeba aktualizovat nebo nakonfigurovat. Výběrem odkazu přejděte na stránku konfigurace zásad.<br><br>Potřebujete pomoct? Viz [Správa zabezpečení zařízení pomocí zásad zabezpečení koncových bodů v Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Spustit rychlou kontrolu | Spustí na zařízení rychlou antivirovou kontrolu a zaměří se na běžná místa, kde může být malware registrovaný, například klíče registru a známé Windows spouštěcí složky. |
| Spustit úplnou kontrolu | Spustí na zařízení úplnou antivirovou kontrolu, která se zaměří na společná umístění, kde může být malware registrovaný, a včetně všech souborů a složek na zařízení. Výsledky se posílají do [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Aktualizace antivirového softwaru | Vyžaduje, aby zařízení dostávat [aktualizace bezpečnostních informací pro](https://go.microsoft.com/fwlink/?linkid=2149926) antivirovou a antimalwarovou ochranu. |
| Restartování zařízení | Vynutí restartování Windows 10 zařízení během pěti minut.<br><br>**DŮLEŽITÉ:** Vlastník nebo uživatel zařízení není automaticky upozorněn na restartování a může přijít o neuloženou práci. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Správa zjišťování hrozeb v Microsoft Endpoint Manager

Pomocí funkce Microsoft Endpoint Manager ke správě zjišťování hrozeb. Windows 10 musí být [zaregistrovaná v Intune](/mem/intune/enrollment/windows-enrollment-methods) (součást Microsoft Endpoint Manager).

1. Přejděte do centra Microsoft Endpoint Manager správce a <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> přihlaste se.

2. V navigačním podokně vyberte Zabezpečení **koncového bodu**.

3. V **části Manage**(Spravovat) vyberte Antivirus **(Antivirová ochrana).** Zobrazí se několik karet, například Souhrn **,** **Windows 10** chybně v pořádku a **Windows 10 malware**.

4. Zkontrolujte informace na dostupných kartách a pak udělejte všechny potřebné akce.

Předpokládejme například, že zařízení jsou uvedená na **kartě Windows 10 malware.** Když vyberete zařízení, budete mít k dispozici určité akce, jako je **restartování,** rychlá **kontrola,** úplná **kontrola,** **synchronizace** nebo **aktualizace podpisů.** Vyberte akci pro toto zařízení.

Následující tabulka popisuje akce, které se můžou zobrazit v Microsoft Endpoint Manager.<br><br>

| Akce | Popis |
|--|--|
| Restartovat | Vynutí restartování Windows 10 zařízení během pěti minut.<br><br>**DŮLEŽITÉ:** Vlastník nebo uživatel zařízení není automaticky upozorněn na restartování a může přijít o neuloženou práci. |
| Rychlá kontrola | Spustí na zařízení rychlou antivirovou kontrolu a zaměří se na běžná místa, kde může být malware registrovaný, například klíče registru a známé Windows spouštěcí složky. Výsledky se posílají do [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Úplná kontrola | Spustí na zařízení úplnou antivirovou kontrolu, která se zaměří na společná umístění, kde může být malware registrovaný, a včetně všech souborů a složek na zařízení. Výsledky se posílají do [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Synchronizace | Vyžaduje zařízení pro přihlášení pomocí Intune (součást Microsoft Endpoint Manager). Když se zařízení nasouvá, přijme zařízení všechny čekající akce nebo zásady přiřazené k zařízení. |
| Aktualizace podpisů | Vyžaduje, aby zařízení dostávat [aktualizace bezpečnostních informací pro](https://go.microsoft.com/fwlink/?linkid=2149926) antivirovou a antimalwarovou ochranu. |

> [!TIP]
> Další informace najdete v tématu [Vzdálené akce pro zařízení](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices).

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Jak odeslat soubor pro analýzu malwaru

Pokud máte soubor, o který si myslíte, že byl zmeškaný nebo nesprávně klasifikovaný jako malware, můžete tento soubor odeslat microsoftu pro analýzu malwaru. Uživatelé a správci IT mohou odeslat soubor k analýze. Navštivte [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) stránku .