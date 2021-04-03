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
description: Zjistěte, jak nastavit Microsoft 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších možností.
ms.openlocfilehash: c8e2ca94f4947d4f9c69915d2fef410a6075bfed
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579908"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="7bcc7-103">Nastavení Microsoft 365 Business Premium v průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="7bcc7-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="7bcc7-104">V tomto videu najdete přehled nastavení Microsoftu 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="7bcc7-105">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="7bcc7-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="7bcc7-106">Když si koupíte Microsoft 365 Business Premium, máte možnost používat doménu, kterou vlastníte, nebo si ji koupit během [registrace](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="7bcc7-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="7bcc7-107">Pokud jste si při přihlášení koupili novou doménu, vaše doména je nastavená a můžete přejít na Přidat uživatele a [přiřadit licence.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="7bcc7-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="7bcc7-108">Přidání domény k přizpůsobení přihlášení</span><span class="sxs-lookup"><span data-stu-id="7bcc7-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="7bcc7-109">Přihlaste se [do Centra pro správu Microsoftu 365](https://admin.microsoft.com) pomocí přihlašovacích údajů globálního správce.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="7bcc7-110">Průvodce **spustíte tak,** že zvolíte Přejít na nastavení.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="7bcc7-112">Na **stránce Instalace aplikací Office** můžete aplikace volitelně nainstalovat na vlastní počítač.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="7bcc7-113">V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7bcc7-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="7bcc7-114">Pokud jste si doménu koupili během registrace, neuvidíte tady krok **Přidat** doménu.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="7bcc7-115">Přejděte místo [toho na Přidat](#add-users-and-assign-licenses) uživatele.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Snímek obrazovky s přizpůsobením přihlašovací stránky](../media/adddomain.png)

    
4. <span data-ttu-id="7bcc7-117">Podle pokynů v průvodci vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro [Microsoft 365,](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověří, že doménu vlastníte.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="7bcc7-118">Pokud znáte svého hostitele domény, přečtěte si taky pokyny [specifické pro hostitele](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="7bcc7-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="7bcc7-119">Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiným hostitelem povoleným s připojením domény [,](/office365/admin/get-help-with-domains/domain-connect)proces je snadný a automaticky se zobrazí dotaz, jestli se chcete přihlásit a nechat Microsoft ověřit vaším jménem.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stránce GoDaddy Confirm Access (Potvrdit přístup GoDaddy) vyberte Authorize (Autorizovat).](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="7bcc7-121">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="7bcc7-121">Add users and assign licenses</span></span>

<span data-ttu-id="7bcc7-122">Uživatele můžete přidat v průvodci, ale můžete je přidat [i později](../admin/add-users/add-users.md) v Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="7bcc7-123">Pokud máte místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="7bcc7-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="7bcc7-124">Přidání uživatelů v průvodci</span><span class="sxs-lookup"><span data-stu-id="7bcc7-124">Add users in the wizard</span></span>

<span data-ttu-id="7bcc7-125">Uživatelům, které přidáte v průvodci, se automaticky přiřadí licence Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Snímek obrazovky se stránkou Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. <span data-ttu-id="7bcc7-127">Pokud má vaše předplatné Microsoft 365 Business Premium stávající uživatele (například pokud jste používali Azure AD Connect), můžete jim teď přiřadit licence.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="7bcc7-128">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="7bcc7-129">Po přidání uživatelů získáte taky možnost sdílet přihlašovací údaje s novými uživateli, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="7bcc7-130">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="7bcc7-131">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="7bcc7-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="7bcc7-132">Pokud jste se rozhodli použít doménu .onmicrosoft nebo jste k nastavení uživatelů použili Azure AD Connect, tento krok se vám neuvidí.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="7bcc7-133">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="7bcc7-134">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="7bcc7-135">Pokud ne, změňte názvové servery tak, aby [nastavily Microsoft 365 u jakéhokoli doménového registrátora](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span><span class="sxs-lookup"><span data-stu-id="7bcc7-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="7bcc7-136">Pokud máte existující záznamy DNS, například existující web, ale váš hostitel DNS je povolený pro připojení domény [,](/office365/admin/get-help-with-domains/domain-connect)zvolte Přidat záznamy **za mě**.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="7bcc7-137">Na stránce **Zvolte online služby** přijměte všechna výchozí nastavení a  zvolte Další a na stránce hostitele DNS zvolte Autorizovat. </span><span class="sxs-lookup"><span data-stu-id="7bcc7-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="7bcc7-138">Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povolené pro připojení domény), budete chtít spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojené.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="7bcc7-139">Další [informace najdete v tématu Základy](/office365/admin/get-help-with-domains/dns-basics) domény.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Stránka Aktivace záznamů](../media/activaterecords.png)

2. <span data-ttu-id="7bcc7-141">Postupujte podle pokynů v průvodci a budete mít nastavené e-maily a další služby.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="7bcc7-142">Ochrana vaší organizace</span><span class="sxs-lookup"><span data-stu-id="7bcc7-142">Protect your organization</span></span> 

<span data-ttu-id="7bcc7-143">Zásady, které nastavíte v průvodci, se automaticky použijí ve skupině [Zabezpečení](/office365/admin/create-groups/compare-groups#security-groups) s *názvem Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="7bcc7-144">V Centru pro správu můžete taky vytvořit další skupiny, ke které chcete přiřadit zásady.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="7bcc7-145">V části Zvýšení ochrany **před** pokročilými kybernetickými hrozbami doporučujeme přijmout výchozí nastavení, aby [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) prohledl soubory a odkazy v aplikacích Office.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. <span data-ttu-id="7bcc7-147">Na  stránce Zabránit úniku citlivých dat přijměte výchozí nastavení, jak zapnout Office 365 Data Loss Prevention (DLP) ke sledování citlivých dat v aplikacích Office a zabránit nechtěnému sdílení těchto dat mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="7bcc7-148">Na stránce **Chraňte data v Office** pro mobilní zařízení nechte správu mobilních aplikací zak dispozici, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit zásady správy **mobilních aplikací.**</span><span class="sxs-lookup"><span data-stu-id="7bcc7-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Snímek obrazovky s zamknout data v Office pro mobilní stránku](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="7bcc7-150">Zabezpečení počítačů s Windows 10</span><span class="sxs-lookup"><span data-stu-id="7bcc7-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="7bcc7-151">V levém navigačním panelu **vyberte** Nastavení a potom v části Přihlášení a **zabezpečení** zvolte Zabezpečit počítače s **Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="7bcc7-152">Pokud **chcete začít,** zvolte Zobrazení.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-152">Choose **View** to get started.</span></span> <span data-ttu-id="7bcc7-153">Úplné pokyny najdete v tématu Zabezpečení [počítačů s Windows 10.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="7bcc7-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="7bcc7-154">Nasazení klientských aplikací Office 365</span><span class="sxs-lookup"><span data-stu-id="7bcc7-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="7bcc7-155">Pokud jste se během instalace rozhodli automaticky instalovat aplikace Office, aplikace se nainstalují na zařízení s Windows 10, jakmile se uživatelé ze svých zařízení s Windows k Azure AD přihlásili pomocí svých pracovních přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="7bcc7-156">Informace o instalaci Office na mobilní zařízení s iOS nebo Androidem najdete v tématu Nastavení mobilních zařízení [pro uživatele Microsoftu 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7bcc7-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="7bcc7-157">Office můžete nainstalovat také jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="7bcc7-157">You can also install Office individually.</span></span> <span data-ttu-id="7bcc7-158">Pokyny [najdete v článku Instalace Office na PC nebo Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="7bcc7-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="7bcc7-159">Viz také</span><span class="sxs-lookup"><span data-stu-id="7bcc7-159">See also</span></span>

[<span data-ttu-id="7bcc7-160">Školicí videa k Microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="7bcc7-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
