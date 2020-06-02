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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Seznamte se s kroky nastavení microsoftu 365 Business Premium, od přihlášení k odběru přes přidání domény a uživatelů až po nastavení zásad zabezpečení a další informace.
ms.openlocfilehash: 4670344263ceb64a32962dfa6eb9c1644e61541d
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470519"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Podívejte se na krátké video o nastavení Microsoftu 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Většinu kroků nastavení lze provést v průvodci instalací, ale jsou uvedeny také další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte svou doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (pokud jste si koupili doménu během [registrace](sign-up.md), tento krok je již hotovo.)

   - **Přidat uživatele**. Uživatele můžete přidat libovolným ze tří způsobů:
        - V [průvodci](set-up.md#add-users-in-the-wizard).
        - Pomocí synchronizace adresářů [můžete přidat uživatele pomocí služby Azure AD Connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) pokud máte místní službu Active Directory.
        - Uživatele můžete přidat také [později](add-users-m365b.md) v Centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Nastavení zásad zabezpečení a konfigurace zařízení 

  - Pomocí [Průvodce instalací](set-up.md#protect-your-organization) nakonfigurujte zásady zařízení. 
  - Další nebo upravit můžete také později v [Centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Průvodce instalací také nastaví základní nastavení ochrany před hrozbami a ztráty dat.
  
  Kromě nastavení zabezpečení v průvodci instalací můžete zvýšit zabezpečení přidáním následujících nastavení:

- **Ochrana proti malwaru e-mailem**
- **Ochrana proti phishingu atp**
- **Exchange Online - archiv**
- **Azure Information Protection (Plán1)**

Chcete-li začít, přečtěte [si přečtěte si informace o zvýšení ochrany před hrozbami](increase-threat-protection.md) a [nastavení funkcí dodržování předpisů](set-up-compliance.md).

Podívejte se také [na 10 nejlepších způsobů, jak zabezpečit Microsoft 365 Business Premium,](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) kde najdete přehled osvědčených postupů v oblasti zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa zařízení s Windows 10

Po spuštění průvodce nastavením budete chtít proctect všechny počítače Windwos 10 ve vaší organizaci.
  
- Windows 10 Pro je [předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business Premium, ale pokud máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné vás opravňuje k [upgradu na Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Podle pokynů v [zabezpečených počítačích s Windows 10](secure-win-10-pcs.md) nastavte zásady pro zařízení s Windows 10.

Když se připojíte k zařízení s Windows 10 k Azure AD, použijí se na něj zásady nastavené pro počítače s Windows 10. Další informace naleznete [v tématu Nastavení zařízení s Windows pro uživatele Microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Krok 4: Instalace aplikací Microsoft 365 pro firmy
- Office můžete automaticky nainstalovat do zařízení se systémem Windows pomocí [průvodce instalací](set-up.md#deploy-office-365-client-apps).
- Umožňuje uživatelům [instalovat aplikace Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro Windows a zařízení.
     
## <a name="advanced"></a>Pokročilé
- **Nastavení nových zařízení pomocí funkce Autopilot**
            
     Pomocí [systému Windows Autopilot](add-autopilot-devices-and-profile.md) můžete automaticky předem nakonfigurovat **nová** zařízení s Windows 10 pro uživatele, ale může být jednodušší získat [partnera,](https://www.microsoft.com/solution-providers/search) který to může udělat za vás. Můžete taky přejít do [Microsoft Storu](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudové technologie, aby nastavil nová zařízení, která si zakoupíte.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Podle pokynů v části [Povolit zařízení s Windows 10 připojená k doméně, která bude spravovat Microsoft 365 Business Premium,](manage-windows-devices.md) nastavte to. Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají hybridní zařízení spojené Azure AD.

    - Pokud má vaše firma místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete zařízením spojeným s Azure AD udělit přístup k těmto prostředkům pomocí kroků: [Přístup k místním prostředkům ze zařízení spojených s Azure AD v Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Viz také

[Školicí videa microsoftu 365 pro firmy](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
