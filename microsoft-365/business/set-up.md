---
title: Nastavení Microsoft 365 Business
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
description: Naučte se nastavit aplikaci Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831297"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Nastavení aplikace Microsoft 365 Business v Průvodci nastavením

Na tomto videu můžete sledovat přehled programu Microsoft 365 Business Setup.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Pokud jste toto video našli, podívejte se na [kompletní tréninkové řady pro malé firmy a ty nové do společnosti Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Zakoupí-li společnost Microsoft 365 Business, máte možnost používat vlastní doménu nebo ji zakoupit během [zápisu](sign-up.md).

- Pokud jste při přihlášení zakoupili novou doménu, je vaše doména nastavena a můžete se přesouvat a [přidávat uživatele a přiřazovat jim licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény k přizpůsobení přihlášení

1. Přihlaste se ke [středisku Microsoft 365 Admin Center](https://admin.microsoft.com) pomocí globálních pověření pro správu. 

2. Chcete-li spustit průvodce, zvolte možnost **Přejít k instalačnímu programu** .

    ![Vyberte možnost přejít k nastavení.](media/gotosetupinadmincenter.png)

3. Na stránce **instalace aplikací sady Office** můžete aplikace volitelně nainstalovat do vlastního počítače.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).

    > [!IMPORTANT]
    > Pokud jste během zápisu zakoupili doménu, nezobrazí se zde krok **Přidat doménu** . Přejděte na místo pro [Přidání uživatelů](#add-users-and-assign-licenses) .

    ![Obrazovka stránky přizpůsobit přihlašovací stránku.](media/adddomain.png)

    
4. Postupujte podle pokynů průvodce a [vytvořte záznamy DNS u kteréhokoli poskytovatele hostitelských služeb DNS pro sadu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověřuje vlastní doménu. Pokud znáte hostitele domény, podívejte se také na [pokyny týkající se hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je poskytovatelem hostitelských služeb GoDaddy nebo jiný hostitel povolený s [připojením k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadný a budete automaticky požádáni o přihlášení a ověřování společnosti Microsoft ve vašem zastoupení.

    ![U možnosti potvrdit přístup na stránce GoDaddy vyberte možnost ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Můžete přidat uživatele v průvodci, ale můžete je také [přidat později](add-users-m365b.md) v centru pro správu. Navíc, pokud máte místní řadič domény, můžete přidat uživatele pomocí [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v Průvodci

Všichni uživatelé, které přidáte v průvodci, dostanou automaticky přiřazenu licenci Microsoft 365 Business.

![Obrazovka stránky přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. Pokud vaše předplatné aplikace Microsoft 365 Business obsahuje existující uživatele (například pokud jste použili program Azure AD Connect), můžete jim nyní přiřadit licence. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů budete mít také možnost sdílet pověření s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud zvolíte použití domény. onmicrosoft nebo použijete Azure AD Connect pro nastavení uživatelů, tento krok se nezobrazí.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [změňte nameservery tak, aby sadu Office 365 nastavil s jakýmkoli registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte možnost **Přidat záznamy**. Na stránce **Vyberte stránku služeb online** , přijměte všechny výchozí hodnoty a klepněte na tlačítko **Další**a na stránce hostitele DNS vyberte možnost **autorizovat** .
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (nejsou povoleny pro připojení k doméně), budete chtít spravovat své vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou propojeny. Další informace naleznete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Aktivuje stránku záznamů.](media/activaterecords.png)

2. Postupujte podle pokynů průvodce a e-maily a další služby budou nastaveny pro vás.

### <a name="protect-your-organization"></a>Ochrana organizace 

Zásady nastavené v průvodci jsou automaticky použity pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*. Můžete také vytvořit další skupiny pro přiřazení zásad v centru pro správu.

1. Při **zvýšení ochrany před pokročilými internetovými hrozbami**se doporučuje přijmout výchozí hodnoty, které umožňují [systému Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) prohledávat soubory a odkazy v aplikacích sady Office.

    ![Obrazovka stránky zvýšení ochrany.](media/increasetreatprotection.png)


2. Pokud chcete **zabránit úniku citlivých datových** stránek, přijměte výchozí nastavení pro zapnutí funkce Zabránění ztrátám dat (DLP) sady Office 365 za účelem sledování citlivých dat v aplikacích sady Office a zabránění nechtěnému sdílení těchto dat mimo vaši organizaci.

3. Na stránce **Chraňte data v sadě Office pro mobilní** stránku ponechejte správu mobilních aplikací, rozbalte nastavení a Prohlédněte si je a pak vyberte možnost **vytvořit zásadu správy mobilních aplikací**.

    ![Kopie obrazovky Chraňte data v sadě Office pro mobilní stránku.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečení systému Windows 10 počítačů

Na levém navigačním panelu vyberte **Nastavení** a potom v části zapnuto **a zabezpečení**zvolte zabezpečení **počítačů se systémem Windows 10**. Zvolte **zobrazení** pro začátek. Úplné pokyny naleznete v části [zabezpečení počítačů se systémem Windows 10](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>Nasadit sadu Office 365 Client Apps

Pokud jste při instalaci zvolili automatickou instalaci aplikací sady Office, budou aplikace nainstalovány do zařízení systému Windows 10, jakmile se uživatelé k Azure AD přihlašují z jejich zařízení se systémem Windows, pomocí svých pracovních pověření.

Informace o instalaci sady Office na mobilních zařízeních iOS nebo Android naleznete v tématu [nastavení mobilních zařízení pro Microsoft 365 Business Users](set-up-mobile-devices.md).

Sadu Office můžete nainstalovat také jednotlivě. Pokyny naleznete [v části instalace sady Office v počítači nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>Viz také

[Microsoft 365 Business Training video](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
