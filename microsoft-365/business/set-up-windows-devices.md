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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Nastavte Windows zařízení s Windows 10 Pro pro Microsoft 365 Business Premium a povolte centralizovanou správu a ovládací prvky zabezpečení.
ms.openlocfilehash: 0a38a244ca997cfadb46c3833c0587e0c4f79fe3d32b90c6d92f08069b352bd3
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837711"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Nastavení Windows pro Microsoft 365 Business Premium uživatele

## <a name="before-you-begin"></a>Než začnete

Než budete moci nastavit Windows pro Microsoft 365 Business Premium, zkontrolujte, jestli jsou všechna Windows zařízení Windows 10 Pro, verze 1703 (Creators Update). Windows 10 Pro je předpokladem pro nasazení Windows 10 Business, což je sada cloudových služeb a možností správy zařízení, které doplňují Windows 10 Pro a umožňují centralizovanou správu a řízení zabezpečení Microsoft 365 Business Premium.
  
Pokud máte zařízení Windows Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné Microsoft 365 Business Premium vás opravňuje k Windows 10 upgradu.
  
Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Informace [o tom, jestli](#verify-the-device-is-connected-to-azure-ad) máte upgrade, najdete v článku Ověření připojení zařízení k Azure AD nebo ověření, jestli upgrade fungoval.

## <a name="watch-connect-your-pc-to-microsoft-365-business"></a>Přehrát: Připojení počítač do Microsoft 365 Business

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Připojení zařízení s Windows 10 ke službě Azure AD organizace

Když jsou Windows zařízení ve vaší organizaci upgradovaná na aktualizaci Windows 10 Pro Creators Update nebo už máte spuštěnou aktualizaci Windows 10 Pro Creators Update, můžete tato zařízení připojit k Azure Active Directory vaší Azure Active Directory. Po přihlášení se zařízení automaticky upgradují na Windows 10 Business, které je součástí vašeho Microsoft 365 Business Premium předplatného.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Zcela nové nebo nově upgradované zařízení s Windows 10 Pro

U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.
  
1. Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Tady zvolte **Nastavit pro organizaci a** zadejte svoje uživatelské jméno a heslo pro Microsoft 365 Business Premium. 
    
3. Dokončete nastavení zařízení s Windows 10.
    
   Po dokončení nastavení bude uživatel připojen k Azure AD organizace. Pokud chcete nastavení zkontrolovat, přečtěte si část [Kontrola připojení zařízení k Azure AD](#verify-the-device-is-connected-to-azure-ad). 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Nastavené zařízení se spuštěným systémem Windows 10 Pro

 **Připojení uživatelů k Azure AD:**
  
1. V uživatelském počítači se systémem Windows 10 Pro ve verzi 1703 (Creators Update) (viz [předpoklady](pre-requisites-for-data-protection.md)) klikněte na klávesu s logem Windows a potom na ikonu Nastavení.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. V **Nastavení** přejděte na **Účty**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na stránce **Vaše informace** klikněte na **Přístup do práce nebo do školy** \> **Připojit**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. V dialogovém okně **Nastavit pracovní nebo školní účet** v části **Alternativní akce** zvolte **Připojit toto zařízení k Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na stránce **Zkontrolujte, jestli je to vaše** organizace, ověřte, jestli jsou informace správné, a zvolte Připojit **se.**
  
   Na **sadě Jste všichni!** stránka, chosse Done ( **Hotovo).**
  
   ![Na obrazovce Ujistěte se, že je to vaše organizace, zvolte Připojit se.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače. Pokud jste k migraci profilu a souborů použili nástroj jiného výrobce, synchronizujte je taky s novým profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontrola připojení zařízení k Azure AD

Pokud chcete ověřit stav synchronizace, vyberte na pracovní nebo školní  stránce **Accessu** **v Nastavení** oblast Připojeno k _ _ a zobrazí se tlačítka Informace a \<organization name\> **Odpojit.**  Pokud **chcete získat** stav synchronizace, zvolte Informace. 
  
Na stránce **Stav** synchronizace  zvolte Synchronizovat a získejte nejnovější zásady správy mobilních zařízení do počítače.
  
Pokud chcete začít Microsoft 365 Business Premium účtu, přejděte na tlačítko Windows **Start,** klikněte pravým tlačítkem myši na obrázek aktuálního účtu a potom **na Přepnout účet**. Přihlaste se e-mailem a heslem vaší organizace.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Ověření upgradu počítače na Windows 10 Business

Ověřte, jestli jsou vaše zařízení připojená Windows 10 Azure AD upgradovaná na Windows 10 Business jako součást vašeho předplatného Microsoft 365 Business Premium služby.
  
1. Přejděte na **Nastavení** \> **Systém** \> **O systému**.
    
2. Zkontrolujte, jestli **Edice** je **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Další kroky

Informace o nastavení mobilních zařízení najdete v tématu Nastavení mobilních zařízení pro [Microsoft 365 Business Premium](set-up-mobile-devices.md)uživatelů , Nastavení ochrany zařízení nebo zásad ochrany aplikací v tématu Správa [Microsoft 365 pro firmy](manage.md).
  
## <a name="related-content"></a>Související obsah

[Microsoft 365 pro firemní školicí videa](../business-video/index.yml) (stránka odkazu)
