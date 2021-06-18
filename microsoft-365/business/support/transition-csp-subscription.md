---
title: Přechod předplatného csP Microsoft 365 Business
description: Zjistěte, jak můžete předplatné csP Microsoft 365 Business přejít z verze Preview na obecnou dostupnost (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasongroce
ms.topic: article
manager: jasonh
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business
keywords: Microsoft 365 Firemní, Microsoft 365, SMB, přechodové předplatné CSP
ms.date: 11/01/2017
ms.openlocfilehash: 3f6c71edb50cc3c5509e61a83efb64185c10648d
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924997"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Přechod předplatného csP Microsoft 365 Business

Pokud máte předplatné Microsoft 365 Business Preview CSP, postupujte podle tohoto průvodce a zjistěte, jak můžete stávající předplatné Preview přejít na ga Microsoft 365 Business (obecná dostupnost).

**Přechod předplatného preview na GA**

1. Přihlaste se do <a href="https://partnercenter.microsoft.com" target="_blank">Partnerského centra</a>.
2. Na řídicím panelu vyberte **Zákazníci** a pak najděte a vyberte název společnosti.

    Budou uvedená předplatná pro společnost.

    ![Předplatná zákazníků v Partnerském centru](../../media/pc_customer_subscriptions_1.png)
    
3. Na stránce **Předplatná společnosti** vyberte **Přidat předplatné**.
4. Na stránce **Nové předplatné** vyberte **Malá** firma a v seznamu **Microsoft 365 Business.**
5. Přidejte počet licencí a pak vyberte **Další: Zkontrolovat,** zkontrolujte předplatné a pak vyberte **Odeslat.**

    ![Kontrola nového předplatného Microsoft 365 Business](../../media/pc_customer_reviewnewsubscription.png)

    **Předplatná založená na licencích** se zobrazí **Microsoft 365 Business Preview** a Microsoft 365 **Business**. Předplatné Preview budete dál pozastavit.

6. Vyberte **Microsoft 365 Business Preview**.
7. Na stránce **Microsoft 365 Náhled** firmy vyberte **Pozastaveno** a předplatné Preview pozastavíte.

    ![Pozastavení předplatného Microsoft 365 Business Preview](../../media/pc_customer_m365bpreview_suspend.png)

8. Potvrďte **výběrem** možnosti Odeslat.

    Na stránce **Předplatná** potvrďte, že se **ve Microsoft 365 Business Preview** zobrazuje stav **Pozastaveno**.

    ![Potvrzení, že je stav předplatného Preview pozastavený](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Volitelně můžete také ověřit licenční smlouvu. Postupujte takto:
    1. Na **stránce Předplatná** společnosti vyberte Uživatelé **a** licence.
    2. Na **stránce Uživatelé** a licence vyberte uživatele.
    3. Na stránce uživatele zkontrolujte oddíl  Přiřadit licence a ověřte, že se zobrazuje Microsoft 365 **Business**.

        ![Potvrďte Microsoft 365 že je uživateli přiřazená licence Pro firmy](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Dopad na zákazníky a uživatele během přechodu a po přechodu

Při přechodu a po přechodu na tento přechod nemá zákazník ani uživatelé žádný vliv.

## <a name="impact-to-customers-who-dont-transition"></a>Dopad na zákazníky, kteří přechod neschová

Následující tabulka shrnuje dopad na zákazníky, kteří přechádují z předplatného Microsoft 365 Business Preview na předplatné Microsoft 365 Business.

|       | T-0 až T+30     | T+30 až T+60 | T+60 až T+120 | Mimo T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stav** | V období odkladu | Vypršela platnost      | Zakázáno      | Deprovisioned |
| **Dopad na službu**                                                        |
| **Microsoft 365 Portál pro správu firmy** | Bez dopadu na funkčnost | Bez dopadu na funkčnost | Může přidávat nebo odstraňovat uživatele, kupovat předplatná.</br> Licence nelze přiřadit nebo odvolat. | Předplatné zákazníka a všechna data se odstraní. Správce může spravovat další placená předplatná. |
| **Office aplikace**                         | Žádný dopad na koncového uživatele | Žádný dopad na koncového uživatele | Office do režimu omezené funkčnosti.</br> Uživatelé mohou prohlížet jenom soubory. | Office do režimu omezené funkčnosti.</br> Uživatelé mohou prohlížet jenom soubory. |
| **Cloudové služby (SharePoint Online, Exchange Online, Skype, Teams a další)** | Žádný dopad na koncového uživatele | Žádný dopad na koncového uživatele | Koncoví uživatelé a správci nemají přístup k datům v cloudu. | Předplatné zákazníka a všechna data se odstraní. |
| **Součásti EM+S** | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Funkce už není vynucovaná.</br> Další [informace najdete v](#mobile-device-impacts-upon-subscription-expiration) článku Dopad na mobilní zařízení po vypršení [platnosti předplatného a Windows 10 dopad](#windows-10-pc-impacts-upon-subscription-expiration) na počítač po vypršení platnosti předplatného. | Funkce už není vynucovaná.</br> Další [informace najdete v](#mobile-device-impacts-upon-subscription-expiration) článku Dopad na mobilní zařízení po vypršení [platnosti předplatného a Windows 10 dopad](#windows-10-pc-impacts-upon-subscription-expiration) na počítač po vypršení platnosti předplatného. |
| **Windows 10 Business** | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Funkce už není vynucovaná.</br> Další [informace najdete v](#mobile-device-impacts-upon-subscription-expiration) článku Dopad na mobilní zařízení po vypršení [platnosti předplatného a Windows 10 dopad](#windows-10-pc-impacts-upon-subscription-expiration) na počítač po vypršení platnosti předplatného. | Funkce už není vynucovaná.</br> Další [informace najdete v](#mobile-device-impacts-upon-subscription-expiration) článku Dopad na mobilní zařízení po vypršení [platnosti předplatného a Windows 10 dopad](#windows-10-pc-impacts-upon-subscription-expiration) na počítač po vypršení platnosti předplatného. |
| **Přihlášení azure AD k Windows 10 počítači** | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Žádný dopad na správce</br> Žádný dopad na koncového uživatele | Po odstranění tenanta se může uživatel přihlásit jenom pomocí místních přihlašovacích údajů. Pokud nejsou k dispozici místní přihlašovací údaje, zařízení znovu vybitové kopie. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Vliv mobilního zařízení na vypršení platnosti předplatného

Následující tabulka shrnuje dopad na zásady správy aplikací na mobilních zařízeních.

|                            | Plně licencované prostředí                      | T+60 dnů po vypršení platnosti          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Odstranění pracovních souborů z neaktivního zařízení** | Pracovní soubory se po vybraných dnech odebrané | Pracovní soubory zůstávají na osobních zařízeních uživatele. |
| **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** | Pracovní soubory je možné uložit jenom do OneDrive pro firmy | Pracovní soubory se ukládají kdekoli |
| **Šifrovat pracovní soubory** | Pracovní soubory jsou zašifrované | Pracovní soubory už nejsou šifrované.</br> Zásady zabezpečení se odebraly a odebraly se data Office v aplikacích. |
| **Vyžadování PIN kódu nebo otisku prstu pro přístup k aplikacím Office** | Omezený přístup k aplikacím | Žádné omezení přístupu na úrovni aplikace |
| **Resetování KÓDU PIN při neúspěšné přihlášení** | Omezený přístup k aplikacím | Žádné omezení přístupu na úrovni aplikace |
| **Vyžadovat, aby se uživatelé znovu přihlašoval po nečinnosti aplikací Office** | Vyžaduje se přihlášení. | Nevyžaduje se žádné přihlášení. |
| **Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem** | K pracovním souborům není možné přistupovat na zařízeních s jailbrokenem nebo rootem. | K pracovním souborům se dostanete na zařízeních s jailbrokenem nebo rootem. |
| **Povolení uživatelům kopírovat obsah z aplikací Office do osobních aplikací** | Kopírování a vkládání omezeno na aplikace dostupné v rámci předplatného Microsoft 365 | Kopírování a vkládání dostupných pro všechny aplikace |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Dopad na počítač s Windows 10 po vypršení platnosti předplatného

Následující tabulka shrnuje dopad na zásady konfigurace zařízení s Windows 10.

|                            | Plně licencované prostředí                      | T+60 dnů po vypršení platnosti          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ochrana počítačů před hrozbami pomocí programu Windows Defender** | Zapnutí nebo vypnutí je mimo uživatelský ovládací prvek | Uživatel může na počítači s Windows 10 zapnout nebo vypnout Windows Defender. |
| **Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge** | Ochrana počítače v Microsoft Edge | Uživatel může zapnout nebo vypnout ochranu počítače v Microsoft Edge |
| **Vypnutí obrazovky zařízení při nečinnosti** | Správce definuje zásadu intervalu časového limitu obrazovky. | Časový limit obrazovky může nakonfigurovat koncový uživatel. |
| **Povolit uživatelům stahovat aplikace z webu Microsoft Store** | Správce definuje, jestli si uživatel může stahovat aplikace z Microsoft Storu. | Uživatel si může kdykoli stáhnout aplikace z Microsoft Storu. |
| **Umožnit uživatelům přístup ke Cortaně** | Správce definuje zásady přístupu uživatelů k Cortaně. | Uživatelská zařízení pro zapnutí/vypnutí Cortany |
| **Povolení uživatelům přijímat tipy a reklamy od Microsoftu** | Správce definuje zásady pro přijímání tipů a reklam pro uživatele od Microsoftu. | Uživatel může zapnout nebo vypnout tipy a reklamy od Microsoftu |
| **Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací** | Správce definuje zásady, které udržují zařízení s Windows 10 aktuální | Uživatelé se mohou rozhodnout, kdy windows aktualizovat |
