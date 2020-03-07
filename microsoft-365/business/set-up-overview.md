---
title: Přehled nastavení
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přečtěte si kroky nastavení pro Microsoft 365 Business, od přihlášení k odběru, přidání domény a uživatelů, nastavení zásad zabezpečení a další.
ms.openlocfilehash: 9bb536b52981966f6c4c487f8400577b896261e0
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561185"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Podívejte se na krátké video o nastavení Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Většinu kroků nastavení lze provést v průvodci nastavením, ale jsou také uvedeny další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte svou doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (pokud jste si doménu koupili během [registrace](sign-up.md), tento krok je již hotový.)

    - **Přidat uživatele**. Uživatele můžete přidat libovolným ze tří způsobů:
        - V [průvodci](set-up.md#add-users-in-the-wizard).
        - Pomocí synchronizace adresářů [přidejte uživatele pomocí služby Azure AD Connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) pokud máte místní adresář Active.
        - Uživatele můžete [přidat také později](add-users-m365b.md) v Centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Nastavení zásad zabezpečení a konfigurace zařízení 

  - Ke konfiguraci zásad zařízení použijte [Průvodce instalací.](set-up.md#protect-your-organization) 
  - Další můžete taky přidat nebo je později upravit v [Centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Průvodce instalací také nastaví základní nastavení ochrany před hrozbami a zabránění ztrátám dat.
  
  Kromě nastavení zabezpečení v průvodci instalací můžete zvýšit zabezpečení přidáním následujících nastavení:

- **Ochrana proti malwaru e-mailem**
- **Ochrana proti phishingu ATP**
- **Exchange Online - archiv**
- **Azure Information Protection (plán1)**

Chcete-li začít, přečtěte si informace o [zvýšení ochrany před hrozbami](increase-threat-protection.md) a [nastavení funkcí dodržování předpisů](set-up-compliance.md).

Podívejte se také [na 10 nejlepších způsobů zabezpečení microsoftu 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a podívejte se na plán osvědčených postupů zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa zařízení s Windows 10

Po spuštění průvodce nastavením budete chtít proctect všechny Windwos 10 počítačů ve vaší organizaci.
  
- Windows 10 Pro je [předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale pokud máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné vás opravňuje k [upgradu na Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Podle pokynů v [zabezpečeném počítači s Windows 10](secure-win-10-pcs.md) nastavte zásady pro zařízení s Windows 10.

Když se připojíte k zařízení s Windows 10 do Azure AD, použijí se na něj zásady nastavené pro počítače s Windows 10. Další informace naleznete v [tématu Nastavení zařízení s Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Krok 4: Instalace Office 365 Business
- Office můžete automaticky nainstalovat do zařízení s Windows pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).
- [Uchvátíte uživatele, aby si nainstalovali aplikace Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro Windows a zařízení.
     
## <a name="advanced"></a>Pokročilé
- **Nastavení nových zařízení pomocí autopilota**
            
     [Pomocí automatického pilota systému Windows](add-autopilot-devices-and-profile.md) můžete automaticky předem konfigurovat **nová** zařízení s Windows 10 pro uživatele, ale může být jednodušší získat [partnera,](https://www.microsoft.com/solution-providers/search) který to může udělat za vás. Můžete také přejít do [obchodu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudovou technologii, aby nastavil nová zařízení, která si zakoupíte.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá službu Windows Server Active Directory místně, můžete nastavit Microsoft 365 Business tak, aby chránila vaše zařízení s Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle pokynů v [části Povolit, aby zařízení s Windows 10 připojená k doméně byla spravována microsoftem 365 Business,](manage-windows-devices.md) abyste to nastavili. Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají hybridní zařízení azure ad připojená.

    - Pokud vaše firma má místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízení mandatáž Azure AD přístup k těmto prostředkům podle následujících kroků zde: [Přístup k místním prostředkům ze zařízení azure ad připojen k Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Viz také

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
