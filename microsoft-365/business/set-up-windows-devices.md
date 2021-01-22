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
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Přečtěte si, jak nastavit zařízení s Windows a uživateli s Windows 10 Pro for Microsoft 365 Business Premium, aby bylo umožněno centralizované řízení a ovládací prvky zabezpečení.
ms.openlocfilehash: b1877d83f113a2ba23d0db374967e0afcd7fe067
ms.sourcegitcommit: 855719ee21017cf87dfa98cbe62806763bcb78ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/22/2021
ms.locfileid: "49928718"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="37961-103">Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="37961-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="37961-104">Požadavky na nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="37961-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="37961-105">Než budete moci nastavit zařízení s Windows pro uživatele služby Microsoft 365 Business Premium, zkontrolujte, že na všech zařízeních běží Windows 10 Pro verze 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="37961-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="37961-106">Windows 10 Pro je předpokladem nasazení Windows 10 Business, což je sada cloudových služeb a funkcí pro správu zařízení, které doplňují Windows 10 Pro a umožňují centralizované řízení a ovládací prvky zabezpečení služby Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="37961-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="37961-107">Pokud máte zařízení s Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, máte v rámci předplatného Microsoft 365 Business Premium nárok na upgrade na Windows 10.</span><span class="sxs-lookup"><span data-stu-id="37961-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="37961-108">Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="37961-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="37961-109">Podívejte [se, jestli je zařízení připojené k Azure AD,](#verify-the-device-is-connected-to-azure-ad) abyste ověřili, že máte upgrade, nebo abyste měli jistotu, že upgrade funguje.</span><span class="sxs-lookup"><span data-stu-id="37961-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="37961-110">Podívejte se na krátké video o připojení Windows k Microsoftu 365.</span><span class="sxs-lookup"><span data-stu-id="37961-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="37961-111">Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="37961-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="37961-112">Připojení zařízení s Windows 10 ke službě Azure AD organizace</span><span class="sxs-lookup"><span data-stu-id="37961-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="37961-113">Pokud jsou všechna zařízení s Windows ve vaší organizaci upgradovaná na Windows 10 Pro Creators Update (nebo na nich už běží Windows 10 Pro Creators Update), můžete je připojit k Azure Active Directory vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="37961-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="37961-114">Jakmile jsou zařízení připojená, budou automaticky upgradována na Windows 10 Business, který je součástí vašeho předplatného Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="37961-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="37961-115">Zcela nové nebo nově upgradované zařízení s Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="37961-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="37961-116">U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.</span><span class="sxs-lookup"><span data-stu-id="37961-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="37961-117">Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**.</span><span class="sxs-lookup"><span data-stu-id="37961-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="37961-119">Tady zvolte **Nastavit pro organizaci a** potom zadejte svoje uživatelské jméno a heslo pro Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="37961-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="37961-120">Dokončete nastavení zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="37961-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="37961-p103">Po dokončení nastavení bude uživatel připojen k Azure AD organizace. Pokud chcete nastavení zkontrolovat, přečtěte si část [Kontrola připojení zařízení k Azure AD](#verify-the-device-is-connected-to-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="37961-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="37961-123">Nastavené zařízení se spuštěným systémem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="37961-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="37961-124">**Připojení uživatelů k Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="37961-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="37961-125">V uživatelském počítači se systémem Windows 10 Pro ve verzi 1703 (Creators Update) (viz [předpoklady](pre-requisites-for-data-protection.md)) klikněte na klávesu s logem Windows a potom na ikonu Nastavení.</span><span class="sxs-lookup"><span data-stu-id="37961-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="37961-127">V **Nastavení** přejděte na **Účty**.</span><span class="sxs-lookup"><span data-stu-id="37961-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="37961-129">Na stránce **Vaše informace** klikněte na **Přístup do práce nebo do školy** \> **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="37961-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="37961-131">V dialogovém okně **Nastavit pracovní nebo školní účet** v části **Alternativní akce** zvolte **Připojit toto zařízení k Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="37961-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="37961-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="37961-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="37961-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="37961-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="37961-136">Na stránce **Zkontrolujte, jestli se jedná o** vaši organizaci, ověřte, jestli jsou informace správné, a zvolte Připojit **se.**</span><span class="sxs-lookup"><span data-stu-id="37961-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="37961-137">A je **to všechno!**</span><span class="sxs-lookup"><span data-stu-id="37961-137">On the **You're all set!**</span></span> <span data-ttu-id="37961-138">, chosse **Done**.</span><span class="sxs-lookup"><span data-stu-id="37961-138">page, chosse **Done**.</span></span>
  
   ![Na obrazovce Zkontrolujte, že se jedná o vaši organizaci, zvolte Připojit se.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="37961-140">Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače.</span><span class="sxs-lookup"><span data-stu-id="37961-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="37961-141">Pokud jste k migraci profilu a souborů použili nástroj třetí strany, synchronizujte také profil s novým profilem.</span><span class="sxs-lookup"><span data-stu-id="37961-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="37961-142">Kontrola připojení zařízení k Azure AD</span><span class="sxs-lookup"><span data-stu-id="37961-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="37961-143">Stav synchronizace ověříte tak, že na pracovní nebo  školní stránce **Accessu** v Nastavení vyberete oblast Připojeno k_ – zobrazí se informace o tlačítkách a \<organization name\> **odpojit.** </span><span class="sxs-lookup"><span data-stu-id="37961-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="37961-144">Zvolte **Informace a** získejte informace o stavu synchronizace.</span><span class="sxs-lookup"><span data-stu-id="37961-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="37961-145">Na stránce **Stavu** synchronizace  zvolte Synchronizovat, abyste do počítače dostali nejnovější zásady správy mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="37961-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="37961-146">Pokud chcete začít používat účet Microsoft 365 Business Premium, přejděte na tlačítko **Start** ve Windows, klikněte pravým tlačítkem myši na obrázek aktuálního účtu a **pak přejděte na Přepnout účet.**</span><span class="sxs-lookup"><span data-stu-id="37961-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="37961-147">Přihlaste se e-mailem a heslem vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="37961-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="37961-149">Ověření upgradu počítače na Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="37961-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="37961-150">Zkontrolujte, jestli jsou zařízení s Windows 10 připojená k Azure AD upgradována na Windows 10 Business v rámci předplatného Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="37961-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="37961-151">Přejděte na **Nastavení** \> **Systém** \> **O systému**.</span><span class="sxs-lookup"><span data-stu-id="37961-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="37961-152">Zkontrolujte, jestli **Edice** je **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="37961-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="37961-154">Další kroky</span><span class="sxs-lookup"><span data-stu-id="37961-154">Next steps</span></span>

<span data-ttu-id="37961-155">Informace o nastavení mobilních zařízení najdete v tématu Nastavení mobilních zařízení pro uživatele [služby Microsoft 365 Business Premium.](set-up-mobile-devices.md)Informace o nastavení zásad ochrany zařízení nebo aplikací najdete v tématu Správa [Microsoftu 365 pro firmy.](manage.md)</span><span class="sxs-lookup"><span data-stu-id="37961-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="37961-156">Další informace o nastavení a používání Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="37961-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="37961-157">Školicí videa pro Microsoft 365 pro firmy</span><span class="sxs-lookup"><span data-stu-id="37961-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
