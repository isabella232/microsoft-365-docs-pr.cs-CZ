---
title: Nastavení Microsoft 365 Business Premium
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Podívejte se na postup nastavení Microsoft 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších možností.
ms.openlocfilehash: 74a98e915577cf86ec32a706bd3b8f558f49db95
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227633"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Nastavení Microsoft 365 Business Premium v průvodci nastavením

## <a name="watch-overview-of-microsoft-365-setup"></a>Přehrát: Přehled Microsoft 365 nastavení

V tomto videu najdete přehled Microsoft 365 Business Premium nastavení.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

Když si Microsoft 365 Business Premium, máte možnost používat doménu, kterou vlastníte, nebo si ji koupit během [registrace](sign-up.md).

- Pokud jste si při přihlášení koupili novou doménu, vaše doména je nastavená a můžete přejít na Přidat uživatele a [přiřadit licence.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény k přizpůsobení přihlášení

1. Přihlaste se [k Centrum pro správu Microsoftu 365](https://admin.microsoft.com) pomocí přihlašovacích údajů globálního správce. 

2. Průvodce **spustíte tak,** že zvolíte Přejít na nastavení.

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. Na **stránce Instalace Office aplikací** můžete volitelně nainstalovat aplikace na svůj vlastní počítač.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).

    > [!IMPORTANT]
    > Pokud jste si doménu koupili během registrace, neuvidíte tady krok **Přidat** doménu. Přejděte místo [toho na Přidat](#add-users-and-assign-licenses) uživatele.

    ![Snímek obrazovky s přizpůsobením přihlašovací stránky](../media/adddomain.png)

    
4. Podle pokynů v průvodci vytvořte záznamy DNS u [libovolného](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) poskytovatele hostingu DNS Microsoft 365, který ověří, že doménu vlastníte. Pokud znáte hostitele domény, podívejte se taky na přidání [domény do Microsoft 365](/microsoft-365/admin/setup/add-domain).

    Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiným hostitelem povoleným s připojením domény [,](/office365/admin/get-help-with-domains/domain-connect)proces je snadný a automaticky se zobrazí dotaz, jestli se chcete přihlásit a nechat Microsoft ověřit vaším jménem.

    ![Na stránce GoDaddy Confirm Access (Potvrdit přístup GoDaddy) vyberte Authorize (Autorizovat).](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Uživatele můžete přidat v průvodci, ale můžete je přidat [i později](../admin/add-users/add-users.md) v Centru pro správu. Pokud máte místní řadič domény, můžete přidat uživatele s [Azure AD Připojení](/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v průvodci

Uživatelům, které přidáte v průvodci, se automaticky přiřadí Microsoft 365 Business Premium licence.

![Snímek obrazovky se stránkou Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. Pokud vaše Microsoft 365 Business Premium předplatné má stávající uživatele (například pokud jste použili Azure AD Připojení), můžete jim teď přiřadit licence. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů získáte taky možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu .onmicrosoft nebo jste k nastavení uživatelů použili Azure AD Připojení, tento krok se vám zobrazí.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, změňte názvové servery tak, aby [Microsoft 365 u jakéhokoli doménového registrátora](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md). 

    - Pokud máte existující záznamy DNS, například existující web, ale váš hostitel DNS je povolený pro připojení domény [,](/office365/admin/get-help-with-domains/domain-connect)zvolte Přidat záznamy **za mě**. Na stránce **Zvolte online služby** přijměte všechna výchozí nastavení a  zvolte Další a na stránce hostitele DNS zvolte Autorizovat. 
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povolené pro připojení domény), budete chtít spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojené. Další [informace najdete v tématu Základy](/office365/admin/get-help-with-domains/dns-basics) domény.

        ![Stránka Aktivace záznamů](../media/activaterecords.png)

2. Postupujte podle pokynů v průvodci a budete mít nastavené e-maily a další služby.

### <a name="protect-your-organization"></a>Ochrana vaší organizace 

Zásady, které nastavíte v průvodci, se automaticky použijí ve skupině [Zabezpečení](/office365/admin/create-groups/compare-groups#security-groups) s *názvem Všichni uživatelé*. V Centru pro správu můžete taky vytvořit další skupiny, ke které chcete přiřadit zásady.

1. V části Zvýšení ochrany **před** pokročilými kybernetickými hrozbami doporučujeme přijmout výchozí nastavení, abyste v aplikacích Office 365 [advance threat protection](../security/office-365-security/defender-for-office-365.md) prohledaly soubory Office odkazy.

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. Na stránce Prevent **leaks of** sensitive data (Zabránit úniku citlivých dat) přijměte výchozí nastavení pro zapnutí ochrany před únikem dat (DLP) pro sledování citlivých dat v aplikacích Office 365 Office zabránění jejich náhodnému sdílení mimo vaši organizaci.

3. Na stránce **Zamknout data v Office pro mobilní** zařízení nechte správu mobilních aplikací zak dispozici, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit zásady správy **mobilních aplikací**.

    ![Snímek obrazovky s zamknout data v Office pro mobilní stránku](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečené Windows 10 počítače

V levém navigačním panelu **vyberte** Nastavení a potom v části Přihlášení a **zabezpečení** zvolte Zabezpečit **Windows 10 počítače**. Pokud **chcete začít,** zvolte Zobrazení. Úplné [pokyny najdete v Windows 10 zabezpečení počítačů.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Nasazení Office 365 klientských aplikací

Pokud jste se při nastavování rozhodli automaticky instalovat aplikace Office, aplikace se nainstalují na zařízeních Windows 10, jakmile se uživatelé k Azure AD přihlásili ze svých Windows zařízení pomocí svých pracovních přihlašovacích údajů.

Informace o Office na mobilních zařízeních s iOSem nebo Androidem najdete v tématu Nastavení mobilních zařízení [pro Microsoft 365 Business Premium uživatele](set-up-mobile-devices.md).

Můžete také nainstalovat Office jednotlivě. Pokyny [najdete v Office instalace na PC nebo Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="related-content"></a>Související obsah

[Microsoft 365 pro firemní školicí videa](../business-video/index.yml) (stránka odkazu)
