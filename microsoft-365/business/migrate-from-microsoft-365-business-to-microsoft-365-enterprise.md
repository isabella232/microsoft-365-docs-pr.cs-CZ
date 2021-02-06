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
description: Zjistěte, jak můžete přejít z Microsoft 365 Business Premium na Microsoft 365 E3.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126195"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrace z Microsoftu 365 Business Premium na Microsoft 365 E3

Microsoft 365 Business Premium nabízí všechno, co potřebujete pro svoji malou firmu, a spojuje špičkové cloudové aplikace zvyšující produktivitu a jednoduchá správa zařízení a zabezpečení, které vašim zaměstnancům umožní odpracujte co nejlépe. V některých případech ale může být potřeba migrovat předplatné Microsoft 365 Business Premium na Microsoft 365 E3. 

Vaše firma například roste a potřebuje víc než 300 licencí (blahopřejeme).

Nebo vaše firma potřebuje podnikové funkce, jako je Microsoft 365 Apps pro podniky, Windows 10 Enterprise E3 nebo licence pro klientský přístup enterprise (CALs).

Upgrade je snadný: upgrade můžete spustit [z Centra pro správu.](../commerce/subscriptions/upgrade-to-different-plan.md) Všechna vaše data a konfigurace v aktuálním předplatném jsou zachovaná. Není nic, co byste se měli na migraci připravit a potom už nic dělat, kromě využití nových funkcí.

>[!Note]
>Můžete také použít předplatné Microsoft 365 Business Premium až pro 300 licencí a získat předplatné Microsoft 365 E3 pro více než 300 licencí. Program Microsoft Defender pro Office 365 ale není součástí Microsoftu 365 E3. Pro další ochranu před hrozbami byste měli přidat další program Defender pro licence Office 365, aby měli licenci všichni uživatelé, kteří mají obor vašeho programu Defender pro uživatele Office 365.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise

Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Microsoftu 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikace Office*    | [Microsoft 365 Apps pro firmy](#office-365-business)    | Microsoft 365 Apps for enterprise | 
| **Cloudové aplikace zvyšující produktivitu**        | | | 
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezená archivace Exchange Online    | 100GB limit úložiště na poštovní schránku a neomezená archivace Exchange Online | 
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Bez omezení | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbou**        | | | 
| Možnosti omezení útoku na ploše    | [Zobrazit tento seznam](#threat-protection) | Podniková správa hardwarové izolace pro Microsoft Edge | 
| Defender pro Office 365 (Plán 1) | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuté, ale můžete ho přidat na | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), podmíněný přístup, zpětný zápis hesel pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Aplikace Azure AD Office 365 s jednotným přihlašováním Sign-On (SSO): 10 aplikací na uživatele (aplikace SaaS v galerii, jako je Třeba Salesforce)* | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Jednotné přihlašování Azure AD Premium 1: žádný limit (místní aplikace přes proxy aplikace Azure AD a aplikace mimo galerii pomocí šablon Self-Service aplikace)    |     | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Správa zařízení a aplikací**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Přístup k virtuální ploše (VDA)    |  |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Windows Virtual Desktop (WVD)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
|Aktivace sdíleného počítače (SCA)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Balíček pro optimalizaci plochy Microsoftu    | |     ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Ochrana informací**        | | | 
| Office 365 Data Loss Prevention, Azure Information Protection (Plán 1)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Ochrana informací v okně pro ochranu před únikem informací o koncovém bodu    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Licence pro klientský přístup (práva CAL)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Správce konfigurace, Správa přístupových práv ve Windows)| |         ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| **Dodržování předpisů**        | | | 
| Neomezená archivace e-mailů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Správce dodržování předpisů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Blokování z důvodu soudního sporu a blokování z důvodu soudního sporu    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
| Značky uchovávání informací a zásady správy záznamů zpráv    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoftu 365 E3](../media/check-mark.png) | 
||||

\* Uživatelé, kteří mají přiřazený přístup k aplikacím SaaS, mohou získat přístup k jednotnému přihlašování až k 10 aplikacím. Správci mohou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů k různým aplikacím SaaS, ale přístup k jednotnému přihlašování je povolený jenom pro 10 aplikací na uživatele najednou. Všechny aplikace Office 365 se započítávají do jedné aplikace.

## <a name="migration"></a>Migrace

Pokud chcete migrovat, přesuňte ve svém partnerovi předplatné a licence Microsoft 365 Business Premium na vhodné předplatné Microsoft 365 E3 s jeho licencemi.

Následující části popisují, jaké změny je potřeba udělat (pokud nějaké) a co můžete po migraci udělat.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurace a data předplatného Microsoftu 365

Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, mezi které patří:

- Konfigurace předplatného, například názvy domén DNS
- Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb pro zvýšení produktivity a jejich data, jako jsou teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.

Uživatelé si teď užijte neomezené úložiště v poštovních schránkách Exchange Online a složkách OneDrivu pro firmy.

Pro víc než 10 aplikací můžete začít používat Cloud App Discovery, Azure AD Connect Health a jednotné přihlašování.

>[!Note]
>Uživatelé, kteří migrují na Microsoft 365 E3, už nebudou moci aplikaci MileIQ používat.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrana před hrozbou

Windows 10 Business obsahuje tyto ochrany:

- Vynucení integrity procesu spouštění operačního systému
- Vynucení integrity citlivých operačních součástí
- Pokročilá ohrožení zabezpečení a omezení rizik zneužití po nulách
- Ochrana sítě podle reputace pro Microsoft Edge, Internet Explorer a Chrome
- Brána firewall založená na hostiteli
- Omezení ransomwaru
- Hardwarová izolace pro Microsoft Edge
- Application control powered by the Intelligent Security Graph
- Řídicí zařízení (USB)
- Ochrana sítě pro webové hrozby
- Pravidla pro prevenci vniknutí do hostitele

Součástí Windows 10 Enterprise E3 je také podniková správa hardwarové izolace pro Microsoft Edge.

>[!Note]
>Každý uživatel, který migroval do Microsoftu 365 E3, bude pro další ochranu před hrozbou vyžadovat licenci na Microsoft Defender pro Office 365. Kupte si další defender pro licence Office 365, aby všichni uživatelé, kteří mají obor vašeho programu Defender pro uživatele Office 365, mít licenci. 
>

### <a name="device-management-with-intune"></a>Správa zařízení pomocí Intune

Před migrací, včetně zaregistrovaná zařízení a nastavení zařízení a aplikací, nemusíte provádět žádné změny ve své aktuální konfiguraci Intune.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium zahrnuje Windows 10 Business, který si můžete nainstalovat pomocí Windows AutoPilota. Při migraci na Microsoft 365 E3 zahrnuje každá uživatelská licence Windows 10 Enterprise E3, kterou můžete nainstalovat také pomocí Windows Autopilota.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 Apps pro firmy

Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních začne automaticky používat funkce Microsoft 365 Apps pro podniky. Po migraci teď můžete použít:

 - Zásady skupiny podpory
 - Porovnání tabulek a jejich dotazy
 - Business intelligence

