---
title: Migrace na Microsoft 365 Business z Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Pokud máte předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium.
ms.openlocfilehash: d139d07c946ff3efed3db3a73eb5e1a4ae66c190
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "52623599"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrace z Office 365 E3 na Microsoft 365 Business Premium

Microsoft 365 Business Premium má všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové produktivní aplikace s jednoduchou snadná správa a zabezpečení zařízení. Pokud máte aktuálně předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.

Migrace je snadná: Nejdřív přepnete licence a všechna data a informace o uživatelích v aktuálním předplatném se zachová. Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium

Tato tabulka zobrazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Office 365 E3 |
|:-------|:-----|:-----|
| **Místní**        | | |
| Office aplikace<sup>1</sup>    | Microsoft 365 Apps pro firmy    | Aplikace Microsoft 365 pro podniky |
| **Cloudové aplikace pro zvýšení produktivity**        | | |
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezený počet Exchange Online – archiv    | Limit úložiště 100 GB na poštovní schránku a neomezený počet Exchange Online – archiv |
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezená | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) |
| **Ochrana před hrozbou**        | | |
| Defender pro Office 365 Plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno dne |
| **Správa identit**        | | |
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesel pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| **Správa zařízení a aplikací**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivace sdíleného počítače|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| Upgradujte práva na Windows 10 Pro z win 7/8.1 Pro licencí|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    ||
| **Ochrana informací**        | | |
|Office 365 Ochrana před únikem dat|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, nástroj BitLocker vynucení|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|Plán ochrany informací v Azure 1, popisky citlivosti|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licence klientského přístupu (práva CAL)**|||
|Enterprise Cal Suite (Exchange, SharePoint, Skype)||![Součástí Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium aplikace Office nezahrnuje aktivaci multilicence prostřednictvím Zásady skupiny, telemetrie aplikací, ovládacích prvků aktualizace, porovnání tabulek a dotazování nebo business Intelligence.

## <a name="migration"></a>Migrace

Pokyny k migraci [](../commerce/subscriptions/change-plans-manually.md) předplatného najdete v tématu Ruční změna plánů, pokud chcete přesunout jenom několik lidí do Microsoft 365 Business Premium. Můžete taky [upgradovat všechny automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo můžete spolupracovat s partnerem a přesunout předplatné E3 a licence na Microsoft 365 Business Premium předplatné.
Následující části popisují případné změny, které je potřeba udělat, a co můžete udělat po migraci.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 Konfigurace a data předplatného E3
Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, mezi které patří:

- Konfigurace předplatného, jako jsou záznamy DNS a názvy domén.
- Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, Exchange Online poštovní schránky, weby SharePoint Online, OneDrive pro firmy složky a OneNote poznámkové bloky.
- Office aplikace se automaticky škálují. Office 365 moderní licencování zkontroluje přiřazení licence uživatele každých 72 hodin a převede Office aplikace na verzi, která odpovídá uživatelskému předplatnému.

### <a name="windows-10"></a>Windows 10

Pokud vaše Windows ještě nejsou v aktualizaci Windows Pro creatorů, upgradujte je na [Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Nastavení zásad pro ochranu uživatelských zařízení a souborů

> [!NOTE]
> Pokud nastavíte zásady a Office 365 MDM, budou tato zařízení  uvedená na stránce Zařízení v centru Microsoft 365 správy. Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.

Pokud jste upgradovali všechny uživatele ve vaší organizaci na Microsoft 365 Business Premium, zobrazí se průvodce nastavením na domovské stránce a můžete postupovat podle pokynů průvodce nastavením nastavit [Microsoft 365 Business Premium](set-up.md) a chránit soubory a mobilní zařízení.

Tento postup můžete provést taky na stránce Zařízení:
  
1. V Centru pro správu v levém navigačním panelu přejděte na **Zásady** \> **zařízení**.

2. Na stránce **Zásady zařízení** zvolte **Přidat**.

3. V podokně **Přidat zásadu** pojmete zásadu **a** v rozevíracím seznamu zvolte typ zásady.

     Můžete nastavit zásady aplikace pro ochranu souborů na zařízeních s Androidem a iPhone a Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení vlastněná Windows 10 zařízeními. Podrobnosti najdete v následujících odkazech:

  - [Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem](app-protection-settings-for-android-and-ios.md)

  - [Nastavení ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md)

  - [Nastavení ochrany zařízení pro Windows 10 počítače](protection-settings-for-windows-10-pcs.md)
  
4. Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:

  - Postup [pro Windows najdete v Windows](set-up-windows-devices.md) Windows zařízení pro Microsoft 365 Business Premium uživatele. 

  - Postup pro telefony s [Androidem a iPhony najdete v tématu](set-up-mobile-devices.md) Microsoft 365 Business Premium mobilních zařízení pro uživatele. 
  
### <a name="mailbox-size"></a>Velikost poštovní schránky

Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Exchange Online Plán 1. Při migraci na Microsoft 365 Business Premium, pokud některý z vašich uživatelů překročí 50 GB úložiště poštovních schránek, doporučujeme tomuto uživateli přiřadit plán Exchange Online Plán 2 a odebrat plán Exchange Online 1, protože není možné přiřadit obojí.

### <a name="threat-protection"></a>Ochrana před hrozbou

Po migraci na Microsoft 365 Business Premium máte Defender pro Office 365. Přehled [najdete v Office 365](../security/office-365-security/defender-for-office-365.md) Microsoft Defenderu. Pokud chcete nastavit, [podívejte](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)se na nastavení bezpečných odkazů [,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)nastavení bezpečných příloh a nastavení [anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)v Defenderu pro Office 365 .

### <a name="sensitivity-labels"></a>Štítky utajení

Pokud chcete začít používat [](../compliance/sensitivity-labels.md) popisky citlivosti, podívejte se na téma Přehled popisků citlivosti a vytváření a správa popisků [citlivosti](../business-video/create-sensitivity-labels.md) videa.

## <a name="related-content"></a>Související obsah

[Ruční změna plánů](../commerce/subscriptions/change-plans-manually.md) (článek)\
[Upgrade Windows zařízení na Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (video)\
[Nastavení ochrany aplikací pro zařízení s Androidem nebo iOS](app-protection-settings-for-android-and-ios.md) (článek)\
[Nastavení nebo úprava nastavení ochrany aplikací pro Windows 10 zařízení](protection-settings-for-windows-10-devices.md) (článek)\
[]

