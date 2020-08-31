---
title: Základní informace o nastavení
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Přečtěte si informace o krocích nastavení Microsoft 365 Business Premium, o přihlašování, přidání domény a uživatelů, o nastavení zásad zabezpečení a dalších.
ms.openlocfilehash: fa9c02fa9546437c83b9cc6c1f1e6e0d723ec868
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306463"
---
# <a name="overview-of-setup"></a>Základní informace o nastavení

Podívejte se na krátké video o nastavení Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Většinu kroků nastavení je možné provést v Průvodci nastavením, jsou však uvedené i další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidání domény](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste si svoji doménu koupili při [registraci](sign-up.md), je tento krok již proveden.)

   - **Přidejte uživatele**. Uživatele můžete přidat některým ze tří způsobů:
        - V [Průvodci](set-up.md#add-users-in-the-wizard).
        - Pokud máte místní službu Active Directory, můžete pomocí synchronizace adresářů [Přidat uživatele pomocí služby Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .
        - [Uživatele můžete přidat taky později](add-users-m365b.md) v centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: nastavení zásad zabezpečení a konfigurace zařízení 

  - K nastavení zásad zařízení použijte [Průvodce nastavením](set-up.md#protect-your-organization) . 
  - Můžete taky přidat další nebo upravit později v [centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Průvodce nastavením také nastaví základní nastavení ochrany před útoky na ohrožení a ztrátu dat.
  
  Kromě nastavení zabezpečení v Průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:

- **Ochrana proti malwaru e-mailu**
- **ATP anti-phishing**
- **Exchange Online - archiv**
- **Azure Information Protection (Plan1**)

Chcete-li začít, přečtěte si téma [zvýšení ochrany před hrozbami](increase-threat-protection.md) a [Nastavení funkcí dodržování předpisů](set-up-compliance.md).

Další informace najdete v článku o [10 způsobech zabezpečení služby Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro účely přehledu nejlepších postupů zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: nastavení a Správa zařízení s Windows 10

Po spuštění Průvodce nastavením si budete chtít proctect všechny počítače Windwos 10 ve vaší organizaci.
  
- Windows 10 pro je [předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business Premium, ale pokud máte Windows 7 pro, Windows 8 pro nebo Windows 8,1 pro, vaše předplatné vás opravňuje k [upgradu na Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Pokud chcete nastavit zásady pro zařízení s Windows 10, postupujte podle kroků v části [zabezpečení počítačů s Windows 10](secure-win-10-pcs.md) .

Když se připojíte k zařízení s Windows 10 ke službě Azure AD, uplatní se na ně zásady nastavené pro počítače s Windows 10. Další informace najdete v tématu [nastavení zařízení s Windows pro uživatele Microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4: instalace aplikací Microsoft 365 pro firmy
- Office můžete automaticky nainstalovat na zařízení s Windows pomocí [Průvodce nastavením](set-up.md#deploy-office-365-client-apps).
- Umožněte uživatelům [nainstalovat aplikace Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro Windows a zařízení.
     
## <a name="advanced"></a>Moderní
- **Nastavení nových zařízení pomocí autopilotního nasazení**
            
     Pomocí automatického [pilotního nasazení systému Windows](add-autopilot-devices-and-profile.md) můžete automaticky předkonfigurovat **Nová** zařízení s Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který to může udělat za vás. Můžete také přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudovou technologii o nastavení nově zakoupených zařízení.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá místní službu Active Directory serveru Windows, můžete nastavit ochranu zařízení s Windows 10 pomocí Microsoft 365 Business Premium, která bude pořád používat místní ověřování. Podle pokynů v tématu [Povolení zařízení s Windows 10 připojeným k doméně, která se budou spravovat přes Microsoft 365 Business Premium](manage-windows-devices.md) . Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají hybridní zařízení připojení Azure AD.

    - Pokud má vaše firma místní adresář služby Active Directory, který obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete svým postupům udělit přístup k těmto zdrojům prostřednictvím služby Azure AD – spojené s použitím následujících kroků: [přístup k místním prostředkům ze zařízení Azure AD-připojeno v Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Viz také

[Školicí kurzy pro Microsoft 365 for Business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
