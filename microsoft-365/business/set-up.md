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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660743"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="68965-103">Nastavení Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="68965-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="68965-104">Před započetím práce, podrobnosti najdete v části [Získat obchodní 365 Microsoft](get-microsoft-365-business.md) zápisu.</span><span class="sxs-lookup"><span data-stu-id="68965-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="68965-105">Podívejte se na [krátké video návod, jak nastavit Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) pomocí nastavení průvodce, a pokud nemáte služby Active Directory v prostorách</span><span class="sxs-lookup"><span data-stu-id="68965-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="68965-106">Přehled</span><span class="sxs-lookup"><span data-stu-id="68965-106">Overview</span></span>

<span data-ttu-id="68965-107">Většina nastavení kroky lze provést v Průvodci instalací, ale jsou také uvedeny další možnosti.</span><span class="sxs-lookup"><span data-stu-id="68965-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="68965-108">[Přidat do domény](#add-your-domain-to-personalize-sign-in) (Pokud jste si koupili své domény při [přihlášení](sign-up.md), tento krok je již proveden.)</span><span class="sxs-lookup"><span data-stu-id="68965-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="68965-109">Přidáte uživatele.</span><span class="sxs-lookup"><span data-stu-id="68965-109">Add users.</span></span> <span data-ttu-id="68965-110">Lze provést třemi způsoby:</span><span class="sxs-lookup"><span data-stu-id="68965-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="68965-111">Podle pokynů [Průvodce instalací](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="68965-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="68965-112">Používá pro synchronizaci adresářů přidat [uživatele Azure AD připojit pomocí](#add-users-by-using-azure-ad-connect) služby Active directory v prostorách.</span><span class="sxs-lookup"><span data-stu-id="68965-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="68965-113">Můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="68965-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="68965-114">Nastavit zásady zabezpečení a konfigurace zařízení.</span><span class="sxs-lookup"><span data-stu-id="68965-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="68965-115">Lze provést třemi způsoby:</span><span class="sxs-lookup"><span data-stu-id="68965-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="68965-116">Podle pokynů [Průvodce instalací](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="68965-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="68965-117">V [Centru správy](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="68965-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="68965-118">V aplikaci [Centrum pro správu Intune](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="68965-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="68965-119">Nastavit a spravovat zařízení v systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="68965-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="68965-120">Při připojení zařízení WIndows 10 k Azure AD získat k němu použity všechny zásady.</span><span class="sxs-lookup"><span data-stu-id="68965-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="68965-121">Nastavení konfigurace zařízení Windows 10 podle pokynů [Průvodce instalací](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="68965-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="68965-122">[Nové Windows 10 zařízení](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) připojte k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68965-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="68965-123">Připojte [existující zařízení s Windows 10](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68965-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="68965-124">Instalace Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="68965-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="68965-125">Office v zařízení Windows může automaticky instalovat pomocí [Průvodce instalací](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="68965-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="68965-126">Automaticky [nainstalovat systém Office](auto-install-or-uninstall-office.md) z středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="68965-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="68965-127">Umožní uživatelům [instalaci aplikací sady Office](https://docs.microsoft.com/office365/admin/setup/install-applications) pro systém Windows a zařízení.</span><span class="sxs-lookup"><span data-stu-id="68965-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="68965-128">Nastavte další zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="68965-128">Set up additional security.</span></span>
    - <span data-ttu-id="68965-129">Průvodce instalací přidá zásady zabezpečení vašeho zařízení, ale můžete také využít výhod [Další bezpečnostní](#additional-security-settings) funkce, které umožňuje zabezpečené vaše data, účty a e-mailů.</span><span class="sxs-lookup"><span data-stu-id="68965-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="68965-130">Přidání domény, uživatele a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="68965-130">Add your domain, users and set up policies</span></span>

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="68965-132">Při koupi Microsoft 365 Business, máte možnost použít doménu vlastníte, nebo při nákupu [zápisu](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="68965-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="68965-133">Pokud jste zakoupili novou doménu při registraci, vaše doména je sada všech nahoru a můžete přesunout, chcete-li [Přidat uživatele a přiřadit licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="68965-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="68965-134">Přidání přizpůsobit přihlašovací domény</span><span class="sxs-lookup"><span data-stu-id="68965-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="68965-135">Přihlášení k aplikaci [Microsoft 365 admin center](https://admin.microsoft.com) pomocí globální správce pověření.</span><span class="sxs-lookup"><span data-stu-id="68965-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="68965-136">Vyberte **Přidat do domény** , spusťte průvodce.</span><span class="sxs-lookup"><span data-stu-id="68965-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Vyberte Přidat do domény.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="68965-138">V průvodci zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="68965-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Obrazovka přizpůsobit přihlašovací stránku.](media/personalizesignin.png)

    
4. <span data-ttu-id="68965-140">Postupujte podle kroků v průvodci [vytvořit DNS záznamy na jakékoliv DNS poskytovatele hostitelských služeb pro Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) ověří, že jste vlastníkem domény.</span><span class="sxs-lookup"><span data-stu-id="68965-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="68965-141">Pokud víte, váš hostitel domény naleznete v tématu [zvláštní pokyny pro hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="68965-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="68965-142">Pokud svého poskytovatele hostingových služeb, GoDaddy, proces je jednoduchý a vás automaticky vyzve k přihlášení a ověření za vás společnost Microsoft:</span><span class="sxs-lookup"><span data-stu-id="68965-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Na stránce potvrdit přístup GoDaddy vyberte ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="68965-144">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="68965-144">Add users and assign licenses</span></span>

<span data-ttu-id="68965-145">V průvodci můžete přidat uživatele, ale můžete také [Přidat uživatele později](add-users-m365b.md) ve středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="68965-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="68965-146">Navíc pokud máte místní řadič domény, můžete přidat uživatele [Azure AD připojit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="68965-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="68965-147">V průvodci Přidat uživatele</span><span class="sxs-lookup"><span data-stu-id="68965-147">Add users in the wizard</span></span>

<span data-ttu-id="68965-148">Všichni uživatelé, které zadáte v průvodci získáte automaticky přiřazena licence Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="68965-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="68965-149">Pokud máte místní řadič domény a používáte služby Active Directory, naleznete v článku [ddd uživatelů pomocí Azure AD připojit](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="68965-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Obrazovka stránku přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. <span data-ttu-id="68965-p106">Pokud vaše předplatné Microsoft 365 Business již uživatele má (například pokud jste použili službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní. Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="68965-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="68965-153">Po přidání uživatele se zobrazí také možnost sdílet pověření s novým uživatelům, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="68965-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="68965-154">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="68965-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="68965-155">Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="68965-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="68965-156">Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="68965-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="68965-157">Přidání uživatele pomocí Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="68965-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="68965-158">Pokud máte místní řadič domény se službou Active Directory, synchronizovat pomocí [Azure AD připojit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)uživatelé s Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="68965-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="68965-159">Dokončete tuto před spuštěním Průvodce instalací.</span><span class="sxs-lookup"><span data-stu-id="68965-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="68965-160">Si můžete stáhnout v Centru pro správu:</span><span class="sxs-lookup"><span data-stu-id="68965-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="68965-161">Přejděte na **uživatele** \> **aktivních uživatelů**vyberte na tři tečky v horní části stránky a potom vyberte **adresář synchronizace** Azure AD připojit stáhnout.</span><span class="sxs-lookup"><span data-stu-id="68965-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Na stránce aktivní uživatele vyberte elipsy > adresář snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="68965-163">Pokud uživatelé vytvářet tímto způsobem, musíte stále k nim přiřadit licence ve středisku pro správce.</span><span class="sxs-lookup"><span data-stu-id="68965-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="68965-164">Získat přístup k doméně aplikace a zařízení</span><span class="sxs-lookup"><span data-stu-id="68965-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="68965-165">Pokud chcete získat přístup k doméně aplikace a zařízení, přečtěte si dva jiný způsob povolení, které v následujících článcích:</span><span class="sxs-lookup"><span data-stu-id="68965-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="68965-166">Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="68965-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="68965-167">Toto je doporučený způsob.</span><span class="sxs-lookup"><span data-stu-id="68965-167">This is the recommended way.</span></span>

- [<span data-ttu-id="68965-168">Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="68965-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="68965-169">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="68965-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="68965-170">Pokud používáte domény .onmicrosoft nebo lze nastavit uživatele Azure AD připojit, nezobrazí se tento krok.</span><span class="sxs-lookup"><span data-stu-id="68965-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="68965-171">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="68965-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="68965-172">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="68965-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="68965-173">Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="68965-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="68965-174">Pokud máte existující záznamy DNS, například existující web, můžete ke správě DNS záznamů a ujistěte se, že zachovat stávající služby připojení.</span><span class="sxs-lookup"><span data-stu-id="68965-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="68965-175">Viz [základní informace o doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) pro další informace.</span><span class="sxs-lookup"><span data-stu-id="68965-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Připojit domény stránky lze spravovat vlastní záznamy DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="68965-177">Postupujte podle pokynů v průvodci a e-mailů a dalších služeb bude nastavení pro vás.</span><span class="sxs-lookup"><span data-stu-id="68965-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="68965-178">Nastavit zásady zabezpečení a konfigurace zařízení</span><span class="sxs-lookup"><span data-stu-id="68965-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="68965-179">Tyto zásady se týkají všech uživatelů udělíte licenci nebo na skupinu uživatelů a pokud se rozhodnete přiřadit různé zásady pro více uživatelů.</span><span class="sxs-lookup"><span data-stu-id="68965-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="68965-180">Nastavení zásad v Průvodci</span><span class="sxs-lookup"><span data-stu-id="68965-180">Set up policies in the wizard</span></span>

<span data-ttu-id="68965-181">Zásady, které jste nastavili v Průvodci automaticky použity [skupiny zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) s názvem *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="68965-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="68965-182">**Ochranu pracovních souborů na mobilních zařízeních** možnost **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** je zapnutá ve výchozím nastavení.</span><span class="sxs-lookup"><span data-stu-id="68965-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="68965-183">Máte možnost zapnout **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních**, a to je doporučeno.</span><span class="sxs-lookup"><span data-stu-id="68965-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Snímek obrazovky chránit pracovní soubory na stránce Mobilní zařízení.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="68965-185">Jestliže rozbalíte **chránit pracovní soubory, pokud jsou ztráty nebo krádeže zařízení**, jsou vybrány [výchozí hodnoty](protect-work-files-on-lost-or-stolen-device.md) :</span><span class="sxs-lookup"><span data-stu-id="68965-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Obrazovka výchozí hodnoty pro ochranu souborů na ztracené zařízení.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="68965-187">Pokud vyberete **Spravovat přístup uživatelů k souborů sady Office na mobilních zařízeních** a rozbalte ji, [výchozí hodnoty](manage-user-access-on-mobile-devices.md) jsou zobrazeny.</span><span class="sxs-lookup"><span data-stu-id="68965-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="68965-188">Doporučujeme vám přijmou během instalace výchozí hodnoty, abyste vytvořili zásady aplikací pro Android, iOS a Windows 10, které platí pro všechny uživatele.</span><span class="sxs-lookup"><span data-stu-id="68965-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="68965-189">Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="68965-189">You can create more policies after setup completes.</span></span>

        ![Obrazovka nastavení ochrany souborů sady Office Mobile.](media/useraccessonmobile.png)

2. <span data-ttu-id="68965-191">Poslední krok na ochranu dat a zařízení umožňuje nastavit zásady zabezpečení Windows 10 zařízení.</span><span class="sxs-lookup"><span data-stu-id="68965-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="68965-192">Toto nastavení automaticky použito při připojení uživatele v systému Windows 10 pro vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="68965-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="68965-193">Můžete rozbalit **zabezpečení Windows 10 zařízení** zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="68965-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="68965-194">Můžete také [automaticky nainstalovat systém Office](install-office-on-windows-10-during-setup.md) na zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="68965-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Obrazovka nastavení stránku konfigurace zařízení Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="68965-196">Úprava nebo přidání zásady v Centru pro správu</span><span class="sxs-lookup"><span data-stu-id="68965-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="68965-197">Pro odkazy na témata týkající se zobrazení a úprava ochrany zařízení a aplikace zásady, naleznete v tématu [Správa Microsoft 365 Business](manage.md) a jak odstranit nebo obnovit uživatelská zařízení.</span><span class="sxs-lookup"><span data-stu-id="68965-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="68965-198">Nasazení a správa Windows 10</span><span class="sxs-lookup"><span data-stu-id="68965-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="68965-199">V tématu Ruční připojení k Azure AD, buď při instalaci nových počítačů nebo změnou přihlašovacího profilu pro stávající počítače [Nastavení systému Windows zařízení pro uživatele Microsoft 365 Business](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="68965-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="68965-200">Chcete-li nastavit nové zařízení pomocí Autopilot</span><span class="sxs-lookup"><span data-stu-id="68965-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="68965-201">[Autopilot systému Windows](add-autopilot-devices-and-profile.md) lze nakonfigurovat automaticky **Nová** zařízení Windows 10 pro uživatele, ale může být jednodušší získat [partnera](https://www.microsoft.com/solution-providers/search) , který lze provést za vás.</span><span class="sxs-lookup"><span data-stu-id="68965-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="68965-202">Můžete také přejít na [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) a zeptejte se odborníků cloud technologie nastavit nová zařízení, které zakoupíte, vám.</span><span class="sxs-lookup"><span data-stu-id="68965-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="68965-203">Přístup k místním prostředkům</span><span class="sxs-lookup"><span data-stu-id="68965-203">Access on-premises resources</span></span>

<span data-ttu-id="68965-204">Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních.</span><span class="sxs-lookup"><span data-stu-id="68965-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="68965-205">Postupujte podle kroků v [doméně zařízení Windows 10, které jsou spravovány Microsoft 365 Business povolit](manage-windows-devices.md) toto nastavení.</span><span class="sxs-lookup"><span data-stu-id="68965-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="68965-206">Toto je upřednostňovaný způsob a zařízení v tomto stavu se nazývají hybridní Azure AD připojené zařízení.</span><span class="sxs-lookup"><span data-stu-id="68965-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="68965-207">Pokud váš podnik má místní služby Active Directory, která obsahuje některé místní prostředky (například sdílené soubory a tiskárny), můžete přidělit přístup Azure AD připojené zařízení tyto prostředky podle pokynů zde: [přístup místního zdroje z Azure AD připojené zařízení Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="68965-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="68965-208">Nasazení aplikace klienta služeb Office 365</span><span class="sxs-lookup"><span data-stu-id="68965-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="68965-209">Pokud zvolíte automaticky nainstalovat Office apps v průběhu sada nahoru, nainstaluje soubor apps po uživatelé přihlášeni k Azure AD ze svých zařízení systému Windows pomocí pověření jejich práce na zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="68965-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="68965-210">Chcete-li nainstalovat systém Office na mobilním iOS nebo Android zařízení, naleznete v tématu [nastavit mobilní zařízení pro uživatele Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="68965-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="68965-211">Office lze také nainstalovat samostatně.</span><span class="sxs-lookup"><span data-stu-id="68965-211">You can also install Office individually.</span></span> <span data-ttu-id="68965-212">Viz pokyny pro [instalaci sady Office na PC nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) .</span><span class="sxs-lookup"><span data-stu-id="68965-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="68965-213">Další nastavení zabezpečení</span><span class="sxs-lookup"><span data-stu-id="68965-213">Additional security settings</span></span>

<span data-ttu-id="68965-214">Kromě zabezpečení a kompatibility nastavení v Průvodci instalací můžete také nastavit další parametry:</span><span class="sxs-lookup"><span data-stu-id="68965-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="68965-215">**E-mailová ochrana proti malwaru**</span><span class="sxs-lookup"><span data-stu-id="68965-215">**Email malware protection**</span></span>
- <span data-ttu-id="68965-216">**Bezpečné přílohy Advanced Threat Protection (ATP)**</span><span class="sxs-lookup"><span data-stu-id="68965-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="68965-217">**ATP bezpečné propojení**</span><span class="sxs-lookup"><span data-stu-id="68965-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="68965-218">**VÝSTIŽNÝ anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="68965-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="68965-219">**Exchange Online - archiv**</span><span class="sxs-lookup"><span data-stu-id="68965-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="68965-220">**Zabránění ztrátě dat (DLP)**</span><span class="sxs-lookup"><span data-stu-id="68965-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="68965-221">**Ochrana údajů v Azure** (Plán 1)</span><span class="sxs-lookup"><span data-stu-id="68965-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="68965-222">**Dostupnost portálu Intune**</span><span class="sxs-lookup"><span data-stu-id="68965-222">**Intune portal availability**</span></span>

<span data-ttu-id="68965-223">Chcete-li získat spuštění naleznete v tématu [nastavení zásad pokročilé zabezpečení](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="68965-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="68965-224">Další informace naleznete v tématu [horní 10 způsobů, jak zabezpečit váš podnik 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) pro přehled osvědčených postupů zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="68965-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>