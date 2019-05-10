---
title: Nastavení Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Zjistěte, jak nastavit Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660743"
---
# <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

Před započetím práce, podrobnosti najdete v části [Získat obchodní 365 Microsoft](get-microsoft-365-business.md) zápisu.

Podívejte se na [krátké video návod, jak nastavit Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) pomocí nastavení průvodce, a pokud nemáte služby Active Directory v prostorách
  

## <a name="overview"></a>Přehled

Většina nastavení kroky lze provést v Průvodci instalací, ale jsou také uvedeny další možnosti.

1. [Přidat do domény](#add-your-domain-to-personalize-sign-in) (Pokud jste si koupili své domény při [přihlášení](sign-up.md), tento krok je již proveden.)
2. Přidáte uživatele. Lze provést třemi způsoby:
    - Podle pokynů [Průvodce instalací](#add-users-in-the-wizard).
    - Používá pro synchronizaci adresářů přidat [uživatele Azure AD připojit pomocí](#add-users-by-using-azure-ad-connect) služby Active directory v prostorách.
    - Můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.
3. Nastavit zásady zabezpečení a konfigurace zařízení. Lze provést třemi způsoby:
    - Podle pokynů [Průvodce instalací](#set-up-policies-in-the-wizard).  
    - V [Centru správy](#modify-or-add-policies-in-the-admin-center).
    - V aplikaci [Centrum pro správu Intune](https://docs.microsoft.com/intune/what-is-device-management).
4. Nastavit a spravovat zařízení v systému Windows 10.

    Při připojení zařízení WIndows 10 k Azure AD získat k němu použity všechny zásady.
    - Nastavení konfigurace zařízení Windows 10 podle pokynů [Průvodce instalací](#set-up-policies-in-the-wizard).
    - [Nové Windows 10 zařízení](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) připojte k Azure AD.
    - Připojte [existující zařízení s Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) k Azure AD.
1. Instalace Office 365 Business.
    - Office v zařízení Windows může automaticky instalovat pomocí [Průvodce instalací](#set-up-policies-in-the-wizard).
    - Automaticky [nainstalovat systém Office](auto-install-or-uninstall-office.md) z středisku pro správce.
    - Umožní uživatelům [instalaci aplikací sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.
     
1. Nastavte další zabezpečení.
    - Průvodce instalací přidá zásady zabezpečení vašeho zařízení, ale můžete také využít výhod [Další bezpečnostní](#additional-security-settings) funkce, které umožňuje zabezpečené vaše data, účty a e-mailů. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatele a nastavení zásad

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Při koupi Microsoft 365 Business, máte možnost použít doménu vlastníte, nebo při nákupu [zápisu](sign-up.md).

- Pokud jste zakoupili novou doménu při registraci, vaše doména je sada všech nahoru a můžete přesunout, chcete-li [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání přizpůsobit přihlašovací domény

1. Přihlášení k aplikaci [Microsoft 365 admin center](https://admin.microsoft.com) pomocí globální správce pověření. 

2. Vyberte **Přidat do domény** , spusťte průvodce.

    ![Vyberte Přidat do domény.](media/addadomainadmincenter.png)
    
3. V průvodci zadejte název domény, který chcete použít (například contoso.com).


    ![Obrazovka přizpůsobit přihlašovací stránku.](media/personalizesignin.png)

    
4. Postupujte podle kroků v průvodci [vytvořit DNS záznamy na jakékoliv DNS poskytovatele hostitelských služeb pro Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ověří, že jste vlastníkem domény. Pokud víte, váš hostitel domény naleznete v tématu [zvláštní pokyny pro hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud svého poskytovatele hostingových služeb, GoDaddy, proces je jednoduchý a vás automaticky vyzve k přihlášení a ověření za vás společnost Microsoft:

    ![Na stránce potvrdit přístup GoDaddy vyberte ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

V průvodci můžete přidat uživatele, ale můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce. Navíc pokud máte místní řadič domény, můžete přidat uživatele [Azure AD připojit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>V průvodci Přidat uživatele

Všichni uživatelé, které zadáte v průvodci získáte automaticky přiřazena licence Microsoft 365 Business.
Pokud máte místní řadič domény a používáte služby Active Directory, naleznete v článku [ddd uživatelů pomocí Azure AD připojit](#add-users-by-using-azure-ad-connect).

![Obrazovka stránku přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. Pokud vaše předplatné Microsoft 365 Business již uživatele má (například pokud jste použili službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní. Neváhejte a přidejte licence i jim.

3. Po přidání uživatele se zobrazí také možnost sdílet pověření s novým uživatelům, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

4. Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**. 

    Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Přidání uživatele pomocí Azure AD Connect

 Pokud máte místní řadič domény se službou Active Directory, synchronizovat pomocí [Azure AD připojit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)uživatelé s Microsoft 365 Business. Dokončete tuto před spuštěním Průvodce instalací. Si můžete stáhnout v Centru pro správu:

- Přejděte na **uživatele** \> **aktivních uživatelů**vyberte na tři tečky v horní části stránky a potom vyberte **adresář synchronizace** Azure AD připojit stáhnout.

    ![Na stránce aktivní uživatele vyberte elipsy > adresář snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Pokud uživatelé vytvářet tímto způsobem, musíte stále k nim přiřadit licence ve středisku pro správce.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Získat přístup k doméně aplikace a zařízení

Pokud chcete získat přístup k doméně aplikace a zařízení, přečtěte si dva jiný způsob povolení, které v následujících článcích:
  
- [Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business](manage-windows-devices.md)
    - Toto je doporučený způsob.

- [Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud používáte domény .onmicrosoft nebo lze nastavit uživatele Azure AD připojit, nezobrazí se tento krok.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, můžete ke správě DNS záznamů a ujistěte se, že zachovat stávající služby připojení. Viz [základní informace o doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) pro další informace.

        ![Připojit domény stránky lze spravovat vlastní záznamy DNS.](media/connectyourdomainpage.png)

2. Postupujte podle pokynů v průvodci a e-mailů a dalších služeb bude nastavení pro vás.

### <a name="set-up-security-policies-and-device-configurations"></a>Nastavit zásady zabezpečení a konfigurace zařízení 

Tyto zásady se týkají všech uživatelů udělíte licenci nebo na skupinu uživatelů a pokud se rozhodnete přiřadit různé zásady pro více uživatelů.

#### <a name="set-up-policies-in-the-wizard"></a>Nastavení zásad v Průvodci

Zásady, které jste nastavili v Průvodci automaticky použity [skupiny zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*.

1. **Ochranu pracovních souborů na mobilních zařízeních** možnost **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** je zapnutá ve výchozím nastavení. Máte možnost zapnout **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních**, a to je doporučeno.

    ![Snímek obrazovky chránit pracovní soubory na stránce Mobilní zařízení.](media/protectworkfilesondevices.png)

     - Jestliže rozbalíte **chránit pracovní soubory, pokud jsou ztráty nebo krádeže zařízení**, jsou vybrány [výchozí hodnoty](protect-work-files-on-lost-or-stolen-device.md) :

        ![Obrazovka výchozí hodnoty pro ochranu souborů na ztracené zařízení.](media/protectworkfilesondevicesdefault.png)

    - Pokud vyberete **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních** a rozbalte ji, [výchozí hodnoty](manage-user-access-on-mobile-devices.md) jsou zobrazeny. Doporučujeme vám přijmou během instalace výchozí hodnoty, abyste vytvořili zásady aplikací pro Android, iOS a Windows 10, které platí pro všechny uživatele. Další zásady můžete vytvořit po dokončení instalace.

        ![Obrazovka nastavení ochrany souborů sady Office Mobile.](media/useraccessonmobile.png)

2. Poslední krok na ochranu dat a zařízení umožňuje nastavit zásady zabezpečení Windows 10 zařízení. Toto nastavení automaticky použito při připojení uživatele v systému Windows 10 pro vaši organizaci. Můžete rozbalit **zabezpečení Windows 10 zařízení** zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).
3. Můžete také [automaticky nainstalovat systém Office](install-office-on-windows-10-during-setup.md) na zařízení Windows 10.

    ![Obrazovka nastavení stránku konfigurace zařízení Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Úprava nebo přidání zásady v Centru pro správu

Pro odkazy na témata týkající se zobrazení a úprava ochrany zařízení a aplikace zásady, naleznete v tématu [Správa Microsoft 365 Business](manage.md) a jak odstranit nebo obnovit uživatelská zařízení.

## <a name="deploy-and-manage-windows-10"></a>Nasazení a správa Windows 10
V tématu Ruční připojení k Azure AD, buď při instalaci nových počítačů nebo změnou přihlašovacího profilu pro stávající počítače [Nastavení systému Windows zařízení pro uživatele Microsoft 365 Business](set-up-windows-devices.md) . 

### <a name="use-autopilot-to-set-up-new-devices"></a>Chcete-li nastavit nové zařízení pomocí Autopilot

[Autopilot systému Windows](add-autopilot-devices-and-profile.md) lze nakonfigurovat automaticky **Nová** zařízení Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který lze provést za vás. Můžete také přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) a zeptejte se odborníků cloud technologie nastavit nová zařízení, které zakoupíte, vám.

### <a name="access-on-premises-resources"></a>Přístup k místním prostředkům

Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních. Postupujte podle kroků v [doméně zařízení Windows 10, které jsou spravovány Microsoft 365 Business povolit](manage-windows-devices.md) toto nastavení. Toto je upřednostňovaný způsob a zařízení v tomto stavu se nazývají hybridní Azure AD připojené zařízení.

Pokud váš podnik má místní služby Active Directory, která obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete přidělit přístup Azure AD připojené zařízení tyto prostředky podle pokynů zde: [přístup místního zdroje z Azure AD připojené zařízení Microsoft 365 Business](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Nasazení aplikace klienta služeb Office 365

Pokud zvolíte automaticky nainstalovat Office apps v průběhu sada nahoru, nainstaluje soubor apps po uživatelé přihlášeni k Azure AD ze svých zařízení systému Windows pomocí pověření jejich práce na zařízení Windows 10.
Chcete-li nainstalovat systém Office na mobilním iOS nebo Android zařízení, naleznete v tématu [nastavit mobilní zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).

Office lze také nainstalovat samostatně. Viz pokyny pro [instalaci sady Office na PC nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .

## <a name="additional-security-settings"></a>Další nastavení zabezpečení

Kromě zabezpečení a kompatibility nastavení v Průvodci instalací můžete také nastavit další parametry:
  
- **E-mailová ochrana proti malwaru**
- **Bezpečné přílohy Advanced Threat Protection (ATP)**
- **ATP bezpečné propojení**
- **VÝSTIŽNÝ anti-phishing**
- **Exchange Online - archiv**
- **Zabránění ztrátě dat (DLP)**
- **Ochrana údajů v Azure** (Plán 1)
- **Dostupnost portálu Intune**

Chcete-li získat spuštění naleznete v tématu [nastavení zásad pokročilé zabezpečení](set-up-advanced-security.md).

Další informace naleznete v tématu [horní 10 způsobů, jak zabezpečit váš podnik 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro přehled osvědčených postupů zabezpečení.