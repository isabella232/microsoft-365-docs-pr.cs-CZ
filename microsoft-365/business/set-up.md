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
description: Objevte kroky nastavení pro Microsoft 365 Business, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších.
ms.openlocfilehash: 4535a32b579b91b6c2bb0e64ec95904be6c08fce
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417290"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="f7a93-103">Nastavení Microsoft 365 Business v průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="f7a93-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="f7a93-104">Podívejte se na toto video, kde najdete přehled nastavení Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f7a93-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="f7a93-105">Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="f7a93-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="f7a93-106">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="f7a93-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="f7a93-107">[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="f7a93-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="f7a93-108">Při nákupu Microsoft 365 Business máte možnost používat doménu, kterou vlastníte, nebo ji zakoupit během [registrace](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="f7a93-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="f7a93-109">Pokud jste si zakoupili novou doménu, když jste se zaregistrovali, je vaše doména nastavena a můžete přejít na [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="f7a93-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="f7a93-110">Přidání domény pro přizpůsobení přihlášení</span><span class="sxs-lookup"><span data-stu-id="f7a93-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="f7a93-111">Přihlaste se do [Centra pro správu Microsoftu 365](https://admin.microsoft.com) pomocí globálních přihlašovacích údajů pro správce.</span><span class="sxs-lookup"><span data-stu-id="f7a93-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="f7a93-112">Chcete-li spustit průvodce, zvolte **Přejít a** spustit ho.</span><span class="sxs-lookup"><span data-stu-id="f7a93-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="f7a93-114">Na stránce **Instalovat aplikace Office** můžete aplikace volitelně nainstalovat do vlastního počítače.</span><span class="sxs-lookup"><span data-stu-id="f7a93-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="f7a93-115">V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f7a93-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="f7a93-116">Pokud jste si během registrace zakoupili doménu, nezobrazí se zde přidání kroku **domény.**</span><span class="sxs-lookup"><span data-stu-id="f7a93-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="f7a93-117">Přejděte místo toho na [Přidat uživatele.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="f7a93-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Snímek obrazovky s přihlašovací stránkou](../media/adddomain.png)

    
4. <span data-ttu-id="f7a93-119">Podle pokynů průvodce [vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro Office 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověřuje vlastní doménu.</span><span class="sxs-lookup"><span data-stu-id="f7a93-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="f7a93-120">Pokud znáte hostitele domény, přečtěte si také [pokyny pro konkrétní hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="f7a93-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="f7a93-121">Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiný hostitel povolen s [připojením domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), proces je snadný a budete automaticky vyzváni, abyste se přihlásili a nechali Microsoft ověřovat vaším jménem.</span><span class="sxs-lookup"><span data-stu-id="f7a93-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stránce Potvrzení přístupu GoDaddy vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="f7a93-123">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="f7a93-123">Add users and assign licenses</span></span>

<span data-ttu-id="f7a93-124">Do průvodce můžete přidat uživatele, ale uživatele můžete přidat [i později](add-users-m365b.md) v Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="f7a93-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="f7a93-125">Pokud máte místní řadič domény, můžete navíc přidat uživatele pomocí [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="f7a93-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="f7a93-126">Přidání uživatelů do průvodce</span><span class="sxs-lookup"><span data-stu-id="f7a93-126">Add users in the wizard</span></span>

<span data-ttu-id="f7a93-127">Všem uživatelům, které přidáte do průvodce, bude automaticky přiřazena licence Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f7a93-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Snímek obrazovky stránky Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. <span data-ttu-id="f7a93-129">Pokud má vaše předplatné Microsoft 365 Business existující uživatele (například pokud jste použili Azure AD Connect), získáte možnost přiřadit jim licence nyní.</span><span class="sxs-lookup"><span data-stu-id="f7a93-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="f7a93-130">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="f7a93-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="f7a93-131">Po přidání uživatelů získáte také možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="f7a93-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="f7a93-132">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="f7a93-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="f7a93-133">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="f7a93-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="f7a93-134">Pokud jste se rozhodli použít doménu .onmicrosoft nebo pomocí Azure AD Connect k nastavení uživatelů, tento krok se vám nezobrazí.</span><span class="sxs-lookup"><span data-stu-id="f7a93-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="f7a93-135">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="f7a93-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="f7a93-136">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="f7a93-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="f7a93-137">Pokud tomu tak není, [změňte názvové servery a nastavte Office 365 s libovolným registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="f7a93-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="f7a93-138">Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte Přidat záznamy **pro mě**.</span><span class="sxs-lookup"><span data-stu-id="f7a93-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="f7a93-139">Na stránce **Zvolit online služby** přijměte všechny výchozí hodnoty a zvolte **Další**a na stránce hostitele DNS zvolte **Autorizovat.**</span><span class="sxs-lookup"><span data-stu-id="f7a93-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="f7a93-140">Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení domény), budete chtít spravovat vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou připojeny.</span><span class="sxs-lookup"><span data-stu-id="f7a93-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="f7a93-141">Další informace naleznete v [základech domény.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="f7a93-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivujte stránku záznamů.](../media/activaterecords.png)

2. <span data-ttu-id="f7a93-143">Postupujte podle pokynů průvodce a e-mail a další služby budou nastaveny pro vás.</span><span class="sxs-lookup"><span data-stu-id="f7a93-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="f7a93-144">Ochrana vaší organizace</span><span class="sxs-lookup"><span data-stu-id="f7a93-144">Protect your organization</span></span> 

<span data-ttu-id="f7a93-145">Zásady nastavené v průvodci se automaticky použijí na [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="f7a93-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="f7a93-146">Můžete také vytvořit další skupiny, které budou přiřazeny zásady v Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="f7a93-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="f7a93-147">V části **Zvýšení ochrany před pokročilými kybernetickými hrozbami**doporučujeme přijmout výchozí nastavení, které umožní [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skenovat soubory a odkazy v aplikacích Office.</span><span class="sxs-lookup"><span data-stu-id="f7a93-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Snímek obrazovky stránky Zvýšit ochranu](../media/increasetreatprotection.png)


2. <span data-ttu-id="f7a93-149">Na stránce **Zabránit úniku citlivých dat** přijměte výchozí nastavení pro zapnutí Office 365 Data Loss Prevention (DLP) pro sledování citlivých dat v aplikacích Office a zabránění náhodnému sdílení těchto dat mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="f7a93-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="f7a93-150">Na stránce **Zamknout data v Office pro mobilní zařízení** ponechte zapnutou správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit **zásady správy mobilních aplikací**.</span><span class="sxs-lookup"><span data-stu-id="f7a93-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Snímek obrazovky Stránky Ochrana dat v Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="f7a93-152">Zabezpečené počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="f7a93-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="f7a93-153">Na levé nav vyberte **Nastavení** a potom v části **Sing-in a security**zvolte **Zabezpečit počítače se systémem Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="f7a93-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="f7a93-154">Chcete-li začít, zvolte **Zobrazení.**</span><span class="sxs-lookup"><span data-stu-id="f7a93-154">Choose **View** to get started.</span></span> <span data-ttu-id="f7a93-155">Kompletní pokyny najdete v [tématu zabezpečení počítačů s Windows 10.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="f7a93-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="f7a93-156">Nasazení klientských aplikací Office 365</span><span class="sxs-lookup"><span data-stu-id="f7a93-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="f7a93-157">Pokud jste se během instalace rozhodli automaticky nainstalovat aplikace Office, aplikace se nainstalují na zařízení s Windows 10, jakmile se uživatelé přihlásí k Azure AD ze svých zařízení s Windows pomocí svých pracovních přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="f7a93-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="f7a93-158">Pokud chcete Office nainstalovat na mobilní zařízení se systémem iOS nebo Android, přečtěte si v [tématu Nastavení mobilních zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="f7a93-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="f7a93-159">Office můžete nainstalovat také samostatně.</span><span class="sxs-lookup"><span data-stu-id="f7a93-159">You can also install Office individually.</span></span> <span data-ttu-id="f7a93-160">Pokyny najdete v [tématu Instalace Office na PC nebo Mac.](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="f7a93-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="f7a93-161">Viz také</span><span class="sxs-lookup"><span data-stu-id="f7a93-161">See also</span></span>

[<span data-ttu-id="f7a93-162">Školicí videa k Microsoftu 365 Business</span><span class="sxs-lookup"><span data-stu-id="f7a93-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
