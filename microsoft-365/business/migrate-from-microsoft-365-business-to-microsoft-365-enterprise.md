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
description: Přečtěte si, jak přesunout firmu z Microsoft 365 Business Premium na Microsoft 365 E3.
ms.openlocfilehash: 3f1bb9591e1bd2bac49326325ce6c8c2d6778497
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558232"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Migrace z aplikace Microsoft 365 Business Premium na Microsoft 365 E3

Microsoft 365 Business Premium obsahuje vše potřebné pro vaši malou firmu a spojuje aplikace pro práci založené na cloudu co nejlépe ve třídě s jednoduchou správou a zabezpečením zařízení, které umožní zaměstnancům co nejvýhodnější práci. V některých případech ale možná budete muset migrovat předplatné Microsoft 365 Business Premium na Microsoft 365 E3. 

Váš podnik například vyrostl a potřebuje více než 300 licencí (blahopřejení).

Nebo potřebuje vaše firma funkce Enterprise, jako jsou aplikace Microsoft 365 pro podnik, Windows 10 Enterprise E3 nebo licence Enterprise Client Access (CAL).

Snadná inovace: můžete zahájit upgrade [z centra pro správu](../commerce/subscriptions/upgrade-to-different-plan.md). Všechna vaše data a konfigurace ve vašem aktuálním předplatném jsou zachována. Není nic, co byste chtěli připravit na migraci a nic nedělat, dokud nebudete moci provádět nové funkce.

>[!Note]
>Můžete také použít předplatné Microsoft 365 Business Premium pro až 300 sedadel a získat předplatné Microsoft 365 E3 pro více než 300 sedadel. Microsoft Defender pro Office 365 se ale netýká Microsoft 365 E3. Za účelem zachování ochrany před hrozbami byste měli přidat další program Defender for Office 365 licenses, aby všichni uživatelé, kteří jsou v dosahu svého programu Defender pro Office 365, měli licenci.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 Enterprise

Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Microsoft 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Aplikace Office *    | [Aplikace Microsoft 365 pro firmy](#office-365-business)    | Microsoft 365 Apps for enterprise | 
| **Kancelářské aplikace**        | | | 
| Exchange Online a Outlook    | 50 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online    | 100 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online | 
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | 1 TB limit úložiště na uživatele    | Neomezené | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbami**        | | | 
| Možnosti pro redukci pro omezení plochy    | [Podívejte se na tento seznam](#threat-protection) | Podniková správa izolace hardwaru pro Microsoft Edge | 
| Defender pro Office 365 plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale můžete ho přidat | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), Azure AD Multi-Factor Authentication (MFA), podmíněný přístup, zápis hesel pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Zjišťování Cloud App, Azure AD Connect    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Aplikace Azure AD 365 Single Sign-On (SSO): 10 aplikací na uživatele (Galerie SaaS aplikací, například Salesforce) * | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Jednotné přihlašování k Azure AD Premium 1: bez limitu (místní aplikace prostřednictvím proxy aplikace Azure AD a aplikací mimo galerii s použitím Self-Service šablon pro integraci aplikací)    |     | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| **Správa zařízení a aplikací**        | | | 
| Microsoft Intune, Windows autopilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|Přístup k virtuální ploše (VDA)    |  |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|Virtuální plocha systému Windows (WVD)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
|Aktivace sdíleného počítače (SCA)    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png) |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Balíček Microsoft Desktop Optimization    | |     ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| **Ochrana informací**        | | | 
| Ochrana před únikem dat v Office 365, plán Azure Information Protection 1    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Ochrana informací v okně pro službu DLP koncového bodu    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| **Licence klientského přístupu (licence CAL)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| **Požadavků**        | | | 
| Časově neomezené archivace e-mailů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Správce dodržování předpisů    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Sad    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Blokování pro archivaci a držení soudní pře    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
| Značky uchování záznamů zpráv a zásady uchovávání informací    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Uživatelé, kterým byl přiřazen přístup k aplikacím SaaS, můžou získat přístup k jednotnému přihlašování k až 10 aplikacím. Správci můžou nakonfigurovat jednotné přihlašování a měnit přístup uživatelů na různé aplikace SaaS, ale přístup pomocí jednotného přihlašování je povolený jenom u 10 aplikací na jednoho uživatele najednou. Všechny aplikace Office 365 se počítají jako jediná aplikace.

## <a name="migration"></a>Migrace

Pokud chcete migrovat, spolupracujte se svým partnerem a přesuňte předplatné Microsoft 365 Business Premium a licence na vhodný tarif Microsoft 365 E3 s jeho licencemi.

V následujících částech jsou popsány změny, které je třeba udělat, pokud existují, a co můžete udělat po migraci.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurace a data předplatného Microsoft 365

Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, což zahrnuje:

- Konfigurace předplatného, třeba názvy domén DNS.
- Účty uživatelů a skupin a nastavení ověřování, například vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace produktivity služeb a jejich data, například týmy, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.

Uživatelé teď můžou využívat neomezené úložiště v poštovních schránkách Exchange Online a složkách OneDrivu pro firmy.

Můžete začít používat vyhledávání Cloud App Appu, stav Azure AD Connect a jednotné přihlašování pro více než 10 aplikací.

>[!Note]
>Uživatelé migrace do Microsoft 365 E3 už nemůžou používat MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Ochrana před hrozbami

Windows 10 Business zahrnuje tyto ochrany:

- Vynucení integrity procesu spuštění operačního systému
- Vynucení integrity citlivých provozních součástí
- Zdokonalená řešení chyb a zneužití nulového počtu dnů
- Ochrana sítě založená na pověsti pro Microsoft Edge, Internet Explorer a Chrome
- Hostitelská brána firewall
- Ransomwaru Zklidňující fakta
- Hardwarově izolovaná izolace pro Microsoft Edge
- Řízení aplikací poháněné grafem inteligentního zabezpečení
- Ovládání zařízení (USB)
- Ochrana sítě pro webové hrozby
- Pravidla prevence vniknutí hostitele

Windows 10 Enterprise E3 zahrnuje také podnikovou správu izolace hardwaru pro Microsoft Edge.

>[!Note]
>Uživatelé, kteří jsou migrováni do Microsoft 365 E3, budou muset mít licenci programu Microsoft Defender pro Office 365 pro pokračování ochrany proti ohrožení. Nezapomeňte si zakoupit další program Defender for Office 365 licenses, aby všichni uživatelé, kteří jsou v dosahu svého programu Defender pro Office 365, měli licenci. 
>

### <a name="device-management-with-intune"></a>Správa zařízení s Intune

Před migrací nemusíte dělat žádné změny v aktuální konfiguraci Intune, včetně zaregistrovaných zařízení a nastavení zařízení a aplikací.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium zahrnuje Windows 10 Business, který se dá nainstalovat s autopilotem Windows. Když migrujete na Microsoft 365 E3, každá uživatelská licence obsahuje Windows 10 Enterprise E3, který se dá taky nainstalovat s autopilotem Windows.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Aplikace Microsoft 365 pro firmy

Váš klient Microsoft 365 Apps pro firmy nainstalovaný na vašich zařízeních bude automaticky používat funkce aplikací Microsoft 365 pro podnik. Po migraci můžete použít:

 - Aktivace multilicence prostřednictvím zásad skupiny
 - Telemetrie aplikací
 - Aktualizace ovládacích prvků
 - Porovnání tabulky a dotazy
 - Business Intelligence

