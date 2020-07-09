---
title: Migrace z Microsoftu 365 Business do Microsoftu 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Přečtěte si, jak přesunout svou firmu z Microsoft 365 Business Premium do Microsoftu 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081795"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrace z Microsoftu 365 Business Premium do Microsoftu 365 E3

Microsoft 365 Business Premium má vše, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace ve své třídě s jednoduchou správou zařízení a zabezpečením, které vašim zaměstnancům umožní odváděli nejlepší práci. V některých případech však může být nutné migrovat předplatné Microsoft 365 Business Premium do Microsoft 365 E3. 

Vaše firma se například rozrostla a potřebuje více než 300 licencí (mimochodem blahopřejeme).

Nebo vaše firma potřebuje podnikové funkce, jako jsou aplikace Microsoft 365 pro podniky, Windows 10 Enterprise E3 nebo licence enterprise client access (CAL).

Upgrade je snadný: upgrade můžete spustit [z Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md). Všechna vaše data a konfigurace v aktuálním předplatném jsou zachována. Není nic, co byste měli udělat, abyste se připravili na migraci, a nic dělat později, kromě využití nových funkcí.

>[!Note]
>Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí. Však Office 365 ATP není součástí Microsoft 365 E3. Chcete-li pokračovat v ochraně před hrozbami, měli byste přidat další licence office 365 ATP, aby měli licenci všichni uživatelé v rozsahu vašich policistů ochrany ATP Office 365.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Rozdíly mezi Microsoftem 365 Business Premium a Microsoft 365 Enterprise

Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkce    | Podpora v Microsoftu 365 Business Premium    | Podpora v Microsoftu 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikace Office*    | [Aplikace Microsoft 365 pro firmy](#office-365-business)    | Aplikace Microsoft 365 pro podniky | 
| **Cloudové aplikace pro zvýšení produktivity**        | | | 
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezená archivace Exchange Online    | Limit úložiště 100 GB na poštovní schránku a neomezená archivace Exchange Online | 
| Týmy    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezené | 
| Yammer, SharePoint Online, Plánovač, Stream    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbami**        | | | 
| Možnosti redukce povrchu útoku    | [Podívejte se na tento seznam](#threat-protection) | Podniková správa hardwarové izolace pro Microsoft Edge | 
| Plán 1 pokročilé ochrany před hrozbami Office 365 | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno na | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure (MFA), podmíněný přístup, zpětný zápis hesel pro místní identity|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Zjišťování cloudových aplikací, azure ad connect stav    |     | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Jednotné přihlašení aplikací Azure AD Office 365 (jednotné přihlašení): 10 aplikací na uživatele (aplikace Galerie SaaS, jako je Salesforce)* | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: bez omezení (místní aplikace prostřednictvím azure ad application proxy a non-galerie aplikace pomocí samoobslužné šablony integrace aplikací)    |     | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| **Správa zařízení a aplikací**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|Přístup k virtuální ploše (VDA)    |  |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|Virtuální plocha systému Windows (WVD)    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
|Aktivace sdíleného počítače (SCA)    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Balíček optimalizace pro stolní počítače společnosti Microsoft    | |     ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrana informací**        | | | 
| Office 365 Ochrana před ztrátou dat, Plán ochrany informací Azure 1    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Ochrana informací o okně pro dlp koncového bodu    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| **Licence klientského přístupu (práva CAL)**    | | |     
| Sada Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Správa práv systému Windows)| |         ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| **Dodržování**        | | | 
| Neomezená archivace e-mailů    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Skóre dodržování předpisů/Správce dodržování předpisů    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Ediscovery    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Blokování na místě a blokování ze soudních sporů    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
| Retenční značky a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM) a zásady uchovávání informací    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí balení je Microsoft 365 E3](../media/check-mark.png) | 
||||

\*Uživatelé, kterým byl přiřazen přístup k aplikacím SaaS, mohou získat přístup k návěsům až pro 10 aplikací. Správci můžou konfigurovat jednosadové služby a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednoodvolům je povolen jenom pro 10 aplikací na uživatele najednou. Všechny aplikace Office 365 se počítají jako jedna aplikace.

## <a name="migration"></a>Migrace

Chcete-li migrovat, spolupracujte se svým partnerem na přesunutí předplatného a licencí Microsoft 365 Business Premium do vhodného předplatného Microsoft 365 E3 s jeho licencemi.

Následující části popisují, jaké změny je třeba provést, pokud existuje, a co můžete udělat po migraci.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurace předplatného Microsoftu 365 a data

Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, což zahrnuje:

- Konfigurace předplatného, například názvy domén DNS.
- Uživatelské a skupinové účty a nastavení ověřování, jako je například vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.

Vaši uživatelé teď můžou využívat neomezené úložiště v poštovních schránkách Exchange Online a ve složkách OneDrivu pro firmy.

Můžete začít používat Cloud App Discovery, Azure AD Connect Health a SSO pro více než 10 aplikací.

>[!Note]
>Uživatelé migrovaní na Microsoft 365 E3 již nemohou používat Správce zákazníků aplikace Outlook a MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrana před hrozbami

Windows 10 Business zahrnuje tyto ochrany:

- Vynucení integrity procesu spouštění operačního systému
- Prosazování integrity citlivých provozních součástí
- Pokročilá chyba zabezpečení a skutečnosti snižující závažnost rizika zneužití nultého dne
- Ochrana sítě založená na reputaci pro Microsoft Edge, Internet Explorer a Chrome
- Brána firewall založená na hostiteli
- Skutečnosti snižující závažnost rizika ransomwaru
- Hardwarová izolace pro Microsoft Edge
- Řízení aplikací poháněné grafem inteligentního zabezpečení
- Ovládání zařízení (USB)
- Ochrana sítě před webovými hrozbami
- Pravidla prevence narušení hostitele

Windows 10 Enterprise E3 také zahrnuje podnikovou správu hardwarové izolace pro Microsoft Edge.

>[!Note]
>Uživatelé migrované na Microsoft 365 E3 budou potřebovat licenci Office 365 ATP pro trvalou ochranu před hrozbami. Nezapomeňte zakoupit další licence Office 365 ATP, aby všichni uživatelé v rozsahu vašich policistů office 365 ATP získali licenci. 
>

### <a name="device-management-with-intune"></a>Správa zařízení s Intune

Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium obsahuje Windows 10 Business, který můžete nainstalovat pomocí Windows AutoPilot. Při migraci na Microsoft 365 E3 obsahuje každá uživatelská licence Windows 10 Enterprise E3, který můžete nainstalovat také pomocí programu Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikace Microsoft 365 pro firmy

Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních začne automaticky používat funkce Aplikací Microsoft 365 pro podniky. Po migraci můžete nyní použít:

 - Aktivace svazku prostřednictvím zásad skupiny
 - Telemetrie aplikací
 - Aktualizovat ovládací prvky
 - Porovnání a dotazování v tabulkovém procesoru
 - Business intelligence

