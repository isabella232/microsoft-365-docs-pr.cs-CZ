---
title: Přehled nastavení
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zjistěte, jak nastavit Microsoft 365 Business Premium, od předplatného až po přidání domény a uživatelů, nastavení zásad zabezpečení a další možnosti.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579928"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Podívejte se na krátké video o nastavení Microsoftu 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Většinu kroků nastavení můžete provést v nastavení s průvodcem, ale jsou uvedené i další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (pokud jste si doménu koupili během [registrace,](sign-up.md)tento krok už je hotový.)

   - **Přidání uživatelů** Uživatele můžete přidat libovolným ze tří způsobů:
        - V [nastavení s průvodcem](set-up.md#add-users-in-the-wizard).
        - Pokud máte místní adresář [Active Directory,](../enterprise/set-up-directory-synchronization.md) můžete pomocí služby Azure AD Connect přidávat uživatele pomocí synchronizace adresářů.
        - Uživatele taky [můžete přidat později](../admin/add-users/add-users.md) v Centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Nastavení zásad zabezpečení a konfigurace zařízení 

  - Pomocí nastavení [s průvodcem](set-up.md#protect-your-organization) nakonfigurujte zásady zařízení. 
  - Můžete je taky přidat nebo upravit později v Centru [pro správu](view-policies-and-devices.md) a na portálu [Intune](/intune/tutorial-walkthrough-intune-portal).
  - Průvodce nastavením taky nastaví základní nastavení ochrany před hrozbami a ochrany před únikem dat.
  
  Kromě nastavení zabezpečení v průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:

- **Ochrana proti malwaru v e-mailu**
- **Anti-phishing v Defenderu pro Office 365**
- **Exchange Online - archiv**
- **Azure Information Protection (Plán1)**

Pokud chcete začít, podívejte se na zvýšení [ochrany před hrozbou](increase-threat-protection.md) a [nastavení funkcí dodržování předpisů](set-up-compliance.md).

Podívejte se také na 10 nejlepších způsobů, jak zabezpečit [Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) a zmapovat osvědčené postupy zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa zařízení s Windows 10

Po dokončení nastavení s průvodcem budete chtít chránit všechny počítače s Windows 10 ve vaší organizaci.
  
- Windows 10 Pro [](pre-requisites-for-data-protection.md) je předpokladem pro Microsoft 365 Business Premium, ale pokud máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné vás opravňuje k upgradu na [Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).
- Postupujte podle pokynů v [zabezpečených počítačích s Windows 10](secure-win-10-pcs.md) a nastavte zásady pro zařízení s Windows 10.

Když připojíte zařízení s Windows 10 k Azure AD, použijí se na něj zásady nastavené pro počítače s Windows 10. Další informace najdete v tématu [Nastavení zařízení s Windows pro uživatele Microsoftu 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4: Instalace aplikací Microsoft 365 pro firmy
- Office můžete automaticky nainstalovat na zařízení s Windows pomocí průvodce [nastavením](set-up.md#deploy-office-365-client-apps).
- Uživatelé [instalujte aplikace Office pro](/office365/admin/setup/install-applications) Windows a zařízení.
     
## <a name="advanced"></a>Upřesnit
- **Nastavení nových zařízení pomocí Autopilota**
            
     Pomocí Windows [Autopilota](add-autopilot-devices-and-profile.md) můžete automaticky předkonfigurovat nová zařízení **s** Windows 10 [](https://www.microsoft.com/solution-providers/search) pro uživatele, ale může být jednodušší získat partnera, který to může udělat za vás. Můžete taky přejít do [Microsoft Storu](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudovou technologii, aby nastavil nová zařízení, která si koupíte.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránil vaše zařízení s Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle pokynů v článku Povolení spravování zařízení s Windows 10 připojených k doméně [microsoftem 365 Business Premium.](manage-windows-devices.md) Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají zařízení připojená k Hybridní službě Azure AD.

    - Pokud má vaše firma místní adresář Active Directory, který obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízením připojeným k Azure AD dát přístup k těmto prostředkům podle pokynů tady: Přístup k místním prostředkům ze zařízení připojeného k Azure AD v [Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Viz také

[Školicí videa k Microsoftu 365 pro firmy](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)