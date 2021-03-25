---
title: Migrace z Microsoftu 365 Business na Microsoft 365 E3
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
description: Zjistěte, jak přesunout svou firmu z Microsoft 365 Business Premium na Microsoft 365 E3.
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164507"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrace z Microsoft 365 Business Premium na Microsoft 365 E3

Microsoft 365 Business Premium má všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace založené na produktivitě s jednoduchou snadná správa zařízení a zabezpečení, které vašim zaměstnancům umožňují dělat nejlepší práci. V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium na Microsoft 365 E3. 

Vaše firma například roste a potřebuje víc než 300 licencí (mimochodem blahopřejeme).

Nebo vaše firma potřebuje podnikové funkce, jako jsou Aplikace Microsoft 365 pro podniky, Windows 10 Enterprise E3 nebo Licence klientského přístupu enterprise (CAL).

Upgrade je snadný: Upgrade můžete spustit z [Centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md). Všechna vaše data a konfigurace v aktuálním předplatném se zachová. Není nic, co byste měli udělat, abyste se připravili na migraci a potom nic dělat, kromě využití nových funkcí.

>[!Note]
>Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí. Microsoft Defender pro Office 365 ale není součástí Microsoft 365 E3. Pokud chcete pokračovat v ochraně před hrozbami, měli byste přidat další licence Defenderu pro Office 365, aby měli licenci všichni uživatelé, kteří mají v rámci vašeho programu Defender for Office 365 licenci.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise

V této tabulce jsou uvedené rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Microsoftu 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikace Office*    | [Aplikace Microsoft 365 pro firmy](#office-365-business)    | Aplikace Microsoft 365 pro podniky | 
| **Cloudové aplikace pro zvýšení produktivity**        | | | 
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezenou archivaci Exchange Online    | Limit úložiště 100 GB na poštovní schránku a neomezenou archivaci Exchange Online | 
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezená | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Ochrana před hrozbou**        | | | 
| Možnosti omezení útoku na povrch    | [Zobrazit tento seznam](#threat-protection) | Enterprise management of hardware-based isolation for Microsoft Edge | 
| Defender pro Office 365 – plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno dne | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesla pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Aplikace Azure AD Office 365 Single Sign-On (SSO): 10 aplikací na uživatele (aplikace SaaS galerie, jako je Salesforce)* | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Jednotné přihlašování k Azure AD Premium 1: bez omezení (místní aplikace prostřednictvím proxy aplikací Azure AD a aplikací mimo galerii pomocí šablon Self-Service Integrace aplikací)    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Správa zařízení a aplikací**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Přístup k virtuální ploše (VDA)    |  |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Virtuální plocha Windows (WVD)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Aktivace sdíleného počítače (SCA)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Microsoft Desktop Optimization Package    | |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Ochrana informací**        | | | 
| Office 365 Data Loss Prevention, Azure Information Protection Plan 1    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Ochrana informací v okně pro koncový bod DLP    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Licence klientského přístupu (práva CAL)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Správce konfigurace, Správa přístupových práv k Windows)| |         ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Dodržování předpisů**        | | | 
| Neomezená archivace e-mailů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Správce dodržování předpisů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Blokování a blokování soudních sporů na místě    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Značky uchovávání informací a zásady uchovávání informací pro správu záznamů zasílání zpráv (MRM)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
||||

\* Uživatelé, kteří mají přiřazený přístup k aplikacím SaaS, mohou získat přístup k jednotnému přihlašování až k 10 aplikacím. Správci mohou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednotnému přihlašování je povolený jenom pro 10 aplikací na uživatele najednou. Všechny aplikace Office 365 se počítají jako jedna aplikace.

## <a name="migration"></a>Migrace

Pokud chcete migrovat, přesuňte předplatné a licence Microsoft 365 Business Premium na vhodné předplatné Microsoft 365 E3 s jeho licencemi.

Následující části popisují, jaké změny je potřeba udělat, pokud nějaké jsou, a co můžete udělat po migraci.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurace a data předplatného Microsoft 365

Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, které zahrnují:

- Konfigurace předplatného, například názvy domén DNS.
- Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.

Vaši uživatelé teď mohou využívat neomezené úložiště v poštovních schránkách Exchange Online a ve složkách OneDrivu pro firmy.

Pro více než 10 aplikací můžete začít používat Cloud App Discovery, Azure AD Connect Health a jednotné přihlašování.

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
- Řízení aplikací využívající inteligentní graf zabezpečení
- Řízení zařízení (USB)
- Ochrana sítě pro webové hrozby
- Pravidla prevence vniknutí hostitele

Windows 10 Enterprise E3 zahrnuje také podnikovou správu hardwarové izolace pro Microsoft Edge.

>[!Note]
>Uživatelé, kteří migrují na Microsoft 365 E3, budou každý z nich vyžadovat licenci Microsoft Defender pro Office 365, aby bylo možné pokračovat v ochraně před hrozbou. Nezapomeňte si koupit další licence Defenderu pro Office 365, aby všichni uživatelé, kteří mají v rámci vašeho programu Defender for Office 365 oprávnění, mají licenci. 
>

### <a name="device-management-with-intune"></a>Správa zařízení pomocí Intune

Před migrací nemusíte provádět žádné změny v aktuální konfiguraci Intune, což zahrnuje zaregistrovaná zařízení a nastavení zařízení a aplikací.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium zahrnuje Windows 10 Business, který si můžete nainstalovat pomocí Windows AutoPilota. Když migrujete na Microsoft 365 E3, každá uživatelská licence zahrnuje Windows 10 Enterprise E3, který můžete nainstalovat také pomocí Windows Autopilota.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikace Microsoft 365 pro firmy

Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních automaticky začne používat funkce aplikací Microsoft 365 pro podniky. Po migraci teď můžete použít:

 - Zásady skupiny podpora
 - Porovnání tabulek a dotazování
 - Business intelligence

