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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Naučte se nastavit aplikaci Microsoft 365 Business.
ms.openlocfilehash: dbd2e740c85f52d3f43e6cd3d6ce45c478a9b1a9
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121312"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Nastavení aplikace Microsoft 365 Business v Průvodci nastavením

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

[![Popisek vám dá vědět, že se centrum pro správu mění a další podrobnosti naleznete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Zakoupí-li společnost Microsoft 365 Business, máte možnost používat vlastní doménu nebo ji zakoupit během [zápisu](sign-up.md).

- Pokud jste při přihlášení zakoupili novou doménu, je vaše doména nastavena a můžete se přesouvat a [přidávat uživatele a přiřazovat jim licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény k přizpůsobení přihlášení

1. Přihlaste se ke [středisku Microsoft 365 Admin Center](https://admin.microsoft.com) pomocí globálních pověření pro správu. 

2. Zvolte možnost **Přidat doménu** nebo **Přidat uživatele** Chcete-li spustit průvodce.
    > [!IMPORTANT]
    > Pokud jste během zápisu zakoupili doménu, nezobrazí se zde krok **Přidat doménu** . Přejděte na místo pro [Přidání uživatelů](#add-users-and-assign-licenses) .

    ![Vyberte možnost Přidat doménu.](media/addadomainadmincenter.png)
    
3. V průvodci zadejte název domény, který chcete použít (například contoso.com).


    ![Obrazovka stránky přizpůsobit přihlašovací stránku.](media/personalizesignin.png)

    
4. Postupujte podle pokynů průvodce a [vytvořte záznamy DNS u kteréhokoli poskytovatele hostitelských služeb DNS pro sadu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověřuje vlastní doménu. Pokud znáte hostitele domény, podívejte se také na [pokyny týkající se hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je poskytovatelem hostitelských služeb GoDaddy nebo jiný hostitel s připojením k [doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadný a budete automaticky požádáni o přihlášení a společnost Microsoft vám bude ověřovat ve vašem zastoupení:

    ![U možnosti potvrdit přístup na stránce GoDaddy vyberte možnost ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Můžete přidat uživatele v průvodci, ale můžete je také [přidat později](add-users-m365b.md) v centru pro správu. Navíc, pokud máte místní řadič domény, můžete přidat uživatele pomocí [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v Průvodci

Všichni uživatelé, které přidáte v průvodci, dostanou automaticky přiřazenu licenci Microsoft 365 Business.

![Obrazovka stránky přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. Pokud vaše předplatné aplikace Microsoft 365 Business obsahuje existující uživatele (například pokud jste použili program Azure AD Connect), můžete jim nyní přiřadit licence. Neváhejte a přidejte licence i jim.

3. Po přidání uživatelů budete mít také možnost sdílet pověření s novými uživateli, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

4. Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**. 

    Pokud se přesouváte od jiného poskytovatele e-mailu a chcete data později zkopírovat, můžete [přenést e-maily a kontakty do sady Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud zvolíte použití domény. onmicrosoft nebo použijete Azure AD Connect pro nastavení uživatelů, tento krok se nezobrazí.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [změňte nameservery tak, aby sadu Office 365 nastavil s jakýmkoli registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte možnost **Přidat záznamy**. 
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (nejsou povoleny pro připojení k doméně), budete chtít spravovat své vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou propojeny. Další informace naleznete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Připojte stránku domény ke správě vlastních záznamů DNS.](media/connectyourdomainpage.png)

2. Postupujte podle pokynů průvodce a e-maily a další služby budou nastaveny pro vás.

### <a name="set-up-security-policies-and-device-configurations"></a>Nastavení zásad zabezpečení a konfigurace zařízení 

Zásady nastavené v průvodci jsou automaticky použity pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*. Můžete také vytvořit další skupiny pro přiřazení zásad v centru pro správu.

1. Na panelu **Chraňte své pracovní soubory na mobilních zařízeních** možnost **chránit pracovní soubory při ztrátě nebo odcizení zařízení** je ve výchozím nastavení vybráno. Máte možnost zapnout **správu způsobu, jakým uživatelé přistupují k souborům sady Office na mobilních zařízeních**, a tento postup je doporučen.

    ![Obrazovka o ochraně pracovních souborů na stránce mobilních zařízení](media/protectworkfilesondevices.png)

     - Rozbalit **ochranu pracovních souborů při ztrátě nebo odcizení zařízení** pro zobrazení [výchozích hodnot](protect-work-files-on-lost-or-stolen-device.md):

        ![Obrazovka výchozích hodnot pro ochranu souborů ztracených zařízení.](media/protectworkfilesondevicesdefault.png)

    - Vyberte možnost **spravovat způsob, jakým uživatelé přistupují k souborům systému Office v mobilních zařízeních** , a rozbalte ji, aby zobrazili [výchozí hodnoty](manage-user-access-on-mobile-devices.md). Doporučujeme, abyste při instalaci přijali výchozí hodnoty a vytvořili tak zásady použití pro systémy Android, iOS a Windows 10, které se vztahují na všechny uživatele. Další zásady můžete vytvořit po dokončení instalace.

        ![Obrazovka nastavení ochrany pro soubory sady Office v mobilním počítači.](media/useraccessonmobile.png)

2. Poslední krok týkající se ochrany dat a zařízení umožňuje nastavit zásady pro zabezpečení zařízení systému Windows 10. Tato nastavení jsou automaticky použita při připojení uživatele systému Windows 10 k vaší organizaci. Můžete rozbalit **Zabezpečená zařízení Windows 10** a zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).
3. Můžete také zvolit [automatickou instalaci sady Office](install-office-on-windows-10-during-setup.md) do zařízení systému Windows 10.

    ![Obrazovka nastavení stránky konfigurace zařízení systému Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Nasadit sadu Office 365 Client Apps

Pokud se rozhodnete automaticky instalovat aplikace sady Office během nastavování, budou aplikace nainstalovány do zařízení systému Windows 10, jakmile se uživatelé budou přihlásit k Azure AD z jejich zařízení se systémem Windows s jejich pracovním pověřením.
Informace o instalaci sady Office na mobilních zařízeních iOS nebo Android naleznete v tématu [nastavení mobilních zařízení pro Microsoft 365 Business Users](set-up-mobile-devices.md).

Sadu Office můžete nainstalovat také jednotlivě. Pokyny naleznete [v části instalace sady Office v počítači nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .
