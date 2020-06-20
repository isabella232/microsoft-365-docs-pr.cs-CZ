---
title: Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Přečtěte si, jak nastavit zařízení s Windows s Windows 10 Pro pro uživatele Microsoft 365 Business Premium, což umožňuje centralizovanou správu a ovládací prvky zabezpečení.
ms.openlocfilehash: 85ac3c964792a132d5699703e543289020e38f57
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785846"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="e104c-103">Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="e104c-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="e104c-104">Požadavky pro nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="e104c-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="e104c-105">Než budete moci nastavit zařízení s Windows pro uživatele Microsoft 365 Business Premium, ujistěte se, že všechna zařízení s Windows používají Windows 10 Pro, verze 1703 (Aktualizace pro autory).</span><span class="sxs-lookup"><span data-stu-id="e104c-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="e104c-106">Windows 10 Pro je nezbytným předpokladem pro nasazení Windows 10 Business, což je sada cloudových služeb a možností správy zařízení, které doplňují Windows 10 Pro a umožňují centralizovanou správu a ovládací prvky zabezpečení Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e104c-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="e104c-107">Pokud máte zařízení s Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné Microsoft 365 Business Premium vás opravňuje k upgradu na Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e104c-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="e104c-108">Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="e104c-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="e104c-109">Viz [Ověření, zda je zařízení připojené k Azure AD,](#verify-the-device-is-connected-to-azure-ad) abyste ověřili, že máte upgrade, nebo abyste se ujistili, že upgrade fungoval.</span><span class="sxs-lookup"><span data-stu-id="e104c-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="e104c-110">Podívejte se na krátké video o připojení Windows k Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="e104c-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="e104c-111">Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="e104c-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="e104c-112">Připojení zařízení s Windows 10 ke službě Azure AD organizace</span><span class="sxs-lookup"><span data-stu-id="e104c-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="e104c-113">Pokud byla všechna zařízení s Windows ve vaší organizaci buď upgradována na aktualizaci Windows 10 Pro Creators Update, nebo už používáte aktualizaci Windows 10 Pro Creators Update, můžete tato zařízení připojit k Azure Active Directory vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="e104c-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="e104c-114">Jakmile se k nim připojíte, automaticky se upgradují na Windows 10 Business, který je součástí vašeho předplatného Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e104c-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="e104c-115">Zcela nové nebo nově upgradované zařízení s Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="e104c-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="e104c-116">U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.</span><span class="sxs-lookup"><span data-stu-id="e104c-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="e104c-117">Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**.</span><span class="sxs-lookup"><span data-stu-id="e104c-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="e104c-119">Tady zvolte **Nastavit pro organizaci** a pak zadejte své uživatelské jméno a heslo pro Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e104c-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="e104c-120">Dokončete nastavení zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e104c-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="e104c-121">Once you're done, the user will be connected to your organization's Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e104c-121">Once you're done, the user will be connected to your organization's Azure AD.</span></span> <span data-ttu-id="e104c-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span><span class="sxs-lookup"><span data-stu-id="e104c-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="e104c-123">Nastavené zařízení se spuštěným systémem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="e104c-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="e104c-124">**Připojení uživatelů k Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="e104c-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="e104c-125">V uživatelském počítači se systémem Windows 10 Pro ve verzi 1703 (Creators Update) (viz [předpoklady](pre-requisites-for-data-protection.md)) klikněte na klávesu s logem Windows a potom na ikonu Nastavení.</span><span class="sxs-lookup"><span data-stu-id="e104c-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="e104c-127">V **Nastavení** přejděte na **Účty**.</span><span class="sxs-lookup"><span data-stu-id="e104c-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="e104c-129">Na stránce **Vaše informace** klikněte na **Přístup do práce nebo do školy** \> **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="e104c-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="e104c-131">V dialogovém okně **Nastavit pracovní nebo školní účet** v části **Alternativní akce** zvolte **Připojit toto zařízení k Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="e104c-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="e104c-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="e104c-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="e104c-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="e104c-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="e104c-136">Na stránce **Ujistěte se, že se jedná** o vaši organizaci, ověřte, zda jsou informace správné, a klepněte na tlačítko **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="e104c-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="e104c-137">On the **You're all set!**</span><span class="sxs-lookup"><span data-stu-id="e104c-137">On the **You're all set!**</span></span> <span data-ttu-id="e104c-138">page, click **Done**.</span><span class="sxs-lookup"><span data-stu-id="e104c-138">page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="e104c-140">Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače.</span><span class="sxs-lookup"><span data-stu-id="e104c-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="e104c-141">Pokud jste k migraci profilu a souborů použili nástroj jiného výrobce, synchronizujte je také s novým profilem.</span><span class="sxs-lookup"><span data-stu-id="e104c-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="e104c-142">Kontrola připojení zařízení k Azure AD</span><span class="sxs-lookup"><span data-stu-id="e104c-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="e104c-143">Chcete-li ověřit stav synchronizace, klikněte na stránce **Práce nebo Škola aplikace Access** v **nastavení**klepnutím na oblast **Connected to** _ _ \<organization name\> tlačítka **Informace** a **Odpojení**.</span><span class="sxs-lookup"><span data-stu-id="e104c-143">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="e104c-144">Kliknutím na možnost **Informace** zjistíte stav synchronizace.</span><span class="sxs-lookup"><span data-stu-id="e104c-144">Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="e104c-145">Pokud chcete pro tento počítač získat nejnovější zásady správy mobilních zařízení, klikněte na stránce Stav synchronizace na Synchronizovat.</span><span class="sxs-lookup"><span data-stu-id="e104c-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="e104c-146">Pokud chcete začít používat účet Microsoft 365 Business Premium, přejděte na tlačítko **Start** ve Windows, klikněte pravým tlačítkem myši na obrázek aktuálního účtu a potom **přepněte účet**.</span><span class="sxs-lookup"><span data-stu-id="e104c-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="e104c-147">Přihlaste se e-mailem a heslem vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="e104c-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="e104c-149">Kontrola upgradu zařízení na Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="e104c-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="e104c-150">Ověřte, že vaše zařízení Azure AD připojená k Windows 10 byla upgradována na Windows 10 Business jako součást předplatného Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e104c-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="e104c-151">Přejděte na **Nastavení** \> **Systém** \> **O systému**.</span><span class="sxs-lookup"><span data-stu-id="e104c-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="e104c-152">Zkontrolujte, jestli **Edice** je **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="e104c-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="e104c-154">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e104c-154">Next steps</span></span>

<span data-ttu-id="e104c-155">Informace o nastavení mobilních zařízení najdete v tématu [Nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md), Nastavení zásad ochrany zařízení nebo ochrany aplikací v [tématu Správa Microsoftu 365 pro firmy](manage.md).</span><span class="sxs-lookup"><span data-stu-id="e104c-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="e104c-156">Další informace o nastavení a používání Microsoftu 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="e104c-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="e104c-157">Školicí videa microsoftu 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="e104c-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
