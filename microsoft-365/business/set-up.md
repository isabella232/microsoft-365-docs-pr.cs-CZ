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
description: Zjistěte, jak nastavit Microsoft 365 Business Premium, včetně přidání domény a uživatelů, nastavení zásad zabezpečení a dalších možností.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044724"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="7bbd7-103">Nastavení Microsoft 365 Business Premium v průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="7bbd7-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="7bbd7-104">V tomto videu najdete přehled nastavení Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="7bbd7-105">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="7bbd7-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="7bbd7-106">Při nákupu Microsoftu 365 Business Premium máte možnost používat doménu, kterou vlastníte, nebo si ji zakoupit během [registrace.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="7bbd7-107">Pokud jste si koupili novou doménu, je vaše doména nastavená a můžete přejít na Přidat uživatele a přiřadit [licence.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="7bbd7-108">Přidání domény pro přizpůsobení přihlašování</span><span class="sxs-lookup"><span data-stu-id="7bbd7-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="7bbd7-109">Přihlaste se do Centra pro [správu Microsoftu 365](https://admin.microsoft.com) pomocí svých přihlašovacích údajů globálního správce.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="7bbd7-110">Průvodce **spustíte tak,** že zvolíte Přejít do nastavení.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Vyberte Přejít do nastavení.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="7bbd7-112">Na stránce **Instalace aplikací Office** si můžete volitelně nainstalovat aplikace na vlastní počítač.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="7bbd7-113">V kroku **Přidat doménu** zadejte název domény, který chcete použít (třeba contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7bbd7-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="7bbd7-114">Pokud jste si koupili doménu během registrace, neuvidíte **tady** krok Přidat doménu.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="7bbd7-115">Místo toho [přejděte na možnost Přidat](#add-users-and-assign-licenses) uživatele.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Snímek obrazovky s přihlašovací stránkou Přizpůsobení](../media/adddomain.png)

    
4. <span data-ttu-id="7bbd7-117">Postupujte podle pokynů průvodce a vytvořte záznamy DNS u libovolného poskytovatele hostingu DNS pro [Microsoft 365,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) který ověří, že doménu vlastníte.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="7bbd7-118">Pokud hostitele domény znáte, podívejte se také na [konkrétní pokyny pro hostitele.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="7bbd7-119">Pokud je vaším poskytovatelem hostingu GoDaddy nebo jiným hostitelem povoleným připojením [domény,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)proces je snadný a automaticky se zobrazí žádost o přihlášení a ověření společnosti Microsoft vaším jménem.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stránce Potvrdit přístup na GoDaddy vyberte Autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="7bbd7-121">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="7bbd7-121">Add users and assign licenses</span></span>

<span data-ttu-id="7bbd7-122">Uživatele můžete přidat v průvodci, ale můžete je přidat [i později v](add-users-m365b.md) Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="7bbd7-123">Pokud máte také místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="7bbd7-124">Přidání uživatelů v průvodci</span><span class="sxs-lookup"><span data-stu-id="7bbd7-124">Add users in the wizard</span></span>

<span data-ttu-id="7bbd7-125">Všichni uživatelé, které přidáte v průvodci, se automaticky přiřadí licenci Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Snímek obrazovky se stránkou Přidat nové uživatele v průvodci](../media/addnewuserspage.png)

1. <span data-ttu-id="7bbd7-127">Pokud vaše předplatné Microsoft 365 Business Premium již uživatele má (například pokud jste používali službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="7bbd7-128">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="7bbd7-129">Po přidání uživatelů budete mít taky možnost přihlašovací údaje sdílet s novými uživateli, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="7bbd7-130">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="7bbd7-131">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="7bbd7-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="7bbd7-132">Pokud jste se rozhodli použít doménu .onmicrosoft nebo k nastavení uživatelů použili Azure AD Connect, tento krok se vám neukaží.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="7bbd7-133">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="7bbd7-134">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="7bbd7-135">Pokud ne, změňte [názvové servery, abyste nastavili Microsoft 365 u libovolného doménového registrátora.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="7bbd7-136">Pokud máte existující záznamy DNS, třeba existující web, ale hostitel DNS má povolené připojení k [doméně,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)zvolte Přidat **záznamy za mě.**</span><span class="sxs-lookup"><span data-stu-id="7bbd7-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="7bbd7-137">Na stránce **Zvolit online služby** přijměte výchozí nastavení a zvolte  Další a na stránce hostitele DNS zvolte Autorizovat.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="7bbd7-138">Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povoleno pro připojení k doméně), můžete spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojeny.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="7bbd7-139">Další [informace najdete v základních](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) informacích o doméně.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Stránka Aktivace záznamů](../media/activaterecords.png)

2. <span data-ttu-id="7bbd7-141">Postupujte podle pokynů v průvodci a nastavte e-mail a další služby.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="7bbd7-142">Ochrana organizace</span><span class="sxs-lookup"><span data-stu-id="7bbd7-142">Protect your organization</span></span> 

<span data-ttu-id="7bbd7-143">Zásady nastavené v průvodci se automaticky použijí na skupinu [zabezpečení s](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) názvem *Všichni uživatelé.*</span><span class="sxs-lookup"><span data-stu-id="7bbd7-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="7bbd7-144">V Centru pro správu můžete taky vytvořit další skupiny, ke které budete zásady přiřazovat.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="7bbd7-145">Pokud chcete **zvýšit** ochranu před pokročilými kybernetickými hrozbami, doporučujeme vám přijmout výchozí nastavení, abyste v aplikacích [Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) 2013 pustit funkci Rozšířená ochrana před hrozbami a odkazy.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Snímek obrazovky se stránkou Zvýšit ochranu](../media/increasetreatprotection.png)


2. <span data-ttu-id="7bbd7-147">Na  stránce Zabránit úniku citlivých dat přijměte výchozí nastavení, které zapne funkci Ochrana před únikem informací (DLP) v Office 365 za cílem sledovat citlivá data v aplikacích Office a zabránit náhodnému sdílení těchto dat mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="7bbd7-148">Na stránce **Chránit data v Office** pro mobilní zařízení nechte správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte Vytvořit zásadu správy **mobilních aplikací.**</span><span class="sxs-lookup"><span data-stu-id="7bbd7-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Snímek obrazovky se stránkou Zamknout data v Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="7bbd7-150">Zabezpečení počítačů s Windows 10</span><span class="sxs-lookup"><span data-stu-id="7bbd7-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="7bbd7-151">Na levém navigačním panelu **vyberte** Nastavení a pak v části Přihlášení a zabezpečení zvolte Zabezpečení počítačů s Windows **10.**</span><span class="sxs-lookup"><span data-stu-id="7bbd7-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="7bbd7-152">Abyste **s tím začali,** zvolte Zobrazit.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-152">Choose **View** to get started.</span></span> <span data-ttu-id="7bbd7-153">Úplné pokyny najdete v článku o zabezpečení [počítačů s Windows 10.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="7bbd7-154">Nasazení klientských aplikací Office 365</span><span class="sxs-lookup"><span data-stu-id="7bbd7-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="7bbd7-155">Pokud jste během instalace zvolili automatickou instalaci aplikací Office, aplikace se na zařízení s Windows 10 nainstalují, jakmile se uživatelé ze svých zařízení s Windows na svém zařízení s Windows k Azure AD přihlásili pomocí svých pracovních přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="7bbd7-156">Informace o instalaci Office na mobilní zařízení s iOS nebo Androidem najdete v tématu Nastavení mobilních zařízení pro [uživatele Microsoft 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="7bbd7-157">Můžete také nainstalovat Office jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="7bbd7-157">You can also install Office individually.</span></span> <span data-ttu-id="7bbd7-158">Pokyny [najdete v článku o instalaci Office na PC nebo Mac.](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="7bbd7-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="7bbd7-159">Viz také</span><span class="sxs-lookup"><span data-stu-id="7bbd7-159">See also</span></span>

[<span data-ttu-id="7bbd7-160">Školicí videa pro Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="7bbd7-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
