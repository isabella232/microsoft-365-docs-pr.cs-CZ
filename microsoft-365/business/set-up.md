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
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="e4a96-103">Nastavení Microsoft 365 Business Premium v Průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="e4a96-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="e4a96-104">V tomto videu najdete přehled nastavení Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e4a96-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="e4a96-105">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="e4a96-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="e4a96-106">Když si koupíte Microsoft 365 Business Premium, můžete použít doménu, kterou vlastníte, nebo si ji koupit během [zápisu](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="e4a96-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="e4a96-107">Pokud jste při registraci zakoupili novou doménu, bude vaše doména nastavovaná a můžete se přesouvat a [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="e4a96-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="e4a96-108">Přidání domény pro personalizaci přihlášení</span><span class="sxs-lookup"><span data-stu-id="e4a96-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="e4a96-109">Přihlaste se do [centra pro správu Microsoft 365](https://admin.microsoft.com) pomocí přihlašovacích údajů globálního správce.</span><span class="sxs-lookup"><span data-stu-id="e4a96-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="e4a96-110">Kliknutím **na Přejít na nastavení** spusťte průvodce.</span><span class="sxs-lookup"><span data-stu-id="e4a96-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Vyberte Přejít na nastavení.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="e4a96-112">Na stránce **nainstalovat aplikace Office** můžete volitelně nainstalovat aplikace na počítači.</span><span class="sxs-lookup"><span data-stu-id="e4a96-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="e4a96-113">V kroku **Přidat doménu** zadejte název domény, který chcete použít (třeba contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e4a96-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e4a96-114">Pokud jste během registrace zakoupili doménu, nebudete tady zde **Přidat krok pro přidání domény** .</span><span class="sxs-lookup"><span data-stu-id="e4a96-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="e4a96-115">Přejděte na [Přidat uživatele](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="e4a96-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Snímek obrazovky s přidanou přihlašovací stránkou](../media/adddomain.png)

    
4. <span data-ttu-id="e4a96-117">Podle pokynů v průvodci [vytvořte záznamy DNS u kteréhokoli poskytovatele hostingu DNS pro Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověří, že jste vlastníkem domény.</span><span class="sxs-lookup"><span data-stu-id="e4a96-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="e4a96-118">Pokud znáte hostitele domény, přečtěte si také [pokyny pro hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="e4a96-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="e4a96-119">Pokud je váš poskytovatel hostingu GoDaddy nebo je povolený jiný hostitel se službou [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadno přihlášený a Vy se automaticky zobrazí výzva k přihlášení a aby Microsoft ověřil váš účet.</span><span class="sxs-lookup"><span data-stu-id="e4a96-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Na stránce potvrzení přístupu GoDaddy vyberte autorizovat.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="e4a96-121">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="e4a96-121">Add users and assign licenses</span></span>

<span data-ttu-id="e4a96-122">Uživatele můžete do průvodce Přidat, ale můžete je taky [přidat později](add-users-m365b.md) v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="e4a96-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="e4a96-123">Pokud máte místní řadič domény, můžete přidat uživatele pomocí [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e4a96-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="e4a96-124">Přidání uživatelů v Průvodci</span><span class="sxs-lookup"><span data-stu-id="e4a96-124">Add users in the wizard</span></span>

<span data-ttu-id="e4a96-125">Všichni uživatelé, které přidáte do průvodce, získají automaticky licenci Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e4a96-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Snímek obrazovky se stránkou přidat nové uživatele v Průvodci](../media/addnewuserspage.png)

1. <span data-ttu-id="e4a96-127">Pokud vaše předplatné Microsoft 365 Business Premium má existující uživatele (například pokud jste použili Azure AD Connect), získáte k těmto možnostem přiřazení licencí.</span><span class="sxs-lookup"><span data-stu-id="e4a96-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="e4a96-128">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="e4a96-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="e4a96-129">Po přidání uživatelů můžete také sdílet přihlašovací údaje s novými přidanými uživateli.</span><span class="sxs-lookup"><span data-stu-id="e4a96-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="e4a96-130">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="e4a96-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="e4a96-131">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="e4a96-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="e4a96-132">Pokud jste se rozhodli použít doménu. doména společnosti Microsoft nebo použili Azure AD Connect k nastavení uživatelů, tento krok se nezobrazuje.</span><span class="sxs-lookup"><span data-stu-id="e4a96-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="e4a96-133">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="e4a96-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="e4a96-134">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="e4a96-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="e4a96-135">Pokud to nepomůže, [změňte názvové servery na nastavení Microsoft 365 s libovolným doménovým registrátorem](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="e4a96-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="e4a96-136">Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte **Přidat záznamy pro mě**.</span><span class="sxs-lookup"><span data-stu-id="e4a96-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="e4a96-137">Na stránce **Vyberte si online služby** potvrďte všechna výchozí nastavení a zvolte **Další**a zvolte **autorizovat** na stránce hostitele DNS.</span><span class="sxs-lookup"><span data-stu-id="e4a96-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="e4a96-138">Pokud máte existující záznamy DNS s jinými hostiteli DNS (není povolené pro Domain Connect), budete chtít spravovat vlastní záznamy DNS, abyste měli jistotu, že stávající služby zůstanou připojené.</span><span class="sxs-lookup"><span data-stu-id="e4a96-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="e4a96-139">Další informace najdete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="e4a96-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Stránka aktivace záznamů](../media/activaterecords.png)

2. <span data-ttu-id="e4a96-141">Postupujte podle pokynů v průvodci a e-mail a další služby budou pro vás nastaveny.</span><span class="sxs-lookup"><span data-stu-id="e4a96-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="e4a96-142">Ochrana organizace</span><span class="sxs-lookup"><span data-stu-id="e4a96-142">Protect your organization</span></span> 

<span data-ttu-id="e4a96-143">Zásady, které nastavíte v průvodci, se automaticky použijí pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="e4a96-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="e4a96-144">Můžete taky vytvořit další skupiny pro přiřazení zásad do centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="e4a96-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="e4a96-145">Na **zvýšení ochrany před rozšířenými internetovými hrozbami**se doporučuje přijmout výchozí nastavení, aby aplikace Office [365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) prohledala soubory a odkazy v aplikacích Office.</span><span class="sxs-lookup"><span data-stu-id="e4a96-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Snímek obrazovky se stránkou zvýšení ochrany](../media/increasetreatprotection.png)


2. <span data-ttu-id="e4a96-147">Na stránce **zabránění únikům citlivých dat** přijměte výchozí hodnoty, abyste zapnuli ochranu před nevracením dat v Office 365, která sledují citlivá data v aplikacích Office a zabrání nechtěnému sdílení těchto funkcí mimo vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="e4a96-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="e4a96-148">Na stránce **chránit data v Office pro mobil** opustit správu mobilních aplikací, rozbalte nastavení a zkontrolujte je a pak vyberte **vytvořit zásadu správy mobilních aplikací**.</span><span class="sxs-lookup"><span data-stu-id="e4a96-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Snímek obrazovky s ochranou dat na stránce Office pro mobilní zařízení](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="e4a96-150">Zabezpečení počítačů s Windows 10</span><span class="sxs-lookup"><span data-stu-id="e4a96-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="e4a96-151">Na levém navigačním panelu vyberte **Nastavení** a pak v části **přihlášení a zabezpečení**zvolte **zabezpečit počítače s Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="e4a96-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="e4a96-152">Začněte tím, že zvolíte **zobrazení** .</span><span class="sxs-lookup"><span data-stu-id="e4a96-152">Choose **View** to get started.</span></span> <span data-ttu-id="e4a96-153">Podrobné pokyny najdete v tématu [zabezpečení počítačů s Windows 10](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="e4a96-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="e4a96-154">Nasazení klientských aplikací Office 365</span><span class="sxs-lookup"><span data-stu-id="e4a96-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="e4a96-155">Pokud jste se při instalaci rozhodli automaticky nainstalovat aplikace Office, budou se tyto aplikace instalovat na zařízení s Windows 10, jakmile se uživatelé přihlásí ke službě Azure AD ze svých zařízení s Windows, pomocí svých uživatelských přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="e4a96-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="e4a96-156">Pokud chcete nainstalovat Office na mobilní zařízení s iOS nebo Androidem, přečtěte si článek [nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="e4a96-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="e4a96-157">Office můžete také nainstalovat jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="e4a96-157">You can also install Office individually.</span></span> <span data-ttu-id="e4a96-158">Pokyny najdete v článku [instalace Office na PC nebo Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="e4a96-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="e4a96-159">Viz také</span><span class="sxs-lookup"><span data-stu-id="e4a96-159">See also</span></span>

[<span data-ttu-id="e4a96-160">Školicí kurzy pro Microsoft 365 for Business</span><span class="sxs-lookup"><span data-stu-id="e4a96-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
