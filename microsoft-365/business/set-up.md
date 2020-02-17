---
title: Nastavení Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Přečtěte si, jak nastavit Microsoft 365 Business.
ms.openlocfilehash: a41d03c4f9e250cf3b16d11bf23897e31adaf866
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42090828"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Nastavení Microsoft 365 Business v průvodci nastavením

Podívejte se na toto video, kde najdete přehled nastavení Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Při nákupu Microsoft 365 Business máte možnost používat doménu, kterou vlastníte, nebo ji zakoupit během [registrace](sign-up.md).

- Pokud jste si zakoupili novou doménu, když jste se zaregistrovali, je vaše doména nastavena a můžete přejít na [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény pro přizpůsobení přihlášení

1. Přihlaste se do [Centra pro správu Microsoftu 365](https://admin.microsoft.com) pomocí globálních přihlašovacích údajů pro správce. 

2. Chcete-li spustit průvodce, zvolte **Přejít a** spustit ho.

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. Na stránce **Instalovat aplikace Office** můžete aplikace volitelně nainstalovat do vlastního počítače.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).

    > [!IMPORTANT]
    > Pokud jste si během registrace zakoupili doménu, nezobrazí se zde přidání kroku **domény.** Přejděte místo toho na [Přidat uživatele.](#add-users-and-assign-licenses)

    ![Snímek obrazovky s přihlašovací stránkou](../media/adddomain.png)

    
4. Podle pokynů průvodce [vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro Office 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověřuje vlastní doménu. Pokud znáte hostitele domény, přečtěte si také [pokyny pro konkrétní hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiný hostitel povolen s [připojením domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces je snadný a budete automaticky vyzváni, abyste se přihlásili a nechali Microsoft ověřovat vaším jménem.

    ![Na stránce Potvrzení přístupu GoDaddy vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Do průvodce můžete přidat uživatele, ale uživatele můžete přidat [i později](add-users-m365b.md) v Centru pro správu. Pokud máte místní řadič domény, můžete navíc přidat uživatele pomocí [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů do průvodce

Všem uživatelům, které přidáte do průvodce, bude automaticky přiřazena licence Microsoft 365 Business.

![Snímek obrazovky stránky Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. Pokud má vaše předplatné Microsoft 365 Business existující uživatele (například pokud jste použili Azure AD Connect), získáte možnost přiřadit jim licence nyní. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů získáte také možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu .onmicrosoft nebo pomocí Azure AD Connect k nastavení uživatelů, tento krok se vám nezobrazí.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [změňte názvové servery a nastavte Office 365 s libovolným registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte Přidat záznamy **pro mě**. Na stránce **Zvolit online služby** přijměte všechny výchozí hodnoty a zvolte **Další**a na stránce hostitele DNS zvolte **Autorizovat.**
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení domény), budete chtít spravovat vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou připojeny. Další informace naleznete v [základech domény.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivujte stránku záznamů.](../media/activaterecords.png)

2. Postupujte podle pokynů průvodce a e-mail a další služby budou nastaveny pro vás.

### <a name="protect-your-organization"></a>Ochrana vaší organizace 

Zásady nastavené v průvodci se automaticky použijí na [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*. Můžete také vytvořit další skupiny, které budou přiřazeny zásady v Centru pro správu.

1. V části **Zvýšení ochrany před pokročilými kybernetickými hrozbami**doporučujeme přijmout výchozí nastavení, které umožní [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skenovat soubory a odkazy v aplikacích Office.

    ![Snímek obrazovky stránky Zvýšit ochranu](../media/increasetreatprotection.png)


2. Na stránce **Zabránit úniku citlivých dat** přijměte výchozí nastavení pro zapnutí Office 365 Data Loss Prevention (DLP) pro sledování citlivých dat v aplikacích Office a zabránění náhodnému sdílení těchto dat mimo vaši organizaci.

3. Na stránce **Zamknout data v Office pro mobilní zařízení** ponechte zapnutou správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit **zásady správy mobilních aplikací**.

    ![Snímek obrazovky Stránky Ochrana dat v Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečené počítače s Windows 10

Na levé nav vyberte **Nastavení** a potom v části **Sing-in a security**zvolte **Zabezpečit počítače se systémem Windows 10**. Chcete-li začít, zvolte **Zobrazení.** Kompletní pokyny najdete v [tématu zabezpečení počítačů s Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Nasazení klientských aplikací Office 365

Pokud jste se během instalace rozhodli automaticky nainstalovat aplikace Office, aplikace se nainstalují na zařízení s Windows 10, jakmile se uživatelé přihlásí k Azure AD ze svých zařízení s Windows pomocí svých pracovních přihlašovacích údajů.

Pokud chcete Office nainstalovat na mobilní zařízení se systémem iOS nebo Android, přečtěte si v [tématu Nastavení mobilních zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).

Office můžete nainstalovat také samostatně. Pokyny najdete v [tématu Instalace Office na PC nebo Mac.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Viz také

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
