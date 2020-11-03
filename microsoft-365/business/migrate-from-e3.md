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
ms.openlocfilehash: b8aa58f1f050ec6247479ed02e142507a2df45fc
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842154"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Migrace z Office 365 E3 na Microsoft 365 Business Premium 

Microsoft 365 Business Premium obsahuje vše potřebné pro vaši malou firmu a spojuje aplikace pro optimální práci založené na cloudu s jednoduchou správou a zabezpečením zařízení. Pokud aktuálně máte předplatné Office 365 E3, ale nepoužíváte více než 300 zaměstnanců, zvažte přechod na Microsoft 365 Business Premium pro přidané funkce zabezpečení.

Snadná migrace: Nejdřív si přepínáte licence a všechny vaše data a uživatelské informace jsou zachovány. Po migraci budete muset nastavit funkce, které se přidají v Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Rozdíly mezi Office 365 E3 a Microsoft 365 Business Premium

Tato tabulka ukazuje rozdíly mezi Microsoft 365 Business Premium a Office 365 E3.

| Funkce    | Podpora v Microsoft 365 Business Premium    | Podpora v Office 365 E3 | 
|:-------|:-----|:-----|
| **Místní**        | | | 
| Aplikace Office<sup>1</sup>    | Aplikace Microsoft 365 pro firmy    | Aplikace Microsoft 365 pro podniky | 
| **Kancelářské aplikace**        | | | 
| Exchange Online a Outlook    | 50 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online    | 100 GB limit úložiště pro každou poštovní schránku a neomezené archivaci Exchange Online | 
| Teams    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| OneDrive pro firmy    | 1 TB limit úložiště na uživatele    | Neomezené | 
| Yammer, SharePoint Online, Planner, Stream    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Ochrana před hrozbami**        | | | 
| Defender pro Office 365 plán 1 | ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | Není zahrnuto, ale můžete ho přidat | 
| **Správa identit**        | | | 
| Samoobslužné resetování hesla pro hybridní účty Azure Active Directory (Azure AD), Azure Multi-Factor Authentication (MFA), podmíněný přístup, zápis hesel pro místní identity|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Správa zařízení a aplikací**        | | |
| Microsoft Intune, Windows autopilot|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivace sdíleného počítače|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    | ![Součástí Office 365 E3](../media/check-mark.png)| 
| Upgrade práv na Windows 10 pro na licence Win 7/8.1 pro|     ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Ochrana informací**        | | |
|Ochrana před únikem dat v Office 365|    ![Součástí Microsoft 365 Business Premium](../media/check-mark.png)|![Součástí Office 365 E3](../media/check-mark.png)|
|Plán služby Azure Information Protection 1, vynucení nástroje BitLocker|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|Plán služby Azure Information Protection 1, popisky citlivosti|![Součástí Microsoft 365 Business Premium](../media/check-mark.png)||
|**Licence klientského přístupu (licence CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Součástí Office 365 E3](../media/check-mark.png)|

<sup>1</sup> verze Microsoft 365 Business Premium aplikací Office nezahrnují aktivaci multilicence prostřednictvím zásad skupiny, telemetrie aplikací, ovládacích prvků aktualizace, porovnání tabulek a dotazů nebo Business Intelligence.

## <a name="migration"></a>Migrace

Pokud chcete migrovat předplatné, přečtěte si článek [Ruční změna plánů](../commerce/subscriptions/change-plans-manually.md) , jestli chcete přesunout jenom pár lidí na Microsoft 365 Business Premium. Můžete taky [automaticky upgradovat všechny uživatele](../commerce/subscriptions/upgrade-to-different-plan.md)nebo spolupracovat s partnerem, abyste mohli přesunout předplatné E3 a licence na předplatné Microsoft 365 Business Premium.
V následujících částech jsou popsány změny, které je třeba udělat, pokud existují, a co můžete udělat po migraci.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfigurace a data předplatného Office 365 E3
Před migrací nemusíte provádět žádné změny aktuálního předplatného ani dat, což zahrnuje:

- Konfigurace předplatného, například záznamy DNS a názvy domén
- Účty uživatelů a skupin a nastavení ověřování, například vícefaktorové ověřování nebo zásady podmíněného přístupu.
- Konfigurace produktivity služeb a jejich data, například týmy, poštovní schránky Exchange Online, weby SharePointu Online, složky OneDrivu pro firmy a poznámkové bloky OneNotu.
- Aplikace Office se přizpůsobí automaticky. Office 365 moderní licencování zkontroluje přiřazení licencí uživatele každých 72 hodin a převede aplikace Office na verzi, která odpovídá předplatnému uživatele.

### <a name="windows-10"></a>Windows 10

Pokud vaše okna ještě nejsou ve Windows pro Creator Update, [Upgradujte si je na Windows pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Nastavení zásad pro ochranu uživatelských zařízení a souborů

> [!NOTE]
> Pokud nastavíte zásady a zařízení Office 365 MDM, budou tato zařízení uvedená na stránce **zařízení** v centru pro správu systému Microsoft 365. Všechny vámi nastavené zásady se zobrazí v seznamu klasických zásad na [portálu Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Po přiřazení licencí k Microsoft 365 Business Premium můžete začít chránit zařízení a soubory uživatelů.

Pokud jste všichni v organizaci upgradovali na Microsoft 365 Business Premium, uvidíte Průvodce nastavením na domovské stránce a může se řídit [nastavením Microsoft 365 Business Premium v Průvodci nastavením](set-up.md) , abyste chránili soubory a mobilní zařízení.

Tyto kroky můžete provést taky na stránce zařízení:
  
1. V centru pro správu přejděte v levém navigačním podokně na **Devices** \> **zásady** zařízení.
    
2. Na stránce **zásady zařízení** zvolte **Přidat**.
    
3. V podokně **Přidat zásady** udělte dané zásadě název a v rozevíracím seznamu vyberte **Typ zásady** . 
    
     Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních s Androidem a iPhone a Windows 10 a nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností. Podrobnosti najdete v následujících odkazech:
    
  - [Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem](app-protection-settings-for-android-and-ios.md)
    
  - [Nastavení ochrany aplikací pro zařízení s Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [Nastavení ochrany zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:
    
  - Postupy pro zařízení s Windows najdete v tématu [nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md) . 
    
  - Postup [nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md) pro telefony s Androidem a iPhone. 
  
### <a name="mailbox-size"></a>Velikost poštovní schránky

Microsoft 365 Business Premium má limit úložiště 50 GB, protože používá Exchange Online (plán 1). Pokud některý z uživatelů přesáhne 50 GB úložiště poštovních schránek, doporučuje se při přechodu na Microsoft 365 Business Premium přiřadit tomuto uživateli tento uživatel: Exchange Online (plán 2) a odebrat plán 1 služby Exchange Online.


### <a name="threat-protection"></a>Ochrana před hrozbami

Po migraci na Microsoft 365 Business Premium máte k dispozici program Defender pro Office 365. Další informace najdete v článku [Microsoft Defender pro Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) . Nastavení, viz [Nastavení bezpečných odkazů](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [Nastavení bezpečných příloh](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)a [nastavení ochrany proti podvodným zprávám v programu Defender pro Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Štítky utajení

Pokud chcete začít používat popisky citlivosti, přečtěte si článek Přehled popisů [citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) a [vytváření a Správa popisků](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) pro video.
