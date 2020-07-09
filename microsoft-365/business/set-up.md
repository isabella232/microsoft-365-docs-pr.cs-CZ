---
title: Nastavení Microsoftu 365 Business Premium
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
description: Seznamte se s kroky nastavení microsoftu 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081815"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Nastavení Microsoftu 365 Business Premium v průvodci instalací

Podívejte se na toto video, kde najdete přehled nastavení Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

Když si koupíte Microsoft 365 Business Premium, máte možnost použít doménu, kterou vlastníte, nebo si ji zakoupit během [registrace](sign-up.md).

- Pokud jste si při registraci zakoupili novou doménu, je vaše doména nastavena a můžete přejít na [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény k přizpůsobení přihlášení

1. Přihlaste se do [Centra pro správu Microsoftu 365](https://admin.microsoft.com) pomocí svých globálních přihlašovacích údajů správce. 

2. Chcete-li spustit průvodce, zvolte Přejít na **nastavení.**

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. Na stránce **Instalace aplikací Office** můžete aplikace volitelně nainstalovat do vlastního počítače.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).

    > [!IMPORTANT]
    > Pokud jste doménu zakoupili během registrace, zde se krok **Přidání domény** nezobrazuje. Místo toho přejděte na [Přidat uživatele.](#add-users-and-assign-licenses)

    ![Snímek obrazovky s přihlašovací stránkou Přizpůsobení](../media/adddomain.png)

    
4. Postupujte podle pokynů v průvodci [k vytvoření záznamů DNS u libovolného poskytovatele hostingu DNS pro Microsoft 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověří, že doménu vlastníte. Pokud znáte hostitele domény, přečtěte si také [pokyny pro konkrétního hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiný hostitel s [povoleným doménou](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces je snadný a budete automaticky vyzváni k přihlášení a povolení společnosti Microsoft k ověření vaším jménem.

    ![Na stránce GoDaddy Potvrdit přístup vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Uživatele můžete přidat do průvodce, ale [můžete také přidat uživatele později](add-users-m365b.md) v Centru pro správu. Pokud máte místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v průvodci

Všem uživatelům, které přidáte do průvodce, bude automaticky přiřazena licence Microsoft 365 Business Premium.

![Snímek obrazovky se stránkou Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. Pokud vaše předplatné Microsoft 365 Business Premium má stávající uživatele (například pokud jste použili Azure AD Connect), získáte možnost přiřadit licence k nim teď. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů získáte také možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu .onmicrosoft nebo použít Azure AD Connect k nastavení uživatelů, tento krok se vám neuvede.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [změňte názvové servery a nastavte Microsoft 365 s libovolným registrátorem domény](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Pokud máte existující záznamy DNS, například existující web, ale váš hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte **Přidat záznamy pro mě**. Na stránce **Zvolit online služby** přijměte všechna výchozí nastavení a zvolte **Další**a na stránce hostitele DNS zvolte **Autorizovat.**
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení k doméně), budete chtít spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou ve spojení. Další informace najdete v [základech domény.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivovat stránku záznamů.](../media/activaterecords.png)

2. Postupujte podle pokynů v průvodci a e-mail a další služby budou nastaveny za vás.

### <a name="protect-your-organization"></a>Chraňte svou organizaci 

Zásady nastavené v průvodci se automaticky použijí na [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*. Můžete také vytvořit další skupiny pro přiřazení zásad v Centru pro správu.

1. V části **Zvýšení ochrany před pokročilými kybernetickými hrozbami**doporučujeme přijmout výchozí nastavení, abyste office [365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) nechali skenovat soubory a odkazy v aplikacích Office.

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. Na stránce **Zabránit únikům citlivých dat** přijměte výchozí nastavení a zapněte office 365 prevence ztráty dat (DLP) ke sledování citlivých dat v aplikacích Office a zabraňte jejich náhodnému sdílení mimo vaši organizaci.

3. Na stránce **Chránit data v Office pro mobilní zařízení** ponechte zapnutou správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit **zásady správy mobilních aplikací**.

    ![Snímek obrazovky s funkcí Chránit data na stránce Office pro mobily](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečení počítačů s Windows 10

V levém navigačním panelu vyberte **Instalační program** a potom v části Přihlášení **a zabezpečení**zvolte **Zabezpečit počítače s Windows 10**. Chcete-li začít, zvolte **Zobrazení.** Kompletní pokyny [najdete v tématu Zabezpečení počítačů s Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Nasazení klientských aplikací Office 365

Pokud se rozhodnete automaticky instalovat aplikace Office během instalace, aplikace se nainstalují na zařízení s Windows 10, jakmile se uživatelé přihlásí k Azure AD ze svých zařízení s Windows pomocí svých pracovních pověření.

Informace o instalaci Office na mobilní zařízení se systémem iOS nebo Android najdete v [tématu Nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md).

Office můžete nainstalovat také jednotlivě. Pokyny najdete [v tématu instalace Office na PC nebo Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Viz také

[Školicí videa microsoftu 365 pro firmy](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
