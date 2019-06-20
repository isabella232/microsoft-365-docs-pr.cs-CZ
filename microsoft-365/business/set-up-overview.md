---
title: Přehled nastavení
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přehled nastavení kroky pro Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086284"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Většina nastavení kroky lze provést v Průvodci instalací, ale jsou také uvedeny další možnosti.


## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelé

   - **[Přidat do domény](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste si koupili své domény při [přihlášení](sign-up.md), tento krok je již proveden.)

    - **Přidání uživatelů**. Lze provést třemi způsoby:
        - Podle pokynů [Průvodce](set-up.md#add-users-in-the-wizard).
        - Používá pro synchronizaci adresářů přidat [uživatele Azure AD připojit pomocí](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) služby Active directory v prostorách.
        - Můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: Nastavit zásady zabezpečení a konfigurace zařízení 

  - [Průvodce instalací](set-up.md#set-up-security-policies-and-device-configurations) slouží ke konfiguraci zásad zabezpečení a zařízení. 
  - Můžete také přidat více nebo je upravit později v [admin center](view-policies-and-devices.md) a do [Intune portál](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Kromě nastavení zabezpečení v Průvodci instalací můžete zvýšit přidáním následující nastavení zabezpečení:

      - **E-mailová ochrana proti malwaru**
      - **Advanced Threat Protection (ATP) bezpečné propojení**
      - **ATP bezpečné přílohy**
      - **ATP anti-phishing**
      - **Exchange Online - archiv**
      - **Zabránění ztrátě dat (DLP)**
      - **Ochrana informací azure (Plan1**)

          Chcete-li získat spuštění naleznete v tématu [nastavení zásad pokročilé zabezpečení](set-up-advanced-security.md).

        Další informace naleznete v tématu [horní 10 způsobů, jak zabezpečit váš podnik 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro přehled osvědčených postupů zabezpečení.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: Nastavení a správa zařízení v systému Windows 10

   Při připojení zařízení Windows 10 k Azure AD získat k němu použity zásady, které jste vytvořili v [kroku 2](#step-2-set-up-security-policies-and-configure-devices) .

   - Windows 10 Pro je [nutným předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale máte Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro předplatné vás opravňuje k [upgradu na Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - [Průvodce instalací](set-up.md#set-up-security-policies-and-device-configurations) slouží ke konfiguraci zásad pro zařízení Windows 10.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Instalace Office 365 Business
- Office v zařízení Windows může automaticky instalovat pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).
- Automaticky [nainstalovat systém Office](auto-install-or-uninstall-office.md) z středisku pro správce.
- Umožní uživatelům [instalaci aplikací sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.
     
## <a name="advanced"></a>Upřesnit
- **Chcete-li nastavit nové zařízení pomocí Autopilot**
            
     [Autopilot systému Windows](add-autopilot-devices-and-profile.md) lze nakonfigurovat automaticky **Nová** zařízení Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který lze provést za vás. Můžete také přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) a zeptejte se odborníků cloud technologie nastavit nová zařízení, které zakoupíte, vám.

- **Přístup k místním prostředkům**

     - Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních. Postupujte podle kroků v [doméně zařízení Windows 10, které jsou spravovány Microsoft 365 Business povolit](manage-windows-devices.md) toto nastavení. Toto je upřednostňovaný způsob a zařízení v tomto stavu se nazývají hybridní Azure AD připojené zařízení.

    - Pokud váš podnik má místní služby Active Directory, která obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete přidělit přístup Azure AD připojené zařízení tyto prostředky podle pokynů zde: [přístup místního zdroje z Azure AD připojené zařízení Microsoft 365 Business](access-resources.md).

  