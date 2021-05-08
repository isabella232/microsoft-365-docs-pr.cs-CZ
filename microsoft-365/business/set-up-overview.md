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
description: Zjistěte, jak nastavit Microsoft 365 Business Premium, od přihlášení k odběru, přidání domény a uživatelů, k nastavení zásad zabezpečení a dalších.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245058"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Podívejte se na krátké video o Microsoft 365 Business Premium nastavení.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](../business-video/index.yml).

Většinu kroků nastavení můžete provést v nastavení s průvodcem, ale jsou uvedené i další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (pokud jste si doménu koupili během [registrace,](sign-up.md)tento krok už je hotový.)

   - **Přidání uživatelů** Uživatele můžete přidat libovolným ze tří způsobů:
        - V [nastavení s průvodcem](set-up.md#add-users-in-the-wizard).
        - Pomocí synchronizace adresářů [můžete přidat uživatele pomocí služby Azure AD Připojení,](../enterprise/set-up-directory-synchronization.md) pokud máte místní adresář Active.
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

Podívejte se [také na 10](/office365/admin/security-and-compliance/secure-your-business-data) nejlepších způsobů zabezpečení Microsoft 365 Business Premium a podívejte se na mapu osvědčených postupů zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa Windows 10 zařízení

Po dokončení nastavení s průvodcem budete chtít chránit všechny Windows 10 počítače ve vaší organizaci.
  
- Windows 10 Pro je předpokladem [](pre-requisites-for-data-protection.md) pro Microsoft 365 Business Premium, ale pokud máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné vás opravňuje k [upgradu](./upgrade-to-windows-pro-creators-update.md)na Windows 10 Pro .
- Postupujte podle pokynů v [zabezpečených Windows 10 počítačů a](secure-win-10-pcs.md) nastavte zásady pro Windows 10 zařízení.

Když se připojíte k Windows 10 Azure AD, použijí se na něj zásady nastavené pro Windows 10 počítače. Další informace najdete v tématu [Nastavení Windows zařízení pro Microsoft 365 uživatele](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4: Instalace Microsoft 365 Apps pro firmy
- Pomocí průvodce nastavením Office automaticky nainstalovat Windows zařízení. [](set-up.md#deploy-office-365-client-apps)
- Dejte [uživatelům Office aplikace pro](/office365/admin/setup/install-applications) Windows a zařízení.
     
## <a name="advanced"></a>Upřesnit
- **Nastavení nových zařízení pomocí Autopilota**
            
     Pomocí Windows [Autopilota](add-autopilot-devices-and-profile.md) můžete automaticky předkonfigurovat nová **Windows 10** zařízení pro uživatele, ale může [](https://www.microsoft.com/solution-providers/search) být jednodušší získat partnera, který to může udělat za vás. Můžete taky přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudovou technologii, aby nastavil nová zařízení, která si koupíte.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránil vaše zařízení Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Podle pokynů v [části](manage-windows-devices.md) Povolení Windows 10 zařízení připojených k doméně Microsoft 365 Business Premium tuto možnost nastavit. Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají zařízení připojená k Hybridní službě Azure AD.

    - Pokud má vaše firma místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízením připojeným k Azure AD dát přístup k těmto prostředkům podle pokynů tady: Přístup k místním prostředkům ze zařízení připojeného k [Azure AD](access-resources.md)v Microsoft 365 Business Premium .

## <a name="related-content"></a>Související obsah

[Microsoft 365 pro firemní školicí videa](../business-video/index.yml) (stránka odkazu)