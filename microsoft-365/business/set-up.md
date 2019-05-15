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
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966972"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Nastavení Průvodce instalací Microsoft 365 Business

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatele a nastavení zásad

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Při koupi Microsoft 365 Business, máte možnost použít doménu vlastníte, nebo při nákupu [zápisu](sign-up.md).

- Pokud jste zakoupili novou doménu při registraci, vaše doména je sada všech nahoru a můžete přesunout, chcete-li [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání přizpůsobit přihlašovací domény

1. Přihlášení k aplikaci [Microsoft 365 admin center](https://admin.microsoft.com) pomocí globální správce pověření. 

2. Zvolte **Přidat k doméně** nebo **Přidání uživatelů** ke spuštění průvodce.
    > [!IMPORTANT]
    > Pokud jste doménu zakoupili během přihlašování, není viz **Přidání domény** kroku zde. Místo toho přejděte na [Přidat uživatele](#add-users-and-assign-licenses) .

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

![Obrazovka stránku přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. Má-li vaše předplatné Microsoft 365 Business existujících uživatelů (například pokud používáte Azure AD připojit), dostanete možnost přiřazovat licence je nyní. Neváhejte a přidejte licence i jim.

3. Po přidání uživatele se zobrazí také možnost sdílet pověření s novým uživatelům, které jste přidali. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

4. Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**. 

    Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud používáte domény .onmicrosoft nebo lze nastavit uživatele Azure AD připojit, nezobrazí se tento krok.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Pokud máte existující záznamy DNS, například existující web, můžete ke správě DNS záznamů a ujistěte se, že zachovat stávající služby připojení. Viz [základní informace o doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) pro další informace.

        ![Připojit domény stránky lze spravovat vlastní záznamy DNS.](media/connectyourdomainpage.png)

2. Postupujte podle pokynů v průvodci a e-mailů a dalších služeb bude nastavení pro vás.

### <a name="set-up-security-policies-and-device-configurations"></a>Nastavit zásady zabezpečení a konfigurace zařízení 

Zásady, které jste nastavili v Průvodci automaticky použity [skupiny zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*. Můžete také vytvořit další skupiny přiřadit zásady v Centru pro správu.

1. **Ochranu pracovních souborů na mobilních zařízeních** možnost **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** je zapnutá ve výchozím nastavení. Máte možnost zapnout **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních**, a to je doporučeno.

    ![Snímek obrazovky chránit pracovní soubory na stránce Mobilní zařízení.](media/protectworkfilesondevices.png)

     - Rozbalte položku **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** zobrazí [výchozí hodnoty](protect-work-files-on-lost-or-stolen-device.md):

        ![Obrazovka výchozí hodnoty pro ochranu souborů na ztracené zařízení.](media/protectworkfilesondevicesdefault.png)

    - Vyberte **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních** a rozbalit a zobrazit [výchozí hodnoty](manage-user-access-on-mobile-devices.md). Doporučujeme přijmout výchozí hodnoty během instalace k vytvoření zásad aplikace pro Android, iOS a Windows 10, které platí pro všechny uživatele. Další zásady můžete vytvořit po dokončení instalace.

        ![Obrazovka nastavení ochrany souborů sady Office Mobile.](media/useraccessonmobile.png)

2. Poslední krok na ochranu dat a zařízení umožňuje nastavit zásady zabezpečení Windows 10 zařízení. Toto nastavení automaticky použito při připojení uživatele v systému Windows 10 pro vaši organizaci. Můžete rozbalit **zabezpečení Windows 10 zařízení** zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).
3. Můžete také [automaticky nainstalovat systém Office](install-office-on-windows-10-during-setup.md) na zařízení Windows 10.

    ![Obrazovka nastavení stránku konfigurace zařízení Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Nasazení aplikace klienta služeb Office 365

Pokud zvolíte automaticky nainstalovat Office apps v průběhu sada nahoru, nainstaluje soubor apps po uživatelé přihlášeni k Azure AD ze svých zařízení systému Windows pomocí pověření jejich práce na zařízení Windows 10.
Chcete-li nainstalovat systém Office na mobilním iOS nebo Android zařízení, naleznete v tématu [nastavit mobilní zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).

Office lze také nainstalovat samostatně. Viz pokyny pro [instalaci sady Office na PC nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .
