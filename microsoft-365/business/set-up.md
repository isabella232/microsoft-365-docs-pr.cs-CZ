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
description: Zjistěte, jak nastavit Microsoft 365 Business.
ms.openlocfilehash: 42a35810531b6abd5b22e5fdbce2c0cfea57b8d7
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074584"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="fc34b-103">Nastavení Průvodce instalací Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fc34b-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="fc34b-104">Přidání domény, uživatele a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="fc34b-104">Add your domain, users, and set up policies</span></span>

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="fc34b-106">Při koupi Microsoft 365 Business, máte možnost použít doménu vlastníte, nebo při nákupu [zápisu](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="fc34b-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="fc34b-107">Pokud jste zakoupili novou doménu při registraci, vaše doména je sada všech nahoru a můžete přesunout, chcete-li [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="fc34b-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="fc34b-108">Přidání přizpůsobit přihlašovací domény</span><span class="sxs-lookup"><span data-stu-id="fc34b-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="fc34b-109">Přihlášení k aplikaci [Microsoft 365 admin center](https://admin.microsoft.com) pomocí globální správce pověření.</span><span class="sxs-lookup"><span data-stu-id="fc34b-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="fc34b-110">Zvolte **Přidat k doméně** nebo **Přidání uživatelů** ke spuštění průvodce.</span><span class="sxs-lookup"><span data-stu-id="fc34b-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="fc34b-111">Pokud jste doménu zakoupili během přihlašování, není viz **Přidání domény** kroku zde.</span><span class="sxs-lookup"><span data-stu-id="fc34b-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="fc34b-112">Místo toho přejděte na [Přidat uživatele](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="fc34b-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Vyberte Přidat do domény.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="fc34b-114">V průvodci zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="fc34b-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Obrazovka přizpůsobit přihlašovací stránku.](media/personalizesignin.png)

    
4. <span data-ttu-id="fc34b-116">Postupujte podle kroků v průvodci [vytvořit DNS záznamy na jakékoliv DNS poskytovatele hostitelských služeb pro Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ověří, že jste vlastníkem domény.</span><span class="sxs-lookup"><span data-stu-id="fc34b-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="fc34b-117">Pokud víte, váš hostitel domény naleznete v tématu [zvláštní pokyny pro hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="fc34b-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="fc34b-118">Pokud svého poskytovatele hostingových služeb, GoDaddy, proces je jednoduchý a vás automaticky vyzve k přihlášení a ověření za vás společnost Microsoft:</span><span class="sxs-lookup"><span data-stu-id="fc34b-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na stránce potvrdit přístup GoDaddy vyberte ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="fc34b-120">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="fc34b-120">Add users and assign licenses</span></span>

<span data-ttu-id="fc34b-121">V průvodci můžete přidat uživatele, ale můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="fc34b-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="fc34b-122">Navíc pokud máte místní řadič domény, můžete přidat uživatele [Azure AD připojit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="fc34b-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="fc34b-123">V průvodci Přidat uživatele</span><span class="sxs-lookup"><span data-stu-id="fc34b-123">Add users in the wizard</span></span>

<span data-ttu-id="fc34b-124">Všichni uživatelé, které zadáte v průvodci získáte automaticky přiřazena licence Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="fc34b-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Obrazovka stránku přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. <span data-ttu-id="fc34b-126">Má-li vaše předplatné Microsoft 365 Business existujících uživatelů (například pokud používáte Azure AD připojit), dostanete možnost přiřazovat licence je nyní.</span><span class="sxs-lookup"><span data-stu-id="fc34b-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="fc34b-127">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="fc34b-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="fc34b-128">Po přidání uživatele se zobrazí také možnost sdílet pověření s novým uživatelům, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="fc34b-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="fc34b-129">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="fc34b-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="fc34b-130">Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="fc34b-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="fc34b-131">Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="fc34b-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="fc34b-132">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="fc34b-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="fc34b-133">Pokud používáte domény .onmicrosoft nebo lze nastavit uživatele Azure AD připojit, nezobrazí se tento krok.</span><span class="sxs-lookup"><span data-stu-id="fc34b-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="fc34b-134">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="fc34b-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="fc34b-135">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="fc34b-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="fc34b-136">Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="fc34b-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="fc34b-137">Pokud máte existující záznamy DNS, například existující web, můžete ke správě DNS záznamů a ujistěte se, že zachovat stávající služby připojení.</span><span class="sxs-lookup"><span data-stu-id="fc34b-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="fc34b-138">Viz [základní informace o doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) pro další informace.</span><span class="sxs-lookup"><span data-stu-id="fc34b-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Připojit domény stránky lze spravovat vlastní záznamy DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="fc34b-140">Postupujte podle pokynů v průvodci a e-mailů a dalších služeb bude nastavení pro vás.</span><span class="sxs-lookup"><span data-stu-id="fc34b-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="fc34b-141">Nastavit zásady zabezpečení a konfigurace zařízení</span><span class="sxs-lookup"><span data-stu-id="fc34b-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="fc34b-142">Zásady, které jste nastavili v Průvodci automaticky použity [skupiny zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="fc34b-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="fc34b-143">Můžete také vytvořit další skupiny přiřadit zásady v Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="fc34b-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="fc34b-144">**Ochranu pracovních souborů na mobilních zařízeních** možnost **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** je zapnutá ve výchozím nastavení.</span><span class="sxs-lookup"><span data-stu-id="fc34b-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="fc34b-145">Máte možnost zapnout **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních**, a to je doporučeno.</span><span class="sxs-lookup"><span data-stu-id="fc34b-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Snímek obrazovky chránit pracovní soubory na stránce Mobilní zařízení.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="fc34b-147">Rozbalte položku **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** zobrazí [výchozí hodnoty](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="fc34b-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Obrazovka výchozí hodnoty pro ochranu souborů na ztracené zařízení.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="fc34b-149">Vyberte **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních** a rozbalit a zobrazit [výchozí hodnoty](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="fc34b-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="fc34b-150">Doporučujeme přijmout výchozí hodnoty během instalace k vytvoření zásad aplikace pro Android, iOS a Windows 10, které platí pro všechny uživatele.</span><span class="sxs-lookup"><span data-stu-id="fc34b-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="fc34b-151">Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="fc34b-151">You can create more policies after setup completes.</span></span>

        ![Obrazovka nastavení ochrany souborů sady Office Mobile.](media/useraccessonmobile.png)

2. <span data-ttu-id="fc34b-153">Poslední krok na ochranu dat a zařízení umožňuje nastavit zásady zabezpečení Windows 10 zařízení.</span><span class="sxs-lookup"><span data-stu-id="fc34b-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="fc34b-154">Toto nastavení automaticky použito při připojení uživatele v systému Windows 10 pro vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="fc34b-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="fc34b-155">Můžete rozbalit **zabezpečení Windows 10 zařízení** zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="fc34b-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="fc34b-156">Můžete také [automaticky nainstalovat systém Office](install-office-on-windows-10-during-setup.md) na zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fc34b-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Obrazovka nastavení stránku konfigurace zařízení Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="fc34b-158">Nasazení aplikace klienta služeb Office 365</span><span class="sxs-lookup"><span data-stu-id="fc34b-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="fc34b-159">Pokud zvolíte automaticky nainstalovat Office apps v průběhu sada nahoru, nainstaluje soubor apps po uživatelé přihlášeni k Azure AD ze svých zařízení systému Windows pomocí pověření jejich práce na zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fc34b-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="fc34b-160">Chcete-li nainstalovat systém Office na mobilním iOS nebo Android zařízení, naleznete v tématu [nastavit mobilní zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="fc34b-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="fc34b-161">Office lze také nainstalovat samostatně.</span><span class="sxs-lookup"><span data-stu-id="fc34b-161">You can also install Office individually.</span></span> <span data-ttu-id="fc34b-162">Viz pokyny pro [instalaci sady Office na PC nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .</span><span class="sxs-lookup"><span data-stu-id="fc34b-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
