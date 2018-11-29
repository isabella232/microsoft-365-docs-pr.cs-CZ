---
title: Nastavení Microsoft 365 Business pomocí průvodce nastavením
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
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zjistěte, jak nastavit Microsoft 365 Business podle čtyř kroků.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982191"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="e4202-103">Nastavení Microsoft 365 Business pomocí průvodce nastavením</span><span class="sxs-lookup"><span data-stu-id="e4202-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="e4202-104">Proveďte kroky 1-4 níže.</span><span class="sxs-lookup"><span data-stu-id="e4202-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="e4202-105">Nastavení Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4202-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="e4202-106">Podívejte se na video návod, jak nastavit Microsoft 365 Business, pokud nemáte místní služby Active Directory:</span><span class="sxs-lookup"><span data-stu-id="e4202-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="e4202-p101">Informace o nastavení, které zahrnují místní adresář Active Directory zahrnuje následující kroky instalace. Pokud chcete získat přístup k zařízení připojeno k doméně, přečtěte si následující články pro dva jiný způsob povolení a proveďte kroky před spuštěním Průvodce instalací:</span><span class="sxs-lookup"><span data-stu-id="e4202-p101">The set-up steps include information for setups that include local Active Directory. If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="e4202-109">Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4202-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="e4202-110">-Toto je doporučený způsob.</span><span class="sxs-lookup"><span data-stu-id="e4202-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="e4202-111">Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4202-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="e4202-112">Krok 1: Přizpůsobit přihlásit se</span><span class="sxs-lookup"><span data-stu-id="e4202-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="e4202-p102">Přihlaste se k [Microsoft 365 Business](https://portal.microsoft.com) pod uživatelským jménem a heslem globálního správce. Vyberte dlaždici **Správce** a přejděte do Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="e4202-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="e4202-115">V Centru pro správu zvolte **Spustit nastavení** (v závislosti na stavu se může zobrazit **Pokračovat v nastavení**) a spusťte průvodce.</span><span class="sxs-lookup"><span data-stu-id="e4202-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="e4202-116">Zadejte název domény, který chcete použít (jako contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e4202-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="e4202-p103">Pokračovat a zadat domény i v případě, že ověřil při používání Azure AD připojit, například. Následující dva kroky na vás nemusí vztahovat, pokud se používá Azure AD připojit k ověření vaší domény.</span><span class="sxs-lookup"><span data-stu-id="e4202-p103">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example. The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="e4202-119">Postupujte podle kroků v průvodci [vytvořit DNS záznamy na jakékoliv DNS poskytovatele hostitelských služeb pro Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) ověří, že jste vlastníkem domény.</span><span class="sxs-lookup"><span data-stu-id="e4202-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="e4202-p104">Můžete zobrazit příklad video [Video: nastavení služeb Office 365 v nový Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Všimněte si, že toto video neobsahuje kroky ochrany dat Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e4202-p104">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="e4202-123">Krok 2: Přidání uživatelů a přiřazení licencí</span><span class="sxs-lookup"><span data-stu-id="e4202-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="e4202-124">Uživatele můžete přidat nyní nebo je můžete [přidat později](add-users-m365b.md) v Centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="e4202-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="e4202-125">Každému přidanému uživateli se automaticky přiřadí licence Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e4202-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="e4202-p105">Pokud vaše předplatné Microsoft 365 Business již uživatele má (například pokud jste použili službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní. Neváhejte a přidejte licence i jim.</span><span class="sxs-lookup"><span data-stu-id="e4202-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="e4202-p106">Budete mít také možnost přihlašovací údaje s nově přidanými uživateli sdílet. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.</span><span class="sxs-lookup"><span data-stu-id="e4202-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="e4202-130">Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**.</span><span class="sxs-lookup"><span data-stu-id="e4202-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="e4202-131">Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="e4202-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="e4202-133">Krok 3: Připojení domény</span><span class="sxs-lookup"><span data-stu-id="e4202-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="e4202-134">Pokud používáte domény .onmicrosoft nebo použít Azure AD připojit, nezobrazí se tento krok.</span><span class="sxs-lookup"><span data-stu-id="e4202-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="e4202-135">Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.</span><span class="sxs-lookup"><span data-stu-id="e4202-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="e4202-p107">Průvodce instalací obvykle zjistí váš Registrátor a poskytuje odkaz na podrobné pokyny pro aktualizaci na webu registrátora záznamy NS. Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="e4202-p107">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website. If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="e4202-138">E-mail a další služby budou nastaveny za vás.</span><span class="sxs-lookup"><span data-stu-id="e4202-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="e4202-139">Krok 4: Správa zařízení a pracovní soubory</span><span class="sxs-lookup"><span data-stu-id="e4202-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="e4202-p108">**Ochrana pracovních souborů v mobilních zařízeních** stránce nastavte **chránit pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** a **Správa přístupu uživatelů na soubory sady Office na mobilních zařízeních** nastavení **on**. Dostanete každé dílčí nastavení klepnutím na šipky vedle každého nastavení.</span><span class="sxs-lookup"><span data-stu-id="e4202-p108">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**. You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="e4202-142">Všechny pracovní soubory licencovaných uživatelů jsou nyní chráněna na iOS a Android zařízení, jakmile jsou [instalace aplikací sady Office](set-up-mobile-devices.md) (a ověření pomocí pověření Microsoft 365 Business).</span><span class="sxs-lookup"><span data-stu-id="e4202-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="e4202-144">Na stránce **Konfigurace zařízení Windows 10 nastavit** nastavte nastavení **Zabezpečení zařízení Windows 10** **On**.</span><span class="sxs-lookup"><span data-stu-id="e4202-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="e4202-145">Dostanete každé dílčí nastavení klepnutím na dvojitou šipku vedle ní.</span><span class="sxs-lookup"><span data-stu-id="e4202-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="e4202-p109">Nastavte nastavení **Instalace sady Office v systému Windows 10 zařízení** **Ano** Pokud všem uživatelům Windows 10 počítačů a nainstaluje žádné existující Office nebo instalace sady Office klepněte na tlačítko spustit. Pokud tomu tak není, nastavte tuto možnost na hodnotu **Ne**. Po skončení přípravy počítačů uživatelů můžete [automaticky nainstalovat Office](auto-install-or-uninstall-office.md) později z středisku pro správce. Pokyny naleznete v tématu [Příprava instalace klienta sady Office](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="e4202-p109">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs. If this is not the case, set this option to **No**. You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers. For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="e4202-150">Pracovní soubory licencovaných uživatelů na zařízeních s Windows 10 bude co nejdříve, jakmile budou promítat [připojit své zařízení Windows 10](set-up-windows-devices.md) obchodní Microsoft 365 Azure AD doméně nebo při současně spojující Microsoft 365 [Windows 10 do nového počítače nainstalovat](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) Obchodní domény Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4202-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="e4202-151">Klikněte na **Další** a nastavení je hotové.</span><span class="sxs-lookup"><span data-stu-id="e4202-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="e4202-152">Podělte se s námi prosím o svůj názor, abyste nám pomohli vylepšit toto prostředí.</span><span class="sxs-lookup"><span data-stu-id="e4202-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="e4202-154">Další nastavení zabezpečení</span><span class="sxs-lookup"><span data-stu-id="e4202-154">Additional security settings</span></span>

<span data-ttu-id="e4202-155">Kromě zabezpečení a kompatibility nastavení v Průvodci instalací můžete také nastavit další parametry:</span><span class="sxs-lookup"><span data-stu-id="e4202-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="e4202-p110">Nastavení ochrany proti nebezpečným přílohám. **Advanced Threat Protection** (ATP) označuje škodlivý obsah a pak blokuje dodání nebezpečné přílohy, pomáhá chránit před podvodnými postupy typu phishing a ransomware infekcemi. Aktivaci ochrany přílohy naleznete v tématu [nastavení zásad bezpečné přílohy ATP Office 365](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="e4202-p110">Set up protection against unsafe attachments. **Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections. To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="e4202-p111">Chrání vaše prostředí klepnutím na nebezpečné odkazy. ATP kontroluje odkazy v e-mailu v okamžiku kliknutí na ně. Pokud odkaz není bezpečné, uživatel je varován, aby na webu nebo informován, že webu byl zablokován. To pomáhá chránit před podvodnými postupy typu phishing. [Nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) nebo [nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="e4202-p111">Protect your environment when users click malicious links. ATP examines links in email at the time a user clicks them. If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked. This helps protect against phishing schemes. [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="e4202-p112">Můžete zachovat veškerý obsah poštovní schránky včetně vložením celé poštovní schránky uživatele na **soudní spory podržte**odstraněných položek. Pokyny naleznete v tématu</span><span class="sxs-lookup"><span data-stu-id="e4202-p112">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**. For instructions, see</span></span> 
- <span data-ttu-id="e4202-166">[Nastavení uchovávání e-mailů s Exchange Online archivaci](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="e4202-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="e4202-p113">Například nastavte vlastní **zásady uchovávání informací**má být zachována po určitou dobu nebo trvale odstranit obsah na konci období uchování informací Můžete povolit zásady uchovávání přizpůsobené s cennými papíry a centra kompatibility, přejděte do **správy věcí veřejných dat** \> **uchovávání informací**a pak postupujte podle kroků v průvodci. Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="e4202-p113">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period. You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard. To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="e4202-170">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e4202-170">Next steps</span></span>

<span data-ttu-id="e4202-171">Pokud uživatelé mají licenci, nastaví si v dalším kroku zařízení.</span><span class="sxs-lookup"><span data-stu-id="e4202-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="e4202-172">Další informace najdete v článcích [Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business](set-up-windows-devices.md) a [Nastavení mobilních zařízení pro uživatele služby Microsoft 365 Business](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="e4202-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="e4202-173">Pokud hledáte odkazy na témata týkající se nastavení zásad ochrany zařízení a aplikací nebo chcete zjistit, jak odebrat data ze zařízení uživatelů, přečtěte si článek [Správa Microsoft 365 Business](manage.md).</span><span class="sxs-lookup"><span data-stu-id="e4202-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  


