---
title: Ověření nastavení ochrany aplikace u zařízení Android nebo iOS
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
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Zjistěte, jak ověřit nastavení ochrany Microsoft 365 Business app v zařízeních Android nebo iOS.
ms.openlocfilehash: 309dbf5bdba81bbf8ad0a9707c136a03c4a28586
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575522"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="c4e4d-103">Ověření nastavení ochrany aplikace u zařízení Android nebo iOS</span><span class="sxs-lookup"><span data-stu-id="c4e4d-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="c4e4d-104">Podle pokynů v následujících oddílech ověřte nastavení ochrany aplikace u zařízení Android nebo iOS.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="c4e4d-105">Android</span><span class="sxs-lookup"><span data-stu-id="c4e4d-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="c4e4d-106">Kontrola nastavení ochrany aplikací na zařízeních uživatelů</span><span class="sxs-lookup"><span data-stu-id="c4e4d-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="c4e4d-107">Jakmile [nastavíte konfigurace aplikací pro zařízení s Androidem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="c4e4d-108">Napřed zkontrolujte, jestli zásada platí pro aplikaci, ve které ji budete ověřovat.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="c4e4d-109">V [Centru pro správu](https://portal.office.com) služby Microsoft 365 Business přejděte na **Zásady** \> **Upravit zásadu**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="c4e4d-110">Pro nastavení, které jste vytvořili při nastavení, zvolte **Zásady aplikace pro Android** (nebo jinou vytvořenou zásadu) a ověřte, že se dodržuje například pro Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="c4e4d-112">Ověření nastavení Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu</span><span class="sxs-lookup"><span data-stu-id="c4e4d-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="c4e4d-113">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="c4e4d-115">Na zařízení uživatele s Androidem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4e4d-116">Také se zobrazí výzva k zadání kódu PIN nebo použití otisku prstu.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="c4e4d-118">Ověření možnosti Resetovat PIN po několika neúspěšných pokusech</span><span class="sxs-lookup"><span data-stu-id="c4e4d-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="c4e4d-119">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Resetovat PIN kód po tomto počtu neúspěšných přihlášení** je nastavená na nějaké číslo. Výchozí nastavení je 5.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="c4e4d-120">Na zařízení uživatele s Androidem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4e4d-p101">Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada. Před resetováním kódu PIN se zobrazí výzva **Dosáhli jste maximálního počtu pokusů o zadání PIN kódu**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="c4e4d-p102">Stiskněte **Resetovat PIN kód**. Zobrazí se výzva, abyste k přihlášení použili uživatelské jméno a heslo Microsoft 365 Business, a pak musíte nastavit nový PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="c4e4d-126">Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="c4e4d-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="c4e4d-127">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="c4e4d-129">Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-130">Otevřete e-mail, který obsahuje přílohu, a vedle informací o příloze klepněte na ikonu se šipkou dolů.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="c4e4d-132">Dole na obrazovce se zobrazí zpráva, že **není možné ukládat do zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="c4e4d-134">V této chvíli není v Androidu ukládání na OneDrive pro firmy povoleno, takže vidíte jen zablokované místní ukládání.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="c4e4d-135">Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="c4e4d-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="c4e4d-136">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že možnost **Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu** je nastavená na určitý počet minut. Výchozí hodnota je 30 minut.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="c4e4d-137">Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-p103">Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s Androidem nečinné aspoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="c4e4d-141">Na zařízení s Androidem znovu otevřete Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="c4e4d-142">Před opětovným otevřením Outlooku budete vyzváni k zadání kódu PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="c4e4d-143">Ověření možnosti Chránit pracovní soubory šifrováním</span><span class="sxs-lookup"><span data-stu-id="c4e4d-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="c4e4d-144">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="c4e4d-145">Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-146">Otevřete e-mail, který má jako přílohu několik obrázkových souborů.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="c4e4d-147">Klepnutím na ikonu šipky vedle informací o příloze soubory uložte.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="c4e4d-p104">Může se zobrazit výzva, abyste Outlooku na zařízení povolili přístup k fotkám, multimediálním a jiným souborům. Klepněte na **Povolit**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="c4e4d-151">Dole na obrazovce zvolte **Uložit do zařízení** a otevřete aplikaci **Galerie**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="c4e4d-p105">Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla být v seznamu. V seznamu obrázků by se měla zobrazit jako šedý čtvereček, který má uprostřed bílý vykřičník v kroužku.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="c4e4d-155">Ios</span><span class="sxs-lookup"><span data-stu-id="c4e4d-155">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="c4e4d-156">Kontrola nastavení ochrany aplikací na zařízeních uživatelů</span><span class="sxs-lookup"><span data-stu-id="c4e4d-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="c4e4d-157">Jakmile [nastavíte konfigurace aplikací pro zařízení s iOSem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="c4e4d-158">Napřed zkontrolujte, jestli zásada platí pro aplikaci, ve které ji budete ověřovat.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="c4e4d-159">V [Centru pro správu](https://portal.office.com) služby Microsoft 365 Business přejděte na **Zásady** \> **Upravit zásadu**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="c4e4d-160">Pro nastavení, které jste vytvořili při nastavování, zvolte **Zásady použití pro iOS** (nebo jinou vytvořenou zásadu) a ověřte, že se dodržuje například pro Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="c4e4d-162">Ověření možnosti Vyžadovat pro přístup k aplikacím Office PIN</span><span class="sxs-lookup"><span data-stu-id="c4e4d-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="c4e4d-163">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="c4e4d-165">Na zařízení uživatele s iOSem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4e4d-166">Také se zobrazí výzva k zadání kódu PIN nebo použití otisku prstu.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="c4e4d-168">Ověření možnosti Resetovat PIN po několika neúspěšných pokusech</span><span class="sxs-lookup"><span data-stu-id="c4e4d-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="c4e4d-169">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Resetovat PIN kód po tomto počtu neúspěšných přihlášení** je nastavená na nějaké číslo. Výchozí nastavení je 5.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="c4e4d-170">Na zařízení uživatele s iOSem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4e4d-p106">Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada. Před resetováním kódu PIN se zobrazí výzva **Dosáhli jste maximálního počtu pokusů o zadání PIN kódu**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="c4e4d-p107">Stiskněte **OK**. Zobrazí se výzva, abyste k přihlášení použili uživatelské jméno a heslo Microsoft 365 Business, a pak musíte nastavit nový PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="c4e4d-176">Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy</span><span class="sxs-lookup"><span data-stu-id="c4e4d-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="c4e4d-177">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="c4e4d-179">Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-180">Otevřete e-mail, který obsahuje přílohu. Přílohu otevřete a ve spodní části obrazovky zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="c4e4d-p108">Měla by se zobrazit jen možnost OneDrive pro firmy. Pokud tomu tak není, klepněte na **Přidat účet** a z obrazovky **Přidat účet úložiště** vyberte **OneDrive pro firmy**. Po zobrazení výzvy zadejte přihlašovací údaje koncového uživatele pro Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="c4e4d-185">Klepněte na **Uložit** a vyberte **OneDrive pro firmy**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="c4e4d-186">Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu</span><span class="sxs-lookup"><span data-stu-id="c4e4d-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="c4e4d-187">V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že možnost **Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu** je nastavená na určitý počet minut. Výchozí hodnota je 30 minut.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="c4e4d-188">Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-p109">Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s iOSem nečinné alespoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="c4e4d-192">Na zařízení s iOSem znovu otevřete Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="c4e4d-193">Před opětovným otevřením Outlooku budete vyzváni k zadání kódu PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="c4e4d-194">Ověření možnosti Chránit pracovní soubory šifrováním</span><span class="sxs-lookup"><span data-stu-id="c4e4d-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="c4e4d-195">V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="c4e4d-196">Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4e4d-197">Otevřete e-mail, který má jako přílohu několik obrázkových souborů.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="c4e4d-198">Klepněte na přílohu a potom klepněte níže na možnost **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="c4e4d-p110">Na domovské obrazovce otevřete aplikaci **Fotky**. Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla uložená, ale zašifrovaná.</span><span class="sxs-lookup"><span data-stu-id="c4e4d-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

