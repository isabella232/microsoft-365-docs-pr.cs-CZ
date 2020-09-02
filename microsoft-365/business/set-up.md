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
description: Podívejte se na postup nastavení Microsoft 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a další.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324490"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Nastavení Microsoft 365 Business Premium v Průvodci nastavením

V tomto videu najdete přehled nastavení Microsoft 365 Business Premium.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>Přidání domény, uživatelů a nastavení zásad

Když si koupíte Microsoft 365 Business Premium, můžete použít doménu, kterou vlastníte, nebo si ji koupit během [zápisu](sign-up.md).

- Pokud jste při registraci zakoupili novou doménu, bude vaše doména nastavovaná a můžete se přesouvat a [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Přidání domény pro personalizaci přihlášení

1. Přihlaste se do [centra pro správu Microsoft 365](https://admin.microsoft.com) pomocí přihlašovacích údajů globálního správce. 

2. Kliknutím **na Přejít na nastavení** spusťte průvodce.

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. Na stránce **nainstalovat aplikace Office** můžete volitelně nainstalovat aplikace na počítači.
    
4. V kroku **Přidat doménu** zadejte název domény, který chcete použít (třeba contoso.com).

    > [!IMPORTANT]
    > Pokud jste během registrace zakoupili doménu, nebudete tady zde **Přidat krok pro přidání domény** . Přejděte na [Přidat uživatele](#add-users-and-assign-licenses) .

    ![Snímek obrazovky s přidanou přihlašovací stránkou](../media/adddomain.png)

    
4. Podle pokynů v průvodci [vytvořte záznamy DNS u kteréhokoli poskytovatele hostingu DNS pro Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověří, že jste vlastníkem domény. Pokud znáte hostitele domény, přečtěte si také [pokyny pro hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Pokud je váš poskytovatel hostingu GoDaddy nebo je povolený jiný hostitel se službou [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadno přihlášený a Vy se automaticky zobrazí výzva k přihlášení a aby Microsoft ověřil váš účet.

    ![Na stránce potvrzení přístupu GoDaddy vyberte autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Přidání uživatelů a přiřazení licencí

Uživatele můžete do průvodce Přidat, ale můžete je taky [přidat později](add-users-m365b.md) v centru pro správu. Pokud máte místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Přidání uživatelů v Průvodci

Všichni uživatelé, které přidáte do průvodce, získají automaticky licenci Microsoft 365 Business Premium.

![Snímek obrazovky se stránkou přidat nové uživatele v Průvodci](../media/addnewuserspage.png)

1. Pokud vaše předplatné Microsoft 365 Business Premium má existující uživatele (například pokud jste použili Azure AD Connect), získáte k těmto možnostem přiřazení licencí. Neváhejte a přidejte licence i jim.

2. Po přidání uživatelů můžete také sdílet přihlašovací údaje s novými přidanými uživateli. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.

### <a name="connect-your-domain"></a>Připojení domény

> [!NOTE]
> Pokud jste se rozhodli použít doménu. doména společnosti Microsoft nebo použili Azure AD Connect k nastavení uživatelů, tento krok se nezobrazuje.
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud to nepomůže, [změňte názvové servery na nastavení Microsoft 365 s libovolným doménovým registrátorem](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte **Přidat záznamy pro mě**. Na stránce **Vyberte si online služby** potvrďte všechna výchozí nastavení a zvolte **Další**a zvolte **autorizovat** na stránce hostitele DNS.
    - Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povolené pro Domain Connect), budete chtít spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojené. Další informace najdete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![Stránka aktivace záznamů](../media/activaterecords.png)

2. Postupujte podle pokynů v průvodci a e-mail a další služby budou pro vás nastaveny.

### <a name="protect-your-organization"></a>Ochrana organizace 

Zásady, které nastavíte v průvodci, se automaticky použijí pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*. Můžete taky vytvořit další skupiny pro přiřazení zásad do centra pro správu.

1. Na **zvýšení ochrany před rozšířenými internetovými hrozbami**se doporučuje přijmout výchozí nastavení, aby aplikace Office [365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) prohledala soubory a odkazy v aplikacích Office.

    ![Snímek obrazovky se stránkou zvýšení ochrany](../media/increasetreatprotection.png)


2. Na stránce **zabránění únikům citlivých dat** přijměte výchozí hodnoty, abyste zapnuli ochranu před nevracením dat v Office 365, která sledují citlivá data v aplikacích Office a zabrání nechtěnému sdílení těchto funkcí mimo vaši organizaci.

3. Na stránce **chránit data v Office pro mobil** opustit správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte **vytvořit zásadu správy mobilních aplikací**.

    ![Snímek obrazovky s ochranou dat na stránce Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Zabezpečení počítačů s Windows 10

Na levém navigačním panelu vyberte **Nastavení** a pak v části **přihlášení a zabezpečení**zvolte **zabezpečit počítače s Windows 10**. Začněte tím, že zvolíte **zobrazení** . Podrobné pokyny najdete v tématu [zabezpečení počítačů s Windows 10](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>Nasazení klientských aplikací Office 365

Pokud jste se při instalaci rozhodli automaticky nainstalovat aplikace Office, budou se tyto aplikace instalovat na zařízení s Windows 10, jakmile se uživatelé přihlásí ke službě Azure AD ze svých zařízení s Windows, pomocí svých uživatelských přihlašovacích údajů.

Pokud chcete nainstalovat Office na mobilní zařízení s iOS nebo Androidem, přečtěte si článek [nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md).

Office můžete také nainstalovat jednotlivě. Pokyny najdete v článku [instalace Office na PC nebo Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>Viz také

[Školicí kurzy pro Microsoft 365 for Business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
