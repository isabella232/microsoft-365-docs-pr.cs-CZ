---
title: Ověření nastavení ochrany aplikací na zařízeních se systémem Android nebo iOS
f1.keywords:
- NOCSH
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
description: Přečtěte si, jak ověřit nastavení ochrany aplikací Microsoft 365 Business na zařízeních s Androidem nebo iOS.
ms.openlocfilehash: f37bc262b3a80f4acb7113829e3d809ee16d41d1
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42091009"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Ověření nastavení ochrany aplikací na zařízeních se systémem Android nebo iOS

Podle pokynů v následujících částech ověřte nastavení ochrany aplikací na zařízeních se systémem Android nebo iOS.
  
## <a name="android"></a>Android
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Zkontrolujte, zda nastavení ochrany aplikací funguje na uživatelských zařízeních

Jakmile [nastavíte konfigurace aplikací pro zařízení s Androidem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení. 
  
Nejprve se ujistěte, že se zásady vztahují na aplikaci, ve které ji chcete ověřit.
  
1. V [Centru pro správu](https://portal.office.com) služby Microsoft 365 Business přejděte na **Zásady** \> **Upravit zásadu**.
    
2. Zvolte **Zásady aplikace pro Android** pro nastavení vytvořená při instalaci nebo jinou zásadu, kterou jste vytvořili, a ověřte, zda jsou vynuceny například pro Aplikaci Outlook. 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>Ověření nastavení Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu

V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.
  
![Ujistěte se, že je pro přístup k aplikacím Office nastavený kód Vyžadovat PIN kód nebo otisk prstu.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Na zařízení uživatele s Androidem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.
    
2. Budete také vyzváni k zadání KÓDU PIN nebo k použití otisku prstu.
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Ověření možnosti Resetovat PIN po několika neúspěšných pokusech

V podokně **Upravit zásady** zvolte **Upravit** vedle **ovládacího prvku přístupu k dokumentům Office**, rozbalte Možnost Spravovat přístup uživatelů **k souborům Office na mobilních zařízeních**a ujistěte se, že je **resetování kódu PIN po počtu neúspěšných pokusů** nastaveno na určité číslo. Toto je 5 ve výchozím nastavení. 
  
1. Na zařízení uživatele s Androidem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.
    
2. Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada. Zobrazí se výzva, ve které se zobrazí **limit pokusů o zadání PIN,** který má pin resetovat. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. Stiskněte **Resetovat PIN kód**. Budete vyzváni k přihlášení pomocí přihlašovacích údajů uživatele Microsoft 365 Business a poté budete muset nastavit nový kód PIN.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy

V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Otevřete e-mail, který obsahuje přílohu, a vedle informací o příloze klepněte na ikonu se šipkou dolů.
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    V dolní části obrazovky se zobrazí **možnost Uložit do zařízení.** 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > V této chvíli není v Androidu ukládání na OneDrive pro firmy povoleno, takže vidíte jen zablokované místní ukládání. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu

V podokně **Upravit zásady** zvolte **Upravit** vedle **ovládacího prvku přístupu k dokumentům Office**, rozbalte Možnost Spravovat přístup uživatelů **k souborům Office na mobilních zařízeních**a ujistěte se, že po nastavení aplikace **Office, aby se uživatelé znovu přihlásili,** je nastaveno na určitý počet minut. To je 30 minut ve výchozím nastavení. 
  
1. Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s Androidem nečinné aspoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.
    
3. Znovu přistupovat k Outlooku na zařízení Android.
    
4. Před znovu přístupem k Outlooku budete vyzváni k zadání kódu PIN.
    
### <a name="validate-protect-work-files-with-encryption"></a>Ověření možnosti Chránit pracovní soubory šifrováním

V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.
  
1. Na uživatelském zařízení s Androidem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Otevřete e-mail, který obsahuje několik příloh souboru obrázků.
    
3. Klepnutím na ikonu šipky vedle informací o příloze soubory uložte.
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Může se zobrazit výzva, abyste Outlooku na zařízení povolili přístup k fotkám, multimediálním a jiným souborům. Klepněte na **Povolit**.
    
5. Dole na obrazovce zvolte **Uložit do zařízení** a otevřete aplikaci **Galerie**. 
    
6. Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla být v seznamu. V seznamu obrázků by se měla zobrazit jako šedý čtvereček, který má uprostřed bílý vykřičník v kroužku.
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a>Ios
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Kontrola nastavení ochrany aplikací na zařízeních uživatelů

Jakmile [nastavíte konfigurace aplikací pro zařízení s iOSem](app-protection-settings-for-android-and-ios.md), abyste chránili aplikace, můžete tímto postupem ověřit funkčnost zvoleného nastavení. 
  
Nejprve se ujistěte, že se zásady vztahují na aplikaci, ve které ji chcete ověřit.
  
1. V [Centru pro správu](https://portal.office.com) služby Microsoft 365 Business přejděte na **Zásady** \> **Upravit zásadu**.
    
2. Zvolte **Zásady aplikace pro iOS** pro nastavení, která jste vytvořili při instalaci, nebo jinou zásadu, kterou jste vytvořili, a ověřte, zda jsou vynuceny pro aplikaci Outlook. 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>Ověření možnosti Vyžadovat pro přístup k aplikacím Office PIN

V podokně **Upravit zásadu** zvolte vedle **Řízení přístupu k dokumentům Office** možnost **Upravit**, rozbalte **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** a zkontrolujte, že volba **Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu** je nastavena na **Zapnuto**.
  
![Ujistěte se, že je pro přístup k aplikacím Office nastavený kód Vyžadovat PIN kód nebo otisk prstu.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Na zařízení uživatele s iOSem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.
    
2. Budete také vyzváni k zadání KÓDU PIN nebo k použití otisku prstu.
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Ověření možnosti Resetovat PIN po několika neúspěšných pokusech

V podokně **Upravit zásady** zvolte **Upravit** vedle **ovládacího prvku přístupu k dokumentům Office**, rozbalte Možnost Spravovat přístup uživatelů **k souborům Office na mobilních zařízeních**a ujistěte se, že je **resetování kódu PIN po počtu neúspěšných pokusů** nastaveno na určité číslo. Toto je 5 ve výchozím nastavení. 
  
1. Na zařízení uživatele s iOSem otevřete Outlook a přihlaste se pomocí uživatelského jména a hesla Microsoft 365 Business.
    
2. Zadejte nesprávný PIN tolikrát, kolikrát to dovoluje nastavená zásada. Zobrazí se výzva, ve které se zobrazí **limit pokusů o zadání PIN,** který má pin resetovat. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. Stiskněte **OK**. Budete vyzváni k přihlášení pomocí přihlašovacích údajů uživatele Microsoft 365 Business a poté budete muset nastavit nový kód PIN.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Ověření možnosti Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy

V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že je možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** nastavená na **Zapnuto**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Otevřete e-mail, který obsahuje přílohu. Přílohu otevřete a ve spodní části obrazovky zvolte **Uložit**. 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. Měla by se zobrazit jen možnost OneDrive pro firmy. Pokud ne, klepněte na **Přidat účet** a na obrazovce Přidat **účet úložiště** vyberte **OneDrive pro firmy.** Po zobrazení výzvy zadejte přihlašovací údaje koncového uživatele pro Microsoft 365 Business. 
    
    Klepněte na **Uložit** a vyberte **OneDrive pro firmy**.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Ověření možnosti Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu

V podokně **Upravit zásady** zvolte **Upravit** vedle **ovládacího prvku přístupu k dokumentům Office**, rozbalte Možnost Spravovat přístup uživatelů **k souborům Office na mobilních zařízeních**a ujistěte se, že po nastavení aplikace **Office, aby se uživatelé znovu přihlásili,** je nastaveno na určitý počet minut. To je 30 minut ve výchozím nastavení. 
  
1. Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Měla by se zobrazit doručená pošta Outlooku. Nechte zařízení s iOSem nečinné alespoň 30 minut (nebo o něco déle, než jste zadali v zásadě). Obrazovka zařízení pravděpodobně ztmavne.
    
3. Znovu přistupovat k Outlooku na iOS zařízení.
    
4. Před znovu přístupem k Outlooku budete vyzváni k zadání kódu PIN.
    
### <a name="validate-protect-work-files-with-encryption"></a>Ověření možnosti Chránit pracovní soubory šifrováním

V podokně **Upravit zásadu** zvolte vedle **Ochrana v případě ztráty nebo odcizení zařízení** možnost **Upravit**, rozbalte možnost **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a zkontrolujte, že **ochrana pracovních souborů šifrováním** je nastavená na **Zapnuto** a možnost **Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy** je nastavená na **Vypnuto**.
  
1. Na uživatelském zařízení s iOSem otevřete Outlook a přihlaste se pod uživatelským jménem a heslem Microsoft 365 Business. Pokud k tomu budete vyzváni, zadejte PIN.
    
2. Otevřete e-mail, který obsahuje několik příloh souboru obrázků.
    
3. Klepněte na přílohu a potom klepněte níže na možnost **Uložit**. 
    
4. Na domovské obrazovce otevřete aplikaci **Fotky**. Šifrovaná fotka (nebo více fotek, pokud jste uložili více příloh obrázkových souborů) by měla uložená, ale zašifrovaná. 
    
---

