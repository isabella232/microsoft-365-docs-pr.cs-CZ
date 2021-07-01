---
title: Migrace z Microsoft 365 Business na Microsoft 365 E3
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
description: Zjistěte, jak přesunout svou firmu z Microsoft 365 Business Premium do Microsoft 365 E3.
ms.openlocfilehash: 6502d79dbb283db37b00e4fccf89b15ab4291ce5
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227613"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrace z Microsoft 365 Business Premium na Microsoft 365 E3

Microsoft 365 Business Premium má všechno, co potřebujete pro svoji malou firmu, a kombinuje nejlepší cloudové aplikace na bázi produktivity ve své třídě s jednoduchou snadná správa zařízení a zabezpečení, které vašim zaměstnancům umožňují dělat svou nejlepší práci. V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium do Microsoft 365 E3.

Vaše firma například roste a potřebuje víc než 300 licencí (mimochodem blahopřejeme).

Nebo vaše firma potřebuje podnikové funkce, jako jsou Microsoft 365 Apps pro velké organizace, Windows 10 Enterprise E3 nebo Enterprise klientského přístupu (CAL).

Upgrade je snadný: Upgrade můžete spustit z [Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md). Všechna vaše data a konfigurace v aktuálním předplatném se zachová. Není nic, co byste měli udělat, abyste se připravili na migraci a potom nic dělat, kromě využití nových funkcí.

> [!NOTE]
> Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí. Program Microsoft Defender pro Office 365 ale není součástí Microsoft 365 E3. Pokud chcete pokračovat v ochraně před hrozbami, měli byste přidat další defender pro Office 365, aby všichni uživatelé v rozsahu vašeho Defenderu pro Office 365 měli licenci.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise

Tato tabulka zobrazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Microsoft 365 E3 |
|:-------|:-----|:-----|
| **Místní**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office aplikace*    | [Microsoft 365 Apps pro firmy](#office-365-business)    | Aplikace Microsoft 365 pro podniky |
| **Cloudové aplikace pro zvýšení produktivity**        | | |
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezená Exchange Online archivace    | Limit úložiště 100 GB na poštovní schránku a neomezená Exchange Online archivace |
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezená |
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| **Ochrana před hrozbou**        | | |
| Možnosti omezení útoku na povrch    | [Zobrazit tento seznam](#threat-protection) | Enterprise správy hardwarové izolace pro Microsoft Edge |
| Defender pro Office 365 Plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno dne |
| **Správa identit**        | | |
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesel pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Zjišťování cloudových aplikací, Azure AD Připojení Health    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Aplikace Azure AD Office 365 Sign-On jednotné přihlašování (SSO): 10 aplikací na uživatele (aplikace Gallery SaaS, jako je Salesforce)* | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Premium 1 jednotné přihlašování: bez omezení (místní aplikace prostřednictvím Proxy aplikací Azure AD a aplikací mimo galerii pomocí šablon Self-Service Integrace aplikací)    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| **Správa zařízení a aplikací**        | | |
| Microsoft Intune, Windows Autopilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|Přístup k virtuální ploše (VDA)    |  |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|Windows Virtuální plocha (WVD)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
|Aktivace sdíleného počítače (SCA)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Microsoft Desktop Optimization Package    | |     ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| **Ochrana informací**        | | |
| Office 365 Ochrana před únikem dat, Plán ochrany informací v Azure 1    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Ochrana informací v okně pro koncový bod DLP    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| **Licence klientského přístupu (práva CAL)**    | | |
| Enterprise Cal Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| **Dodržování předpisů**        | | |
| Neomezená archivace e-mailů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Správce dodržování předpisů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| eDiscovery    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Blokování a blokování soudních sporů na místě    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
| Značky uchovávání informací a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) |
||||

\* Uživatelé, kteří mají přiřazený přístup k aplikacím SaaS, mohou získat přístup k jednotnému přihlašování až k 10 aplikacím. Správci mohou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednotnému přihlašování je povolený jenom pro 10 aplikací na uživatele najednou. Všechny Office 365 aplikace se počítají jako jedna aplikace.

## <a name="migration"></a>Migrace

Pokud chcete migrovat, můžete spolupracovat se svým partnerem a přesunout Microsoft 365 Business Premium předplatné a licence na vhodné předplatné Microsoft 365 E3 s jeho licencemi.

Následující části popisují, jaké změny je potřeba udělat, pokud nějaké jsou, a co můžete udělat po migraci.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 a data předplatného

Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, které zahrnují:

- Konfigurace předplatného, například názvy domén DNS.
- Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, Exchange Online poštovní schránky, weby SharePoint Online, OneDrive pro firmy složky a OneNote poznámkové bloky.

Vaši uživatelé teď mohou využívat neomezené úložiště v Exchange Online poštovních schránkách a OneDrive pro firmy složkách.

Pro více než 10 aplikací můžete začít používat Cloud App Discovery, Azure AD Připojení Health a jednotné přihlašování.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrana před hrozbou

Windows 10 Business zahrnuje tyto ochrany:

- Vynucení integrity procesu spouštění operačního systému
- Vynucení integrity citlivých operačních komponent
- Pokročilá zranitelnost a omezení zneužití po nulu
- Ochrana sítě založená na reputaci pro Microsoft Edge, Internet Explorer a Chrome
- Brána firewall založená na hostiteli
- Zmírnění rizik ransomwaru
- Hardwarová izolace pro Microsoft Edge
- Řízení aplikací využívající inteligentní zabezpečení Graph
- Řízení zařízení (USB)
- Ochrana sítě pro webové hrozby
- Pravidla prevence vniknutí hostitele

Windows 10 Enterprise E3 zahrnuje také podnikovou správu hardwarové izolace pro Microsoft Edge.

> [!NOTE]
> Uživatelé migrované do Microsoft 365 E3 budou pro další ochranu před hrozbou vyžadovat licenci Microsoft Defender Office 365 ochranu před internetovou hrozbou. Nezapomeňte si koupit další defender pro Office 365 licencí, aby všichni uživatelé v rozsahu vašeho Defenderu pro Office 365 licencí.

### <a name="device-management-with-intune"></a>Správa zařízení pomocí Intune

Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium obsahuje Windows 10 Business, které můžete nainstalovat pomocí Windows AutoPilota. Když migrujete na Microsoft 365 E3, každá uživatelská licence obsahuje Windows 10 Enterprise E3, kterou můžete nainstalovat také pomocí Windows Autopilota.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 Apps pro firmy

Váš Microsoft 365 Apps pro firmy klient nainstalovaný na vašich zařízeních automaticky začne používat funkce Microsoft 365 Apps pro velké organizace. Po migraci teď můžete použít:

- Zásady skupiny podpora
- Porovnání tabulek a dotazování
- Business intelligence
