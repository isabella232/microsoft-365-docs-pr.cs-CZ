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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přečtěte si postup nastavení pro Microsoft 365 Business, od přihlášení k odběru, přes přidání domény a uživatelů až po nastavení zásad zabezpečení a další.
ms.openlocfilehash: 4c9c3ee4c45625cebe5d19eb03fcb6d90eb9243e
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415559"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Podívejte se na krátké video o nastavení Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Většinu kroků nastavení lze provést v průvodci nastavením, ale jsou uvedeny i další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (pokud jste si zakoupili doménu během [registrace](sign-up.md), tento krok je již hotový.)

    - **Přidejte uživatele**. Uživatele můžete přidat libovolným ze tří způsobů:
        - V [průvodci](set-up.md#add-users-in-the-wizard).
        - Synchronizace adresářů slouží k [přidání uživatelů pomocí azure ad connect,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) pokud máte místní adresář Active.
        - Uživatele můžete přidat [i později](add-users-m365b.md) v Centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Nastavení zásad zabezpečení a konfigurace zařízení 

  - Průvodce [instalací](set-up.md#protect-your-organization) slouží ke konfiguraci zásad zařízení. 
  - Další možnosti můžete přidat nebo upravit později v [Centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Průvodce instalací také nastaví základní nastavení ochrany před hrozbami a zabránění ztráty dat.
  
  Kromě nastavení zabezpečení v průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:

- **E-mailová ochrana proti malwaru**
- **Ochrana proti phishingu atp**
- **Exchange Online - archiv**
- **Ochrana informací Azure (Plan1**)

Chcete-li začít, přečtěte si [příklady zvýšení ochrany před hrozbami](increase-threat-protection.md) a [nastavení funkcí dodržování předpisů](set-up-compliance.md).

Plán osvědčených postupů zabezpečení najdete také [v 10 nejlepších způsobech zabezpečení microsoft365 firmy.](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data)

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa zařízení s Windows 10

Po spuštění průvodce nastavením budete chtít proctect všechny Windwos 10 počítačů ve vaší organizaci.
  
- Windows 10 Pro je [předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale pokud máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné vás opravňuje k [upgradu na Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Podle pokynů v [zabezpečených počítačích s Windows 10](secure-win-10-pcs.md) nastavte zásady pro zařízení s Windows 10.

Když připojíte zařízení s Windows 10 k Azure AD, zásady, které nastavíte pro počítače s Windows 10, se na něj použijí. Další informace naleznete v tématu [Nastavení zařízení se systémem Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Krok 4: Instalace Office 365 Business
- Office můžete do zařízení se systémem Windows nainstalovat automaticky pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).
- Upřete uživatelům [instalaci aplikací Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro Windows a zařízení.
     
## <a name="advanced"></a>Pokročilé
- **Nastavení nových zařízení pomocí autopilota**
            
     Pomocí [automatického pilotního projektu systému Windows](add-autopilot-devices-and-profile.md) můžete automaticky předkonfigurovat **nová** zařízení s Windows 10 pro uživatele, ale může být jednodušší získat [partnera,](https://www.microsoft.com/solution-providers/search) který to může udělat za vás. Můžete také přejít do [Obchodu Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na cloudové technologie o nastavení nových zařízení, která si koupíte.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business k ochraně zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Podle pokynů v [části Povolit zařízení windows 10 připojená k doméně, která má spravovat Microsoft 365 Business,](manage-windows-devices.md) a nastavte tak to. Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají hybridní zařízení připojená k Azure AD.

    - Pokud má vaše firma místní službu Active Directory, která obsahuje některé místní prostředky (například sdílené složky a tiskárny), můžete k těmto prostředkům přistupovat k těmto prostředkům se službou Azure AD podle kroků: [Přístup k místním prostředkům ze zařízení se službou Azure AD v Microsoft365 Business](access-resources.md).

## <a name="see-also"></a>Viz také

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
