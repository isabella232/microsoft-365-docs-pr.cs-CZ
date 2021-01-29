---
title: Nastavení Microsoft 365 Business Premium
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
description: Zjistěte, jak nastavit Microsoft 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších možností.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044724"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Nastavení Microsoft 365 Business Premium v průvodci nastavením

V tomto videu najdete přehled nastavení Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

Při nákupu Microsoftu 365 Business Premium máte možnost používat doménu, kterou vlastníte, nebo si ji zakoupit během [registrace.](sign-up.md)

- Pokud jste si koupili novou doménu, je vaše doména nastavená a můžete přejít na Přidat uživatele a přiřadit [licence.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény pro přizpůsobení přihlašování

1. Přihlaste se do Centra pro [správu Microsoftu 365](https://admin.microsoft.com) pomocí svých přihlašovacích údajů globálního správce. 

2. Průvodce **spustíte tak,** že zvolíte Přejít do nastavení.

    ![Vyberte Přejít do nastavení.](../media/gotosetupinadmincenter.png)

3. Na stránce **Instalace aplikací Office** si můžete volitelně nainstalovat aplikace na vlastní počítač.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (třeba contoso.com).

    > [!IMPORTANT]
    > Pokud jste si koupili doménu během registrace, neuvidíte **tady** krok Přidat doménu. Místo toho [přejděte na možnost Přidat](#add-users-and-assign-licenses) uživatele.

    ![Snímek obrazovky s přihlašovací stránkou Přizpůsobení](../media/adddomain.png)

    
4. Postupujte podle pokynů průvodce a vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro [Microsoft 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověří, že doménu vlastníte. Pokud hostitele domény znáte, podívejte se také na [konkrétní pokyny pro hostitele.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiným hostitelem povoleným připojením [domény,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)proces je snadný a automaticky se zobrazí žádost o přihlášení a ověření společnosti Microsoft vaším jménem.

    ![Na stránce Potvrdit přístup na GoDaddy vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Uživatele můžete přidat v průvodci, ale můžete je přidat [i později v](add-users-m365b.md) Centru pro správu. Pokud máte také místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v průvodci

Všichni uživatelé, které přidáte v průvodci, se automaticky přiřadí licenci Microsoft 365 Business Premium.

![Snímek obrazovky se stránkou Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. Pokud vaše předplatné Microsoft 365 Business Premium již uživatele má (například pokud jste používali službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů budete mít taky možnost přihlašovací údaje sdílet s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu .onmicrosoft nebo k nastavení uživatelů použili Azure AD Connect, tento krok se vám neukaží.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud ne, změňte [názvové servery, abyste nastavili Microsoft 365 u libovolného doménového registrátora.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 

    - Pokud máte existující záznamy DNS, třeba existující web, ale hostitel DNS má povolené připojení k [doméně,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)zvolte Přidat **záznamy za mě.** Na stránce **Zvolit online služby** přijměte výchozí nastavení a zvolte  Další a na stránce hostitele DNS zvolte Autorizovat.
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení k doméně), můžete spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojeny. Další [informace najdete v základních](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) informacích o doméně.

        ![Stránka Aktivace záznamů](../media/activaterecords.png)

2. Postupujte podle pokynů v průvodci a nastavte e-mail a další služby.

### <a name="protect-your-organization"></a>Ochrana organizace 

Zásady nastavené v průvodci se automaticky použijí na skupinu [zabezpečení s](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) názvem *Všichni uživatelé.* V Centru pro správu můžete taky vytvořit další skupiny, ke které budete zásady přiřazovat.

1. Pokud chcete **zvýšit** ochranu před pokročilými kybernetickými hrozbami, doporučujeme vám přijmout výchozí nastavení, abyste v aplikacích [Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) 2013 pustit funkci Rozšířená ochrana před hrozbami a odkazy.

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. Na  stránce Zabránit úniku citlivých dat přijměte výchozí nastavení, které zapne funkci Ochrana před únikem informací (DLP) v Office 365 za cílem sledovat citlivá data v aplikacích Office a zabránit náhodnému sdílení těchto dat mimo vaši organizaci.

3. Na stránce **Chránit data v Office** pro mobilní zařízení nechte správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit zásadu správy **mobilních aplikací.**

    ![Snímek obrazovky se stránkou Zamknout data v Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečení počítačů s Windows 10

Na levém navigačním panelu **vyberte** Nastavení a pak v části Přihlášení a zabezpečení zvolte Zabezpečení počítačů s Windows **10.** Abyste **s tím začali,** zvolte Zobrazit. Úplné pokyny najdete v článku o zabezpečení [počítačů s Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Nasazení klientských aplikací Office 365

Pokud jste během instalace zvolili automatickou instalaci aplikací Office, aplikace se na zařízení s Windows 10 nainstalují, jakmile se uživatelé ze svých zařízení s Windows na svém zařízení s Windows k Azure AD přihlásili pomocí svých pracovních přihlašovacích údajů.

Informace o instalaci Office na mobilní zařízení s iOS nebo Androidem najdete v tématu Nastavení mobilních zařízení pro [uživatele Microsoft 365 Business Premium.](set-up-mobile-devices.md)

Můžete také nainstalovat Office jednotlivě. Pokyny [najdete v článku o instalaci Office na PC nebo Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Viz také

[Školicí videa pro Microsoft 365 pro firmy](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
