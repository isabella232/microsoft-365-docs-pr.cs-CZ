---
title: Migrace na Microsoft 365 Business z Office 365 E3
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
description: Přečtěte si, jak přesunout firmu na Microsoft 365 Business Premium z Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081798"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Přechod z Office 365 E3 na Microsoft 365 Business Premium 

Microsoft 365 Business Premium má vše, co potřebujete pro vaši malou firmu, a kombinuje nejlepší cloudové aplikace na úrovni produktivity ve své třídě s jednoduchou správou a zabezpečením zařízení. Pokud máte v současné době předplatné Office 365 E3, ale nemáte víc než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.

Migrace je snadná: Nejprve přepnete licence a všechny vaše data a informace o uživateli v aktuálním předplatném budou zachovány. Po migraci budete muset nastavit funkce přidané v Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium

Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.

| Funkce    | Podpora v Microsoftu 365 Business Premium    | Podpora v Office 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Aplikace Office<sup>1</sup>    | Aplikace Microsoft 365 pro firmy    | Aplikace Microsoft 365 pro podniky | 
| **Cloudové aplikace pro zvýšení produktivity**        | | | 
| Exchange Online a Outlook    | Limit úložiště 50 GB na poštovní schránku a neomezená archivace Exchange Online    | Limit úložiště 100 GB na poštovní schránku a neomezený archivaci Exchange Online | 
| Týmy    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | Limit úložiště 1 TB na uživatele    | Neomezené | 
| Yammer, SharePoint Online, Plánovač, Stream    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbami**        | | | 
| Plán 1 pokročilé ochrany před hrozbami Office 365 | ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale může být přidáno na | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), vícefaktorové ověřování Azure (MFA), podmíněný přístup, zpětný zápis hesel pro místní identity|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Správa zařízení a aplikací**        | | |
| Microsoft Intune, Automaticképilot systému Windows|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivace sdíleného počítače|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| Práva na upgrade na Windows 10 Pro z licencí Win 7/8.1 Pro|     ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrana informací**        | | |
|Ochrana před ztrátou dat v Office 365|    ![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, Vynucení nástroje Bitlocker|![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, popisky citlivosti|![Součástí služby Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licence klientského přístupu (práva CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Součástí Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Verze aplikací Office pro Microsoft 365 Business Premium nezahrnuje aktivaci svazku prostřednictvím zásad skupiny, telemetrie aplikací, ovládacích prvků aktualizací, porovnání tabulek a dotazování nebo business intelligence.

## <a name="migration"></a>Migrace

Pokud chcete migrovat předplatné, přečtěte si pokyny v [tématu Ruční změna plánů,](../commerce/subscriptions/change-plans-manually.md) pokud chcete do Microsoft 365 Business Premium přesunout jemnou lidi. Můžete také [upgradovat všechny uživatele automaticky](../commerce/subscriptions/upgrade-to-different-plan.md)nebo spolupracovat s partnerem a přesunout předplatné e3 a licence na předplatné Microsoft 365 Business Premium.
Následující části popisují změny, které je třeba provést, pokud existuje, a co můžete udělat po migraci.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfigurace předplatného Office 365 E3 a data
Před migrací nemusíte provádět žádné změny aktuálního předplatného nebo dat, což zahrnuje:

- Konfigurace předplatného, například záznamy DNS a názvy domén.
- Uživatelské a skupinové účty a nastavení ověřování, jako je například vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace služeb produktivity a jejich data, jako jsou Teams, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.
- Aplikace Office se automaticky škáluje. Moderní licencování Office 365 bude každých 72 hodin kontrolovat přiřazení licencí uživatele a převádí aplikace Office na verzi, která odpovídá uživatelskému předplatnému.

### <a name="windows-10"></a>Windows 10

Pokud váš Windows ještě není v aktualizaci Windows Pro Creator, upgradujte je na [aktualizaci Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Nastavení zásad ochrany uživatelských zařízení a souborů

> [!NOTE]
> Pokud nastavíte zásady a zařízení Office 365 MDM, budou tato zařízení uvedena na stránce **Zařízení** v Centru pro správu Microsoftu 365. Všechny zásady, které nastavíte, se zobrazí v seznamu klasických zásad na [portálu Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Po přiřazení licencí k aplikaci Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.

Pokud jste všechny uživatele ve vaší organizaci upgradovali na Microsoft 365 Business Premium, zobrazí se na domovské stránce Průvodce instalací a můžete postupovat podle [nastavení Microsoft 365 Business Premium v krocích průvodce nastavením](set-up.md) za účelem ochrany souborů a mobilních zařízení.

Můžete také provést tyto kroky na stránce Zařízení:
  
1. V Centru pro správu v levém **Devices** navigačním panelu přejděte na \> **položku Zásady zařízení**.
    
2. Na stránce **Zásady zařízení** zvolte **Přidat**.
    
3. V podokně **Přidat zásady** pojmenujte zásadu a zvolte **typ zásady** z rozevíracího panelu. 
    
     Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních s Androidem a iPhonem a také na Windows 10 a nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností. Podrobnosti naleznete v následujících odkazech:
    
  - [Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem](app-protection-settings-for-android-and-ios.md)
    
  - [Nastavení ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Nastavení ochrany zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:
    
  - Postup pro zařízení s Windows najdete v tématu [Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
  - Postup pro telefony a iPhony s Androidem najdete v článku [Nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium.](set-up-mobile-devices.md) 

### <a name="threat-protection"></a>Ochrana před hrozbami

Po migraci na Microsoft 365 Business Premium máte office 365 ATP. Přehled najdete v [článku Office 365 ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Nastavení naleznete v [tématu nastavení bezpečných odkazů ATP](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [nastavení bezpečných příloh ATP](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)a [nastavení ochrany proti phishingu .](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Štítky utajení

Chcete-li začít používat popisky citlivosti, přečtěte si téma [Přehled popisků citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) a vytvoření a správa videa [s popisky citlivosti.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)
