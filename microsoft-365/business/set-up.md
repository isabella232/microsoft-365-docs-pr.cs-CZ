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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Naučte se nastavit aplikaci Microsoft 365 Business.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575542"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="64b2d-103">Nastavení aplikace Microsoft 365 Business v Průvodci nastavením</span><span class="sxs-lookup"><span data-stu-id="64b2d-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="64b2d-104">Přidání domény, uživatelů a nastavení zásad</span><span class="sxs-lookup"><span data-stu-id="64b2d-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="64b2d-105">[![Popisek vám dá vědět, že se centrum pro správu mění a další podrobnosti naleznete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="64b2d-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="64b2d-106">Zakoupí-li společnost Microsoft 365 Business, máte možnost používat vlastní doménu nebo ji zakoupit během [zápisu](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="64b2d-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="64b2d-107">Pokud jste při přihlášení zakoupili novou doménu, je vaše doména nastavena a můžete se přesouvat a [přidávat uživatele a přiřazovat jim licence](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="64b2d-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="64b2d-108">Přidání domény k přizpůsobení přihlášení</span><span class="sxs-lookup"><span data-stu-id="64b2d-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="64b2d-109">Přihlaste se ke [středisku Microsoft 365 Admin Center](https://admin.microsoft.com) pomocí globálních pověření pro správu.</span><span class="sxs-lookup"><span data-stu-id="64b2d-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="64b2d-110">Zvolte možnost **Přidat doménu** nebo **Přidat uživatele** Chcete-li spustit průvodce.</span><span class="sxs-lookup"><span data-stu-id="64b2d-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="64b2d-111">Pokud jste během zápisu zakoupili doménu, nezobrazí se zde krok **Přidat doménu** .</span><span class="sxs-lookup"><span data-stu-id="64b2d-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="64b2d-112">Přejděte na místo pro [Přidání uživatelů](#add-users-and-assign-licenses) .</span><span class="sxs-lookup"><span data-stu-id="64b2d-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Vyberte možnost přejít k nastavení.](media/gotosetupinadmincenter.png)
    
3. <span data-ttu-id="64b2d-114">V průvodci zadejte název domény, který chcete použít (například contoso.com).</span><span class="sxs-lookup"><span data-stu-id="64b2d-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Obrazovka stránky přizpůsobit přihlašovací stránku.](media/personalizesignin.png)

    
4. <span data-ttu-id="64b2d-116">Postupujte podle pokynů průvodce a [vytvořte záznamy DNS u kteréhokoli poskytovatele hostitelských služeb DNS pro sadu Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , který ověřuje vlastní doménu.</span><span class="sxs-lookup"><span data-stu-id="64b2d-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="64b2d-117">Pokud znáte hostitele domény, podívejte se také na [pokyny týkající se hostitele](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="64b2d-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="64b2d-118">Pokud je poskytovatelem hostitelských služeb GoDaddy nebo jiný hostitel s připojením k [doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), je tento proces snadný a budete automaticky požádáni o přihlášení a společnost Microsoft vám bude ověřovat ve vašem zastoupení:</span><span class="sxs-lookup"><span data-stu-id="64b2d-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![U možnosti potvrdit přístup na stránce GoDaddy vyberte možnost ověřit.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="64b2d-120">Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="64b2d-120">Add users and assign licenses</span></span>

<span data-ttu-id="64b2d-121">Můžete přidat uživatele v průvodci, ale můžete je také [přidat později](add-users-m365b.md) v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="64b2d-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="64b2d-122">Navíc, pokud máte místní řadič domény, můžete přidat uživatele pomocí [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="64b2d-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="64b2d-123">Přidání uživatelů v Průvodci</span><span class="sxs-lookup"><span data-stu-id="64b2d-123">Add users in the wizard</span></span>

<span data-ttu-id="64b2d-124">Všichni uživatelé, které přidáte v průvodci, dostanou automaticky přiřazenu licenci Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="64b2d-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Obrazovka stránky přidat nové uživatele v Průvodci](media/addnewuserspage.png)

1. <span data-ttu-id="64b2d-126">Pokud vaše předplatné aplikace Microsoft 365 Business obsahuje existující uživatele (například pokud jste použili program Azure AD Connect), můžete jim nyní přiřadit licence.</span><span class="sxs-lookup"><span data-stu-id="64b2d-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="64b2d-127">Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="64b2d-127">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="64b2d-128">Po přidání uživatelů budete mít také možnost sdílet pověření s novými uživateli, které jste přidali.</span><span class="sxs-lookup"><span data-stu-id="64b2d-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="64b2d-129">Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="64b2d-129">You can choose to print them out, email them, or download them.</span></span>

3. <span data-ttu-id="64b2d-130">Do pole vytvořit týmy pro vaši organizaci můžete přidat týmy a přidat do nich uživatele.</span><span class="sxs-lookup"><span data-stu-id="64b2d-130">On the Create Teams for your organization, you can choose to add Teams and add users to them.</span></span> <span data-ttu-id="64b2d-131">Můžete to provést také později.</span><span class="sxs-lookup"><span data-stu-id="64b2d-131">You can also do this later.</span></span> <span data-ttu-id="64b2d-132">Další informace naleznete v tématu [vytvoření týmu pro celou společnost](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span><span class="sxs-lookup"><span data-stu-id="64b2d-132">For more information, see [create a company-wide Team](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span></span>

4. <span data-ttu-id="64b2d-133">Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="64b2d-133">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="64b2d-134">Pokud se přesouváte od jiného poskytovatele e-mailu a chcete data později zkopírovat, můžete [přenést e-maily a kontakty do sady Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="64b2d-134">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="64b2d-135">Připojení domény</span><span class="sxs-lookup"><span data-stu-id="64b2d-135">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="64b2d-136">Pokud zvolíte použití domény. onmicrosoft nebo použijete Azure AD Connect pro nastavení uživatelů, tento krok se nezobrazí.</span><span class="sxs-lookup"><span data-stu-id="64b2d-136">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="64b2d-137">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="64b2d-137">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="64b2d-138">Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora.</span><span class="sxs-lookup"><span data-stu-id="64b2d-138">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="64b2d-139">Pokud tomu tak není, [změňte nameservery tak, aby sadu Office 365 nastavil s jakýmkoli registrátorem domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="64b2d-139">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="64b2d-140">Pokud máte existující záznamy DNS, například existující web, ale hostitel DNS je povolen pro [připojení k doméně](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), zvolte možnost **Přidat záznamy**.</span><span class="sxs-lookup"><span data-stu-id="64b2d-140">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="64b2d-141">Na stránce **Vyberte stránku služeb online** , přijměte všechny výchozí hodnoty a klepněte na tlačítko **Další**a na stránce hostitele DNS vyberte možnost **autorizovat** .</span><span class="sxs-lookup"><span data-stu-id="64b2d-141">On the **Choose your online services** page, accept all the defaults, and choose **Next**,and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="64b2d-142">Pokud máte existující záznamy DNS s jinými hostiteli DNS (nejsou povoleny pro připojení k doméně), budete chtít spravovat své vlastní záznamy DNS, abyste zajistili, že stávající služby zůstanou propojeny.</span><span class="sxs-lookup"><span data-stu-id="64b2d-142">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="64b2d-143">Další informace naleznete v tématu [základy domény](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="64b2d-143">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Připojte stránku domény ke správě vlastních záznamů DNS.](media/connectyourdomainpage.png)

2. <span data-ttu-id="64b2d-145">Postupujte podle pokynů průvodce a e-maily a další služby budou nastaveny pro vás.</span><span class="sxs-lookup"><span data-stu-id="64b2d-145">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-data-and-devices"></a><span data-ttu-id="64b2d-146">Ochrana dat a zařízení</span><span class="sxs-lookup"><span data-stu-id="64b2d-146">Protect data and devices</span></span> 

<span data-ttu-id="64b2d-147">Zásady nastavené v průvodci jsou automaticky použity pro [skupinu zabezpečení](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) nazvanou *Všichni uživatelé*.</span><span class="sxs-lookup"><span data-stu-id="64b2d-147">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="64b2d-148">Můžete také vytvořit další skupiny pro přiřazení zásad v centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="64b2d-148">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="64b2d-149">Na panelu **Chraňte své pracovní soubory na mobilních zařízeních** možnost **chránit pracovní soubory při ztrátě nebo odcizení zařízení** je ve výchozím nastavení vybráno.</span><span class="sxs-lookup"><span data-stu-id="64b2d-149">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="64b2d-150">Máte možnost zapnout **správu způsobu, jakým uživatelé přistupují k souborům sady Office na mobilních zařízeních**, a tento postup je doporučen.</span><span class="sxs-lookup"><span data-stu-id="64b2d-150">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Obrazovka o ochraně pracovních souborů na stránce mobilních zařízení](media/protectworkfilesondevices.png)

     - <span data-ttu-id="64b2d-152">Rozbalit **ochranu pracovních souborů při ztrátě nebo odcizení zařízení** pro zobrazení [výchozích hodnot](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="64b2d-152">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Obrazovka výchozích hodnot pro ochranu souborů ztracených zařízení.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="64b2d-154">Vyberte možnost **spravovat způsob, jakým uživatelé přistupují k souborům systému Office v mobilních zařízeních** , a rozbalte ji, aby zobrazili [výchozí hodnoty](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="64b2d-154">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="64b2d-155">Doporučujeme, abyste při instalaci přijali výchozí hodnoty a vytvořili tak zásady použití pro systémy Android, iOS a Windows 10, které se vztahují na všechny uživatele.</span><span class="sxs-lookup"><span data-stu-id="64b2d-155">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="64b2d-156">Další zásady můžete vytvořit po dokončení instalace.</span><span class="sxs-lookup"><span data-stu-id="64b2d-156">You can create more policies after setup completes.</span></span>

        ![Obrazovka nastavení ochrany pro soubory sady Office v mobilním počítači.](media/useraccessonmobile.png)

2. <span data-ttu-id="64b2d-158">Poslední krok týkající se ochrany dat a zařízení umožňuje nastavit zásady pro zabezpečení zařízení systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="64b2d-158">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="64b2d-159">Tato nastavení jsou automaticky použita při připojení uživatele systému Windows 10 k vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="64b2d-159">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="64b2d-160">Můžete rozbalit **Zabezpečená zařízení Windows 10** a zobrazit a upravit [výchozí hodnoty](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="64b2d-160">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="64b2d-161">Můžete také zvolit [automatickou instalaci sady Office](install-office-on-windows-10-during-setup.md) do zařízení systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="64b2d-161">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Obrazovka nastavení stránky konfigurace zařízení systému Windows 10.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="64b2d-163">Nasadit sadu Office 365 Client Apps</span><span class="sxs-lookup"><span data-stu-id="64b2d-163">Deploy Office 365 client apps</span></span>

<span data-ttu-id="64b2d-164">Pokud se rozhodnete automaticky instalovat aplikace sady Office během nastavování, budou aplikace nainstalovány do zařízení systému Windows 10, jakmile se uživatelé budou přihlásit k Azure AD z jejich zařízení se systémem Windows s jejich pracovním pověřením.</span><span class="sxs-lookup"><span data-stu-id="64b2d-164">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="64b2d-165">Informace o instalaci sady Office na mobilních zařízeních iOS nebo Android naleznete v tématu [nastavení mobilních zařízení pro Microsoft 365 Business Users](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="64b2d-165">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="64b2d-166">Sadu Office můžete nainstalovat také jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="64b2d-166">You can also install Office individually.</span></span> <span data-ttu-id="64b2d-167">Pokyny naleznete [v části instalace sady Office v počítači nebo Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="64b2d-167">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
