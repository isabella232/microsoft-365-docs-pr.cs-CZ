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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Naučte se nastavit aplikaci Microsoft 365 Business.
ms.openlocfilehash: 7ab6ae095ae30f8ceb74be69fcee20f31977ae21
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "39818881"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="51e64-103">Nastavení aplikace Microsoft 365 Business v Průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="51e64-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="51e64-104">Na tomto videu můžete sledovat přehled programu Microsoft 365 Business Setup.</span><span class="sxs-lookup"><span data-stu-id="51e64-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="51e64-105">Pokud jste toto video našli, podívejte se na [kompletní tréninkové řady pro malé firmy a ty nové do společnosti Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="51e64-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="51e64-106">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="51e64-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="51e64-107">[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="51e64-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="51e64-108">Zakoupí-li společnost Microsoft 365 Business, máte možnost používat vlastní doménu nebo ji zakoupit během [zápisu](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="51e64-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="51e64-109">Pokud jste při přihlášení zakoupili novou doménu, je vaše doména nastavena a můžete se přesouvat a [přidávat uživatele a přiřazovat jim licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="51e64-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="51e64-110">Přidání domény k přizpůsobení přihlášení</span><span class="sxs-lookup"><span data-stu-id="51e64-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="51e64-111">Přihlaste se ke [středisku Microsoft 365 Admin Center](https://admin.microsoft.com) pomocí globálních pověření pro správu.</span><span class="sxs-lookup"><span data-stu-id="51e64-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="51e64-112">Chcete-li spustit průvodce, zvolte možnost **Přejít k instalačnímu programu** .</span><span class="sxs-lookup"><span data-stu-id="51e64-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Vyberte možnost přejít k nastavení.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="51e64-114">Na stránce **instalace aplikací sady Office** můžete aplikace volitelně nainstalovat do vlastního počítače.</span><span class="sxs-lookup"><span data-stu-id="51e64-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="51e64-115">V kroku **Přidat doménu** zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="51e64-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="51e64-116">Pokud jste během zápisu zakoupili doménu, nezobrazí se zde krok **Přidat doménu** .</span><span class="sxs-lookup"><span data-stu-id="51e64-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="51e64-117">Přejděte na místo pro [Přidání uživatelů](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="51e64-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Obrazovka stránky přizpůsobit přihlašovací stránku.](media/adddomain.png)

    
4. <span data-ttu-id="51e64-119">Postupujte podle pokynů průvodce a [vytvořte záznamy DNS u kteréhokoli poskytovatele hostitelských služeb DNS pro sadu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověřuje vlastní doménu.</span><span class="sxs-lookup"><span data-stu-id="51e64-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="51e64-120">Pokud znáte hostitele domény, podívejte se také na [pokyny týkající se hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="51e64-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="51e64-121">Pokud je poskytovatelem hostitelských služeb GoDaddy nebo jiný hostitel povolený s [připojením k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadný a budete automaticky požádáni o přihlášení a ověřování společnosti Microsoft ve vašem zastoupení.</span><span class="sxs-lookup"><span data-stu-id="51e64-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![U možnosti potvrdit přístup na stránce GoDaddy vyberte možnost ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="51e64-123">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="51e64-123">Add users and assign licenses</span></span>

<span data-ttu-id="51e64-124">Můžete přidat uživatele v průvodci, ale můžete je také [přidat později](add-users-m365b.md) v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="51e64-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="51e64-125">Navíc, pokud máte místní řadič domény, můžete přidat uživatele pomocí [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="51e64-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="51e64-126">Přidání uživatelů v Průvodci</span><span class="sxs-lookup"><span data-stu-id="51e64-126">Add users in the wizard</span></span>

<span data-ttu-id="51e64-127">Všichni uživatelé, které přidáte v průvodci, dostanou automaticky přiřazenu licenci Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="51e64-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Obrazovka stránky přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. <span data-ttu-id="51e64-129">Pokud vaše předplatné aplikace Microsoft 365 Business obsahuje existující uživatele (například pokud jste použili program Azure AD Connect), můžete jim nyní přiřadit licence.</span><span class="sxs-lookup"><span data-stu-id="51e64-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="51e64-130">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="51e64-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="51e64-131">Po přidání uživatelů budete mít také možnost sdílet pověření s novými uživateli, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="51e64-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="51e64-132">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="51e64-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="51e64-133">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="51e64-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="51e64-134">Pokud zvolíte použití domény. onmicrosoft nebo použijete Azure AD Connect pro nastavení uživatelů, tento krok se nezobrazí.</span><span class="sxs-lookup"><span data-stu-id="51e64-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="51e64-135">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="51e64-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="51e64-136">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="51e64-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="51e64-137">Pokud tomu tak není, [změňte nameservery tak, aby sadu Office 365 nastavil s jakýmkoli registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="51e64-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="51e64-138">Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte možnost **Přidat záznamy**.</span><span class="sxs-lookup"><span data-stu-id="51e64-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="51e64-139">Na stránce **Vyberte stránku služeb online** , přijměte všechny výchozí hodnoty a klepněte na tlačítko **Další**a na stránce hostitele DNS vyberte možnost **autorizovat** .</span><span class="sxs-lookup"><span data-stu-id="51e64-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="51e64-140">Pokud máte existující záznamy DNS s jinými hostiteli DNS (nejsou povoleny pro připojení k doméně), budete chtít spravovat své vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou propojeny.</span><span class="sxs-lookup"><span data-stu-id="51e64-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="51e64-141">Další informace naleznete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="51e64-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivuje stránku záznamů.](media/activaterecords.png)

2. <span data-ttu-id="51e64-143">Postupujte podle pokynů průvodce a e-maily a další služby budou nastaveny pro vás.</span><span class="sxs-lookup"><span data-stu-id="51e64-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="51e64-144">Ochrana organizace</span><span class="sxs-lookup"><span data-stu-id="51e64-144">Protect your organization</span></span> 

<span data-ttu-id="51e64-145">Zásady nastavené v průvodci jsou automaticky použity pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="51e64-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="51e64-146">Můžete také vytvořit další skupiny pro přiřazení zásad v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="51e64-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="51e64-147">Při **zvýšení ochrany před pokročilými internetovými hrozbami**se doporučuje přijmout výchozí hodnoty, které umožňují [systému Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) prohledávat soubory a odkazy v aplikacích sady Office.</span><span class="sxs-lookup"><span data-stu-id="51e64-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Obrazovka stránky zvýšení ochrany.](media/increasetreatprotection.png)


2. <span data-ttu-id="51e64-149">Pokud chcete **zabránit úniku citlivých datových** stránek, přijměte výchozí nastavení pro zapnutí funkce Zabránění ztrátám dat (DLP) sady Office 365 za účelem sledování citlivých dat v aplikacích sady Office a zabránění nechtěnému sdílení těchto dat mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="51e64-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="51e64-150">Na stránce **Chraňte data v sadě Office pro mobilní** stránku ponechejte správu mobilních aplikací, rozbalte nastavení a Prohlédněte si je a pak vyberte možnost **vytvořit zásadu správy mobilních aplikací**.</span><span class="sxs-lookup"><span data-stu-id="51e64-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Kopie obrazovky Chraňte data v sadě Office pro mobilní stránku.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="51e64-152">Zabezpečení systému Windows 10 počítačů</span><span class="sxs-lookup"><span data-stu-id="51e64-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="51e64-153">Na levém navigačním panelu vyberte **Nastavení** a potom v části zapnuto **a zabezpečení**zvolte zabezpečení **počítačů se systémem Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="51e64-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="51e64-154">Zvolte **zobrazení** pro začátek.</span><span class="sxs-lookup"><span data-stu-id="51e64-154">Choose **View** to get started.</span></span> <span data-ttu-id="51e64-155">Úplné pokyny naleznete v části [zabezpečení počítačů se systémem Windows 10](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="51e64-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="51e64-156">Nasadit sadu Office 365 Client Apps</span><span class="sxs-lookup"><span data-stu-id="51e64-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="51e64-157">Pokud jste při instalaci zvolili automatickou instalaci aplikací sady Office, budou aplikace nainstalovány do zařízení systému Windows 10, jakmile se uživatelé k Azure AD přihlašují z jejich zařízení se systémem Windows, pomocí svých pracovních pověření.</span><span class="sxs-lookup"><span data-stu-id="51e64-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="51e64-158">Informace o instalaci sady Office na mobilních zařízeních iOS nebo Android naleznete v tématu [nastavení mobilních zařízení pro Microsoft 365 Business Users](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="51e64-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="51e64-159">Sadu Office můžete nainstalovat také jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="51e64-159">You can also install Office individually.</span></span> <span data-ttu-id="51e64-160">Pokyny naleznete [v části instalace sady Office v počítači nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="51e64-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="51e64-161">Viz také</span><span class="sxs-lookup"><span data-stu-id="51e64-161">See also</span></span>

[<span data-ttu-id="51e64-162">Microsoft 365 Business Training video</span><span class="sxs-lookup"><span data-stu-id="51e64-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
