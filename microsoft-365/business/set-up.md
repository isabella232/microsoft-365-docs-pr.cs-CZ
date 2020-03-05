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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Seznamte se s kroky nastavení microsoftu 365 Business, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších.
ms.openlocfilehash: 4535a32b579b91b6c2bb0e64ec95904be6c08fce
ms.sourcegitcommit: 6c8edbc54b193e964cf93aec48c51cb79231f1d9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2020
ms.locfileid: "42543933"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Nastavení Microsoft 365 Business v průvodci instalací

Podívejte se na toto video s přehledem nastavení Microsoftu 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Při nákupu microsoftu 365 Business máte možnost použít doménu, kterou vlastníte, nebo ji zakoupit při [registraci](sign-up.md).

- Pokud jste si při registraci zakoupili novou doménu, je vaše doména nastavena a můžete přejít na [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény pro přizpůsobení přihlášení

1. Přihlaste se k [Centru pro správu Microsoftu 365](https://admin.microsoft.com) pomocí přihlašovacích údajů globálního správce. 

2. Chcete-li průvodce spustit, zvolte **Přejít na nastavení.**

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. Na stránce **Instalovat aplikace Office** můžete volitelně nainstalovat aplikace do vlastního počítače.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).

    > [!IMPORTANT]
    > Pokud jste si doménu zakoupili během registrace, zde se nezobrazí krok **Přidat doménu.** Místo toho přejděte na [Přidat uživatele.](#add-users-and-assign-licenses)

    ![Snímek obrazovky s přihlašovací stránkou Přizpůsobení](../media/adddomain.png)

    
4. Podle pokynů v průvodci [vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro Office 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověří, že doménu vlastníte. Pokud znáte hostitele domény, přečtěte si také [pokyny pro konkrétní hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiným hostitelem s [povoleným připojením domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je proces snadný a budete automaticky požádáni o přihlášení a nechat Microsoft ověřovat vaším jménem.

    ![Na stránce GoDaddy Confirm Access vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Můžete přidat uživatele v průvodci, ale můžete také [přidat uživatele později](add-users-m365b.md) v Centru pro správu. Navíc pokud máte místní řadič domény, můžete přidat uživatele s [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů do průvodce

Všem uživatelům, které přidáte do průvodce, bude automaticky přiřazena licence Microsoft 365 Business.

![Snímek obrazovky stránky Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. Pokud vaše předplatné Microsoft 365 Business má stávající uživatele (například pokud jste použili Azure AD Connect), získáte možnost přiřadit licence k nim teď. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů získáte také možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu .onmicrosoft nebo použít Azure AD Connect k nastavení uživatelů, tento krok se nezobrazí.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [změňte názvové servery a nastavte Office 365 u libovolného doménového registrátora](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, ale váš hostitel DNS je povolen pro [připojení domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte Přidat záznamy **pro mě**. Na stránce **Vyberte si online služby** přijměte všechny výchozí hodnoty a zvolte **Další**a na stránce hostitele DNS zvolte **Autorizovat.**
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení domény), budete chtít spravovat vlastní záznamy DNS, abyste se ujistili, že stávající služby zůstanou ve spojení. Další informace najdete v [základech domény.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Aktivovat stránku záznamů.](../media/activaterecords.png)

2. Postupujte podle pokynů v průvodci a e-mail a další služby budou nastaveny pro vás.

### <a name="protect-your-organization"></a>Ochrana vaší organizace 

Zásady nastavené v průvodci se automaticky použijí na [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*. Můžete také vytvořit další skupiny, ke kterým můžete přiřazovat zásady v Centru pro správu.

1. Pokud jde o **zvýšení ochrany před pokročilými kybernetickými hrozbami**, doporučujeme, abyste přijímali výchozí hodnoty a nechali [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) prohledávat soubory a odkazy v aplikacích Office.

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. Na stránce **Zabránit únikům citlivých dat** přijměte výchozí nastavení pro zapnutí funkce Office 365 Data Loss Prevention (DLP) za účelem sledování citlivých dat v aplikacích Office a zabránění náhodnému sdílení těchto dat mimo vaši organizaci.

3. Na stránce **Chránit data v Office pro mobilní zařízení** ponechejte správu mobilních aplikací zapnutou, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit **zásady správy mobilních aplikací**.

    ![Snímek obrazovky s ochranou dat na stránce Office pro mobily](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečení počítačů s Windows 10

Na levém virtuálním počítači vyberte **Instalační program** a potom v části **Sing-in a security**zvolte **Zabezpečit počítače s Windows 10**. **Chcete-li začít,** zvolte Zobrazení. Kompletní pokyny najdete v [tématu zabezpečení počítačů s Windows 10.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Nasazení klientských aplikací Office 365

Pokud jste se rozhodli automaticky instalovat aplikace Office během instalace, aplikace se nainstalují na zařízeních s Windows 10, jakmile se uživatelé přihlásí k Azure AD ze svých zařízení s Windows, pomocí jejich pracovních pověření.

Informace o instalaci Office na mobilní zařízení se systémem iOS nebo android najdete v tématu [Nastavení mobilních zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).

Office můžete nainstalovat také jednotlivě. Pokyny [najdete v tématu instalace Office na PC nebo Mac.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)

## <a name="see-also"></a>Viz také

[Školicí videa k Microsoftu 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
