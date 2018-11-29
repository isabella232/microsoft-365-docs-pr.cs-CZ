---
title: Převod odběru Microsoft 365 obchodní zprostředkovatel kryptografických služeb 
description: Zjistěte, jak můžete přechod předplatné Microsoft 365 Business CSP z náhledu JM. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: 365 Business společnosti Microsoft, Microsoft 365, SMB, převod odběru CSP
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982481"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Převod odběru Microsoft 365 obchodní zprostředkovatel kryptografických služeb

Pokud máte předplatné Microsoft 365 obchodní náhled zprostředkovatele kryptografických služeb, postupujte podle této příručky a zjistěte, jak můžete převod stávající předplatné náhled Microsoft 365 Business GA (všeobecné dostupnosti).

**Postup při přechodu náhled předplatné GA**

1. Přihlášení do <a href="https://partnercenter.microsoft.com" target="_blank">Partnerské centrum</a>.
2. Z řídicího panelu vyberte **Zákazníci**a vyhledejte a vyberte název společnosti.

    Zobrazí seznam předplatných pro společnost.

    ![Předplatné zákazníka v partnerské Centrum](images/pc_customer_subscriptions_1.png)
    
3. Na stránce **předplatného** společnosti vyberte **Přidat předplatné**.
4. Na stránce **Nový odběr** vyberte **Small business** a ze seznamu vyberte **Microsoft 365 Business** .
5. Přidat počet licencí a potom vyberte **Další: Kontrola** ke kontrole předplatného a pak vyberte **Odeslat**.

    ![Recenze nové předplatné Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Na základě licence předplatného** se zobrazí **Náhled obchodní 365 Microsoft** a **Microsoft 365 Business**. Budete potřebovat pozastavit další předplatné náhled.

6. Vyberte **Náhled 365 obchodní společnosti Microsoft**.
7. Na stránce **Microsoft 365 obchodní náhled** vyberte **Suspended** pozastavení odběru náhled.

    ![Pozastavení předplatného Microsoft 365 obchodní náhled](images/pc_customer_m365bpreview_suspend.png)

8. Vyberte možnost **Odeslat** k potvrzení.

    Na stránce **Odběry** potvrďte, že je **Microsoft 365 obchodní náhled** ve stavu **Suspended**.

    ![Ověřte, zda že stav předplatného náhled je pozastaveno.](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Volitelně je možné ověřit licenční smlouvy. Chcete-li to provést, postupujte takto:
    1. Vyberte **uživatele a licence** od společnosti **Odběry** stránka.
    2. Na stránce **Uživatelé a licencí** vyberte uživatele.
    3. Uživatele stránky zaškrtněte v části **přiřazení licencí** a potvrďte ukazuje **Microsoft 365 Business**.

        ![Ověřte, zda že je uživateli přidělena licence Microsoft 365 Business](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Dopad na zákazníky a uživatele během a po přechodu

Neexistuje žádný dopad na zákazníky a uživatele během přechodu a hraniční přechod.

## <a name="impact-to-customers-who-dont-transition"></a>Dopad na zákazníky, kteří nemají přechod

Následující tabulka shrnuje vliv na zákazníky, kteří nejsou z předplatného Microsoft 365 obchodní náhled přechod do Microsoft 365 Business předplatné.

|       | T-0 T + 30     | T + 30 T + 60 | T + 60 T + 120 | Za T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Stav** | V období odkladu | Platnost vypršela      | Zakázáno      | Deprovisioned |
| **Dopady na služby**                                                        |
| **Portál pro správce Microsoft 365 Business** | Žádný vliv na funkčnost | Žádný vliv na funkčnost | Přidání a odstranění uživatelů, můžete zakoupit předplatné.</br> Nelze přiřadit nebo odebrat licence. | Předplatné zákazníka a všechna data se odstraní. Správce může spravovat jiné placené předplatné. |
| **Aplikace sady Office**                         | Žádný dopad na koncového uživatele | Žádný dopad na koncového uživatele | Office přejde do režimu se sníženou funkčností.</br> Uživatelé mohou zobrazit pouze soubory. | Office přejde do režimu se sníženou funkčností.</br> Uživatelé mohou zobrazit pouze soubory. |
| **Cloud services (služby SharePoint Online, Exchange Online, Skype, týmy a další)** | Žádný dopad na koncového uživatele | Žádný dopad na koncového uživatele | Koncoví uživatelé a Administrátoři nemají přístup k datům v cloudu. | Předplatné zákazníka a všechna data budou odstraněny. |
| **EM + S komponenty** | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Funkce přestane být vynucena.</br> Další informace naleznete v tématu [vliv mobilního zařízení po vypršení předplatného](#mobile-device-impacts-upon-subscription-expiration) a [dopady na Windows 10 PC po vypršení předplatného](#windows-10-pc-impacts-upon-subscription-expiration) . | Funkce přestane být vynucena.</br> Další informace naleznete v tématu [vliv mobilního zařízení po vypršení předplatného](#mobile-device-impacts-upon-subscription-expiration) a [dopady na Windows 10 PC po vypršení předplatného](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Windows 10 obchodní** | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Funkce přestane být vynucena.</br> Další informace naleznete v tématu [vliv mobilního zařízení po vypršení předplatného](#mobile-device-impacts-upon-subscription-expiration) a [dopady na Windows 10 PC po vypršení předplatného](#windows-10-pc-impacts-upon-subscription-expiration) . | Funkce přestane být vynucena.</br> Další informace naleznete v tématu [vliv mobilního zařízení po vypršení předplatného](#mobile-device-impacts-upon-subscription-expiration) a [dopady na Windows 10 PC po vypršení předplatného](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Azure AD přihlášení k Windows 10 PC** | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Žádný dopad na admin</br> Žádný dopad na koncového uživatele | Po odstranění nájemce se uživatel může přihlásit pomocí pouze místní pověření. Zařízení obrázek znovu, pokud neexistují žádné místní pověření. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Dopady na mobilním zařízení po vypršení předplatného

Followint tabulka shrnuje vliv na zásady správy aplikací v mobilních zařízeních.

|                            | Plně licencované zkušenosti                      | Vypršení platnosti T + 60 dnů post          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Odstranit pracovní soubory z neaktivní zařízení** | Pracovní soubory odstraněny po vybrané dny | Pracovní soubory zůstávají na uživatele osobních zařízení. |
| **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** | Pracovní soubory lze uložit pouze na OneDrive pro firmy | Pracovní soubory mohou být uloženy kdekoliv |
| **Šifrovat pracovní soubory** | Pracovní soubory jsou zašifrovány. | Pracovní soubory již nejsou zašifrované.</br> Zásady zabezpečení jsou odebrány a data aplikací sady Office bude odebrán. |
| **Požadovat kód PIN nebo otisků pro přístup k aplikacím sady Office** | Omezený přístup k aplikacím | Žádná omezení přístupu na úrovni aplikace |
| **Při přihlášení se nezdaří obnovit kód PIN** | Omezený přístup k aplikacím | Žádná omezení přístupu na úrovni aplikace |
| **Požadovat, aby uživatelé přihlásit znovu po nečinnosti aplikace sady Office** | Vyžadováno přihlášení | Žádné povinné přihlášení pro přístup k aplikacím |
| **Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem** | Pracovní soubory nelze získat přístup na jailbroken/zakořeněné zařízení | Pracovní soubory jsou přístupné na jailbroken/zakořeněné zařízení |
| **Povolit uživatelům kopírovat obsah z aplikací sady Office do osobní apps** | Kopírování a vkládání omezeno na aplikace, které jsou k dispozici v rámci předplatného Microsoft 365 Business | Kopírování a vkládání k dispozici pro všechny aplikace |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Dopady na Windows 10 PC po vypršení předplatného

Následující tabulka shrnuje vliv zásad konfigurace Windows 10 zařízení.

|                            | Plně licencované zkušenosti                      | Vypršení platnosti T + 60 dnů post          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Ochranu počítače před hrozbami pomocí programu Windows Defender** | Zapnutí/vypnutí je vně uživatelského ovládacího prvku | Uživatel může zapnout nebo vypnout program Windows Defender v systému Windows 10 PC |
| **Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge** | Ochrana počítače v aplikaci Microsoft Edge | Uživatel může zapnout nebo vypnout ochranu počítače v aplikaci Microsoft Edge |
| **Vypněte zařízení obrazovky při nečinnosti** | Správce definuje zásady interval časového limitu obrazovky | Časový limit obrazovky lze nakonfigurovat tak, že koncový uživatel |
| **Povolit uživatelům stahovat aplikace z webu Microsoft Store** | Správce určuje, zda uživatel stáhnout z Microsoft Store apps | Uživatel stáhnout aplikace z Microsoft Store kdykoli |
| **Umožnit uživatelům přístup ke Cortaně** | Správce definuje zásady přístupu uživatele k Cortana | Zařízení uživatele Chcete-li zapnout či vypnout Cortana |
| **Povolit uživatelům získat tipy a reklamy od společnosti Microsoft** | Správce definuje zásady uživatele získat tipy a reklamy od společnosti Microsoft | Uživatel může zapnout nebo vypnout tipy a reklamy od společnosti Microsoft |
| **Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací** | Správce definuje zásady aktualizovat Windows 10 zařízení | Uživatelé se mohou rozhodnout při aktualizaci systému Windows |




