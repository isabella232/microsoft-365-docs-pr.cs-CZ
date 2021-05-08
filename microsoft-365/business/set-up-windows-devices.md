---
title: Nastavení Windows pro Microsoft 365 Business Premium uživatele
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
description: Zjistěte, jak nastavit Windows zařízení s Windows 10 Pro pro Microsoft 365 Business Premium, které umožňují centralizovanou správu a ovládací prvky zabezpečení.
ms.openlocfilehash: 3e268d81ff6fb7113b7e0b0fe5d0545ff5c72b1e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244770"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="1b3b7-103">Nastavení Windows pro Microsoft 365 Business Premium uživatele</span><span class="sxs-lookup"><span data-stu-id="1b3b7-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="1b3b7-104">Předpoklady pro nastavení Windows pro Microsoft 365 Business Premium uživatele</span><span class="sxs-lookup"><span data-stu-id="1b3b7-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="1b3b7-105">Než budete moci nastavit Windows pro Microsoft 365 Business Premium, zkontrolujte, jestli jsou všechna Windows zařízení Windows 10 Pro, verze 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="1b3b7-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="1b3b7-106">Windows 10 Pro je předpokladem pro nasazení Windows 10 Business, což je sada cloudových služeb a možností správy zařízení, které doplňují Windows 10 Pro a umožňují centralizovanou správu a řízení zabezpečení Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="1b3b7-107">Pokud máte zařízení Windows Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné Microsoft 365 Business Premium vás opravňuje k Windows 10 upgradu.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="1b3b7-108">Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="1b3b7-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="1b3b7-109">Informace [o tom, jestli](#verify-the-device-is-connected-to-azure-ad) máte upgrade, najdete v článku Ověření připojení zařízení k Azure AD nebo ověření, jestli upgrade fungoval.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="1b3b7-110">Podívejte se na krátké video o připojení Windows k Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="1b3b7-111">Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="1b3b7-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="1b3b7-112">Připojení zařízení s Windows 10 ke službě Azure AD organizace</span><span class="sxs-lookup"><span data-stu-id="1b3b7-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="1b3b7-113">Když jsou Windows zařízení ve vaší organizaci upgradovaná na aktualizaci Windows 10 Pro Creators Update nebo už máte spuštěnou aktualizaci Windows 10 Pro Creators Update, můžete tato zařízení připojit k Azure Active Directory vaší Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="1b3b7-114">Po přihlášení se zařízení automaticky upgradují na Windows 10 Business, které je součástí vašeho Microsoft 365 Business Premium předplatného.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="1b3b7-115">Zcela nové nebo nově upgradované zařízení s Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="1b3b7-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="1b3b7-116">U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="1b3b7-117">Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="1b3b7-119">Tady zvolte **Nastavit pro organizaci a** zadejte svoje uživatelské jméno a heslo pro Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="1b3b7-120">Dokončete nastavení zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="1b3b7-p103">Po dokončení nastavení bude uživatel připojen k Azure AD organizace. Pokud chcete nastavení zkontrolovat, přečtěte si část [Kontrola připojení zařízení k Azure AD](#verify-the-device-is-connected-to-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="1b3b7-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="1b3b7-123">Nastavené zařízení se spuštěným systémem Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="1b3b7-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="1b3b7-124">**Připojení uživatelů k Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="1b3b7-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="1b3b7-125">V uživatelském počítači se systémem Windows 10 Pro ve verzi 1703 (Creators Update) (viz [předpoklady](pre-requisites-for-data-protection.md)) klikněte na klávesu s logem Windows a potom na ikonu Nastavení.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="1b3b7-127">V **Nastavení** přejděte na **Účty**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="1b3b7-129">Na stránce **Vaše informace** klikněte na **Přístup do práce nebo do školy** \> **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="1b3b7-131">V dialogovém okně **Nastavit pracovní nebo školní účet** v části **Alternativní akce** zvolte **Připojit toto zařízení k Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="1b3b7-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="1b3b7-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="1b3b7-136">Na stránce **Zkontrolujte, jestli je to vaše** organizace, ověřte, jestli jsou informace správné, a zvolte Připojit **se.**</span><span class="sxs-lookup"><span data-stu-id="1b3b7-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="1b3b7-137">Na **sadě Jste všichni!**</span><span class="sxs-lookup"><span data-stu-id="1b3b7-137">On the **You're all set!**</span></span> <span data-ttu-id="1b3b7-138">stránka, chosse Done ( **Hotovo).**</span><span class="sxs-lookup"><span data-stu-id="1b3b7-138">page, chosse **Done**.</span></span>
  
   ![Na obrazovce Ujistěte se, že je to vaše organizace, zvolte Připojit se.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="1b3b7-140">Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="1b3b7-141">Pokud jste k migraci profilu a souborů použili nástroj jiného výrobce, synchronizujte je taky s novým profilem.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="1b3b7-142">Kontrola připojení zařízení k Azure AD</span><span class="sxs-lookup"><span data-stu-id="1b3b7-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="1b3b7-143">Pokud chcete ověřit stav synchronizace, vyberte na pracovní nebo školní  stránce **Accessu** **v Nastavení** oblast Připojeno k _ _ a zobrazí se tlačítka Informace a \<organization name\> **Odpojit.** </span><span class="sxs-lookup"><span data-stu-id="1b3b7-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="1b3b7-144">Pokud **chcete získat** stav synchronizace, zvolte Informace.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="1b3b7-145">Na stránce **Stav** synchronizace  zvolte Synchronizovat a získejte nejnovější zásady správy mobilních zařízení do počítače.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="1b3b7-146">Pokud chcete začít Microsoft 365 Business Premium účtu, přejděte na tlačítko Windows **Start,** klikněte pravým tlačítkem myši na obrázek aktuálního účtu a potom **na Přepnout účet**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="1b3b7-147">Přihlaste se e-mailem a heslem vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="1b3b7-149">Ověření upgradu počítače na Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="1b3b7-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="1b3b7-150">Ověřte, jestli jsou vaše zařízení připojená Windows 10 Azure AD upgradovaná na Windows 10 Business jako součást vašeho předplatného Microsoft 365 Business Premium služby.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="1b3b7-151">Přejděte na **Nastavení** \> **Systém** \> **O systému**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="1b3b7-152">Zkontrolujte, jestli **Edice** je **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="1b3b7-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="1b3b7-154">Další kroky</span><span class="sxs-lookup"><span data-stu-id="1b3b7-154">Next steps</span></span>

<span data-ttu-id="1b3b7-155">Informace o nastavení mobilních zařízení najdete v tématu Nastavení mobilních zařízení pro [Microsoft 365 Business Premium](set-up-mobile-devices.md)uživatelů , Nastavení ochrany zařízení nebo zásad ochrany aplikací v tématu Správa [Microsoft 365 pro firmy](manage.md).</span><span class="sxs-lookup"><span data-stu-id="1b3b7-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="1b3b7-156">Další informace o nastavení a používání Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="1b3b7-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="1b3b7-157">Microsoft 365 pro firemní školicí videa</span><span class="sxs-lookup"><span data-stu-id="1b3b7-157">Microsoft 365 for business training videos</span></span>](../business-video/index.yml)
