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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přehled kroků nastavení pro aplikaci Microsoft 365 Business.
ms.openlocfilehash: 425c465262c266ca764ae8c7a52130903fa635a5
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "39812772"
---
# <a name="overview-of-setup"></a>Přehled nastavení

Většinu kroků nastavení lze provést v Průvodci nastavením, ale jsou zde také uvedeny další možnosti.

## <a name="step-1-add-your-domain-and-users"></a>Krok 1: Přidání domény a uživatelů

   - **[Přidejte svou doménu](set-up.md#add-your-domain-to-personalize-sign-in)** (Pokud jste během [přihlášení](sign-up.md)koupili doménu, je tento krok již vykonáno.)

    - **Přidejte uživatele**. Uživatele můžete přidat některým ze tří způsobů:
        - V [Průvodci](set-up.md#add-users-in-the-wizard).
        - Chcete-li [Přidat uživatele pomocí funkce Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) (v prostorách služby Active Directory), použijte synchronizaci adresářů.
        - Uživatele můžete také [přidat později](add-users-m365b.md) v centru pro správu.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Krok 2: nastavení zásad zabezpečení a konfigurace zařízení 

  - Pomocí [Průvodce instalací](set-up.md#protect-your-organization) nakonfigurujte zásady zařízení. 
  - Můžete je také přidat nebo upravit později v [centru pro správu](view-policies-and-devices.md) a na [portálu Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Průvodce instalací také nastaví základní ochranu proti ohrožení a nastavení prevence ztráty dat.
  
  Kromě nastavení zabezpečení v Průvodci nastavením můžete zvýšit zabezpečení přidáním následujících nastavení:

      - **Ochrana proti malwaru e-mailu**
      - **ATP anti-phishing**
      - **Exchange Online - archiv**
      - **Ochrana informací Azure (Plan1**)

          Chcete-li se začít podívat, [nastavte pokročilé zásady zabezpečení](set-up-advanced-security.md).

        Viz také [10 nejlepších způsobů zabezpečení společnosti Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro cestovní mapu s nejlepšími bezpečnostními postupy.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Krok 3: nastavení a Správa zařízení systému Windows 10

Po spuštění Průvodce nastavením budete chtít v organizaci proctit všechny počítače společnosti Windwos 10.
  
- Systém Windows 10 pro je [nezbytným předpokladem](pre-requisites-for-data-protection.md) pro Microsoft 365 Business, ale pokud používáte systém Windows 7 pro, Windows 8 pro nebo Windows 8,1 pro, vaše předplatné vás opravňuje k [inovaci na systém Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Chcete-li nastavit zásady pro zařízení systému Windows 10, postupujte podle kroků v [zabezpečených počítačích se systémem Windows 10](secure-win-10-pcs.md) .

Připojíte-li zařízení se systémem Windows 10 k Azure AD, budou na něj použity zásady nastavené pro počítače se systémem Windows 10. Další informace naleznete v tématu [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Krok 4: instalace sady Office 365 Business
- Sadu Office lze automaticky nainstalovat do zařízení systému Windows pomocí [Průvodce instalací](set-up.md#deploy-office-365-client-apps).
- Umožňuje uživatelům [instalovat aplikace sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.
     
## <a name="advanced"></a>Pokročilé
- **Použití automatického Opilotu k nastavení nových zařízení**
            
     Pomocí [systému Windows autopilot](add-autopilot-devices-and-profile.md) můžete automaticky nakonfigurovat **Nová** zařízení systému Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který by to mohl udělat za vás. Můžete také přejít do [aplikace Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)a požádat odborníka na technologii cloud, aby nastavil nová zařízení, která zakoupíte.

- **Přístup k prostředkům na místě**

     - Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování. Postupujte podle kroků, [které umožňují, aby zařízení systému Windows 10 spojená s doménou byla spravována společností Microsoft 365 Business](manage-windows-devices.md) . Toto je upřednostňovaná metoda a zařízení v tomto stavu se nazývají zařízení spojená s hybridním Azure.

    - Pokud vaše společnost disponuje místním adresářem služby Active Directory obsahujícím některé místní zdroje (například sdílené soubory a tiskárny), můžete k těmto zdrojům poskytnout přístup k těmto prostředkům pomocí zařízení Azure AD, a to následujícím postupem: [přístup k místním prostředkům z zařízení připojeném Azure AD v Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Viz také

[Microsoft 365 Business Training video](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
