---
title: Migrace z Office 365 E3 na Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Zjistěte, jak přesunout firmu na Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: cb70260201686cae02428c715ac98ffe2f88787f
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198091"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrace z Office 365 E3 na Microsoft 365 Business Premium

Microsoft 365 Business Premium nabízí všechno, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace založené na produktivitě s jednoduchou snadná správa a zabezpečení zařízení. Pokud máte momentálně předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium, abyste získali další funkce zabezpečení.

Migrace je snadná: Nejdřív přepnete licence a všechna data a informace o uživatelích v aktuálním předplatném se zachová. Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium

V této tabulce jsou uvedené rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Office 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Aplikace Office<sup>1</sup>    | Aplikace Microsoft 365 pro firmy    | Aplikace Microsoft 365 pro podniky | 
| **Cloudové aplikace pro zvýšení produktivity**        | | | 
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezenou archivaci Exchange Online    | Limit úložiště 100 GB na poštovní schránku a neomezenou archivaci Exchange Online | 
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezená | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbou**        | | | 
| Defender pro Office 365 – plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno dne | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure AD (MFA), Podmíněný přístup, zpětný zápis hesla pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Správa zařízení a aplikací**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivace sdíleného počítače|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| Upgrade práv na Windows 10 Pro z licencí Win 7/8.1 Pro|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrana informací**        | | |
|Prevence ztráty dat v Office 365|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, vynucení nástroje Bitlocker|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|Plán ochrany informací v Azure 1, popisky citlivosti|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licence klientského přístupu (práva CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Součástí Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Verze aplikací Office pro Microsoft 365 Business Premium nezahrnuje aktivaci multilicence přes Zásady skupiny, telemetrii aplikací, ovládací prvky aktualizací, porovnání tabulek a dotazy nebo business Intelligence.

## <a name="migration"></a>Migrace

Pokud chcete do [](../commerce/subscriptions/change-plans-manually.md) Microsoftu 365 Business Premium přesunout jenom pár lidí, přečtěte si pokyny k migraci předplatného ručně. Můžete také [upgradovat všechny automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo můžete spolupracovat s partnerem a přesunout předplatné E3 a licence na předplatné Microsoft 365 Business Premium.
Následující části popisují případné změny, které je potřeba udělat, a co můžete udělat po migraci.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfigurace a data předplatného Office 365 E3
Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, mezi které patří:

- Konfigurace předplatného, jako jsou záznamy DNS a názvy domén.
- Uživatelské a skupinové účty a nastavení ověřování, jako je vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.
- Aplikace Office se automaticky zmenšují. Moderní licencování Office 365 zkontroluje přiřazení licencí uživatele každých 72 hodin a převede aplikace Office na verzi, která odpovídá předplatnému uživatele.

### <a name="windows-10"></a>Windows 10

Pokud váš systém Windows ještě není v aktualizaci Windows Pro Creator, [upgradujte je na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Nastavení zásad pro ochranu uživatelských zařízení a souborů

> [!NOTE]
> Pokud nastavíte zásady a zařízení Office 365 MDM,  budou tato zařízení uvedená na stránce Zařízení v Centru pro správu Microsoftu 365. Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.

Pokud jste upgradovali všechny uživatele ve vaší organizaci na Microsoft 365 Business Premium, zobrazí se průvodce nastavením na domovské stránce a můžete postupovat podle pokynů Průvodce nastavením nastavit [Microsoft 365 Business Premium](set-up.md) k ochraně souborů a mobilních zařízení.

Tento postup můžete provést taky na stránce Zařízení:
  
1. V Centru pro správu v levém navigačním panelu přejděte na **Zásady** \> **zařízení**.
    
2. Na stránce **Zásady zařízení** zvolte **Přidat**.
    
3. V podokně **Přidat zásadu** pojmete zásadu **a** v rozevíracím seznamu zvolte typ zásady. 
    
     Můžete nastavit zásady aplikace pro ochranu souborů na zařízeních s Androidem a iPhonem i ve Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností. Podrobnosti najdete v následujících odkazech:
    
  - [Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem](app-protection-settings-for-android-and-ios.md)
    
  - [Nastavení ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Nastavení ochrany zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:
    
  - Postup pro zařízení s Windows najdete v tématu Nastavení zařízení s Windows pro uživatele [Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
  - Postup pro telefony s Androidem a iPhony najdete v tématu Nastavení mobilních zařízení pro uživatele [Microsoftu 365 Business Premium.](set-up-mobile-devices.md) 
  
### <a name="mailbox-size"></a>Velikost poštovní schránky

Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Plán 1 Exchange Online. Pokud některý z vašich uživatelů při migraci na Microsoft 365 Business Premium překročí 50 GB úložiště poštovních schránek, doporučujeme tomuto uživateli přiřadit plán 2 Exchange Online a odebrat plán 1 Exchange Online, protože není možné přiřadit obojí.


### <a name="threat-protection"></a>Ochrana před hrozbou

Po migraci na Microsoft 365 Business Premium máte Defender pro Office 365. Přehled [najdete v tématu Microsoft Defender pro Office 365.](../security/office-365-security/defender-for-office-365.md) Pokud chcete nastavit, podívejte se na nastavení bezpečných odkazů [,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [nastavení](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)bezpečných příloh a nastavení anti-phishing v [Defenderu pro Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Štítky utajení

Pokud chcete začít používat [](../compliance/sensitivity-labels.md) popisky citlivosti, podívejte se na téma Přehled popisků citlivosti a vytváření a správa popisků [citlivosti](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videa.
