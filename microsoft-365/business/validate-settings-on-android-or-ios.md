---
title: Ověření nastavení ochrany aplikací na zařízeních s Androidem nebo iOS
f1.keywords:
- NOCSH
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
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Zjistěte, jak ověřit nastavení ochrany Microsoft 365 Business Premium aplikací na zařízeních s Androidem nebo iOS.
ms.openlocfilehash: 43e74b548711550090021c39096b1647cee9e039
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339324"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="e4d4f-103">Ověření nastavení ochrany aplikací na zařízeních s Androidem nebo iOS</span><span class="sxs-lookup"><span data-stu-id="e4d4f-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="e4d4f-104">Podle pokynů v následujících částech ověřte nastavení ochrany aplikací na zařízeních s Androidem nebo iOS.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="e4d4f-105">Android</span><span class="sxs-lookup"><span data-stu-id="e4d4f-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="e4d4f-106">Zkontrolujte, že nastavení ochrany aplikací funguje na uživatelských zařízeních.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="e4d4f-107">Jakmile [nastavíte konfigurace aplikací pro zařízení s Androidem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="e4d4f-108">Nejdřív se ujistěte, že se zásady vztahují na aplikaci, ve které ji chcete ověřit.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="e4d4f-109">V Centru Microsoft 365 Business Premium [pro správu](https://admin.microsoft.com)přejděte na **Zásady pro** \> **úpravy zásad**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-109">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="e4d4f-110">Zvolte **Zásady aplikace pro Android** pro nastavení, která jste vytvořili při nastavení, nebo jinou zásadu, kterou jste vytvořili, a ověřte, jestli je vynucovaná pro Outlook nastavení.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="e4d4f-112">Ověření nastavení Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="e4d4f-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="e4d4f-113">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Ujistěte se, že je možnost Vyžadovat PIN kód nebo otisk prstu pro přístup Office aplikace nastavená na Hodnotu Zapnout.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="e4d4f-115">Na zařízení s Androidem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="e4d4f-116">Zobrazí se taky výzva k zadání PIN kódu nebo k použití otisku prstu.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="e4d4f-118">Ověření možnosti Resetovat PIN po několika neúspěšných pokusech</span><span class="sxs-lookup"><span data-stu-id="e4d4f-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="e4d4f-119">V podokně Upravit **zásadu** zvolte Upravit vedle ovládacího prvku přístupu k dokumentům Office **,** rozbalte Spravovat přístup uživatelů k souborům na mobilních zařízeních **Office** ujistěte se, že je resetování  **PIN** kódu po neúspěšných pokusech nastavené na určité číslo.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="e4d4f-120">Ve výchozím nastavení je to 5.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="e4d4f-121">Na zařízení s Androidem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="e4d4f-122">Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="e4d4f-123">Zobrazí se výzva, která uvádí, že bylo dosaženo limitu pokusu **o pin** kód pro resetování PIN kódu.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="e4d4f-125">Stiskněte **Resetovat PIN kód**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-125">Press **Reset PIN**.</span></span> <span data-ttu-id="e4d4f-126">Zobrazí se výzva k přihlášení pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a pak budete muset nastavit nový PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="e4d4f-127">Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="e4d4f-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="e4d4f-128">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="e4d4f-130">Na zařízení s Androidem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a na vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-131">Otevřete e-mail, který obsahuje přílohu, a vedle informací o příloze klepněte na ikonu se šipkou dolů.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="e4d4f-133">V dolní části **obrazovky** se zobrazí možnost Nelze uložit do zařízení.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="e4d4f-135">V této chvíli není v Androidu ukládání na OneDrive pro firmy povoleno, takže vidíte jen zablokované místní ukládání.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="e4d4f-136">Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="e4d4f-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="e4d4f-137">V  podokně Upravit zásady  zvolte Upravit vedle ovládacího prvku přístupu k dokumentům Office **,** rozbalte Spravovat přístup uživatelů k souborům na mobilních zařízeních **Office** ujistěte se, že možnost Vyžadovat, aby se uživatelé znovu přihlašoval po nečinnosti aplikací **Office** byla nastavena na několik minut.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="e4d4f-138">Ve výchozím nastavení je to 30 minut.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="e4d4f-139">Na zařízení s Androidem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a na vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-p105">Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s Androidem nečinné aspoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="e4d4f-143">Znovu Outlook na zařízení s Androidem.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="e4d4f-144">Před tím, než budete mít přístup k Outlook, se zobrazí výzva k zadání kódu PIN.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="e4d4f-145">Ověření možnosti Chránit pracovní soubory šifrováním</span><span class="sxs-lookup"><span data-stu-id="e4d4f-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="e4d4f-146">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="e4d4f-147">Na zařízení s Androidem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a na vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-148">Otevřete e-mail, který obsahuje několik příloh obrázkových souborů.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="e4d4f-149">Klepnutím na ikonu šipky vedle informací o příloze soubory uložte.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="e4d4f-p106">Může se zobrazit výzva, abyste Outlooku na zařízení povolili přístup k fotkám, multimediálním a jiným souborům. Klepněte na **Povolit**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="e4d4f-153">Dole na obrazovce zvolte **Uložit do zařízení** a otevřete aplikaci **Galerie**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="e4d4f-p107">Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla být v seznamu. V seznamu obrázků by se měla zobrazit jako šedý čtvereček, který má uprostřed bílý vykřičník v kroužku.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="e4d4f-157">iOS</span><span class="sxs-lookup"><span data-stu-id="e4d4f-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="e4d4f-158">Kontrola nastavení ochrany aplikací na zařízeních uživatelů</span><span class="sxs-lookup"><span data-stu-id="e4d4f-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="e4d4f-159">Jakmile [nastavíte konfigurace aplikací pro zařízení s iOSem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="e4d4f-160">Nejdřív se ujistěte, že se zásady vztahují na aplikaci, ve které ji chcete ověřit.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="e4d4f-161">V Centru Microsoft 365 Business Premium [pro správu](https://admin.microsoft.com)přejděte na **Zásady pro** \> **úpravy zásad**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-161">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="e4d4f-162">Zvolte **Zásady aplikace pro iOS** pro nastavení, která jste vytvořili při instalaci, nebo jinou zásadu, kterou jste vytvořili, a ověřte, jestli je vynucovaná pro Outlook nastavení.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="e4d4f-164">Ověření možnosti Vyžadovat pro přístup k aplikacím Office PIN</span><span class="sxs-lookup"><span data-stu-id="e4d4f-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="e4d4f-165">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Ujistěte se, že je možnost Vyžadovat PIN kód nebo otisk prstu pro přístup Office aplikace nastavená na Hodnotu Zapnout.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="e4d4f-167">Na zařízení s iOS uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="e4d4f-168">Zobrazí se taky výzva k zadání PIN kódu nebo k použití otisku prstu.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="e4d4f-170">Ověření možnosti Resetovat PIN po několika neúspěšných pokusech</span><span class="sxs-lookup"><span data-stu-id="e4d4f-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="e4d4f-171">V podokně Upravit **zásadu** zvolte Upravit vedle ovládacího prvku přístupu k dokumentům Office **,** rozbalte Spravovat přístup uživatelů k souborům na mobilních zařízeních **Office** ujistěte se, že je resetování  **PIN** kódu po neúspěšných pokusech nastavené na určité číslo.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="e4d4f-172">Ve výchozím nastavení je to 5.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="e4d4f-173">Na zařízení s iOS uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="e4d4f-174">Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="e4d4f-175">Zobrazí se výzva, která uvádí, že bylo dosaženo limitu pokusu **o pin** kód pro resetování PIN kódu.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="e4d4f-177">Stiskněte **OK**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-177">Press **OK**.</span></span> <span data-ttu-id="e4d4f-178">Zobrazí se výzva k přihlášení pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a pak budete muset nastavit nový PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="e4d4f-179">Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="e4d4f-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="e4d4f-180">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="e4d4f-182">Na zařízení s iOSem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a v případě vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-183">Otevřete e-mail, který obsahuje přílohu. Přílohu otevřete a ve spodní části obrazovky zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="e4d4f-185">Měla by se zobrazit jen možnost OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="e4d4f-186">Pokud ne, **klepněte na Přidat účet** a **OneDrive pro firmy** na obrazovce Přidat **Storage účet.**</span><span class="sxs-lookup"><span data-stu-id="e4d4f-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="e4d4f-187">Po zobrazení výzvy zadejte, Microsoft 365 Business Premium se má koncový uživatel přihlásit.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="e4d4f-188">Klepněte na **Uložit** a vyberte **OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="e4d4f-189">Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="e4d4f-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="e4d4f-190">V  podokně Upravit zásady  zvolte Upravit vedle ovládacího prvku přístupu k dokumentům Office **,** rozbalte Spravovat přístup uživatelů k souborům na mobilních zařízeních **Office** ujistěte se, že možnost Vyžadovat, aby se uživatelé znovu přihlašoval po nečinnosti aplikací **Office** byla nastavena na několik minut.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="e4d4f-191">Ve výchozím nastavení je to 30 minut.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="e4d4f-192">Na zařízení s iOSem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a v případě vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-p113">Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s iOSem nečinné alespoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="e4d4f-196">Znovu Outlook na zařízení s iOSem.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="e4d4f-197">Před tím, než budete mít přístup k Outlook, se zobrazí výzva k zadání kódu PIN.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="e4d4f-198">Ověření možnosti Chránit pracovní soubory šifrováním</span><span class="sxs-lookup"><span data-stu-id="e4d4f-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="e4d4f-199">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="e4d4f-200">Na zařízení s iOSem uživatele otevřete Outlook a přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium uživatele a v případě vyžádání zadejte PIN kód.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="e4d4f-201">Otevřete e-mail, který obsahuje několik příloh obrázkových souborů.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="e4d4f-202">Klepněte na přílohu a potom klepněte níže na možnost **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="e4d4f-p114">Na domovské obrazovce otevřete aplikaci **Fotky**. Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla uložená, ale zašifrovaná.</span><span class="sxs-lookup"><span data-stu-id="e4d4f-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

