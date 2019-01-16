---
title: Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Zjistěte, jak nastavit systém Windows zařízení systémem Windows 10 Pro Microsoft 365 Business uživatelům. '
ms.openlocfilehash: 482199b175c568bfae420619aa02024303894789
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982851"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business

## <a name="prerequisites"></a>Požadavky

Než začnete uživatelům služby Microsoft 365 Business nastavovat zařízení s Windows, ověřte, že na všech zařízeních běží Windows 10 Pro verze 1703 (Creators Update). Windows 10 Pro je předpokladem nasazení Windows 10 Business, což je sada cloudových služeb a funkcí pro správu zařízení. Tyto funkce a služby doplňují Windows 10 Pro a umožňují centralizovat ovládací prvky pro správu a zabezpečení systému Microsoft 365 Business.
  
Pokud máte zařízení, na kterých běží Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, máte v rámci předplatného Microsoft 365 Business nárok na upgrade na Windows 10.
  
Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Pokud chcete ověřit, že tento upgrade máte, nebo chcete zkontrolovat jeho funkčnost, přečtěte si část [Kontrola upgradu zařízení na Windows 10 Business](set-up-windows-devices.md#bkmk_verifywin10). 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Připojení zařízení s Windows 10 ke službě Azure AD organizace

Jakmile jsou všechna zařízení s Windows v organizaci upgradovaná na Windows 10 Pro Creators Update (nebo na nich tato verze už běží), můžete je připojit ke službě Azure Active Directory, kterou organizace používá. Jakmile zařízení připojíte, automaticky se upgradují na verzi Windows 10 Business, která je součástí předplatného Microsoft 365 Business.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Zcela nové nebo nově upgradované zařízení s Windows 10 Pro

U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.
  
1. Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Na této stránce zvolte **Nastavit pro organizaci** a zadejte uživatelské jméno a heslo Microsoft 365 Business. 
    
3. Dokončete nastavení zařízení s Windows 10.
    
   Po dokončení nastavení bude uživatel připojen k Azure AD organizace. Pokud chcete nastavení zkontrolovat, přečtěte si část [Kontrola připojení zařízení k Azure AD](set-up-windows-devices.md#bkmk_verifyaad). 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Nastavené zařízení se spuštěným systémem Windows 10 Pro

 **Připojení uživatelů k Azure AD:**
  
1. V uživatelském počítači se systémem Windows 10 Pro ve verzi 1703 (Creators Update) (viz [předpoklady](pre-requisites-for-data-protection.md)) klikněte na klávesu s logem Windows a potom na ikonu Nastavení.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. V **Nastavení** přejděte na **Účty**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Na stránce **Vaše informace** klikněte na **Přístup do práce nebo do školy** \> **Připojit**.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. V dialogovém okně **Nastavit pracovní nebo školní účet** v části **Alternativní akce** zvolte **Připojit toto zařízení k Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Na stránce **Řekněme získat jste přihlášen** , zadejte účtu práci a ve škole \> **Další**.
  
   Na stránce **Zadejte heslo** zadejte heslo \> **přihlásit**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na ** Přesvědčte se, zda je to organizace ** stránky, ověřte správnost informací a klepněte na tlačítko **Připojit**.
  
   Na stránce **Máte všechno nastavené** klikněte na **Hotovo**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače. Pokud jste k přenesení profilu a souborů použili nástroj třetí strany, synchronizujte je také s novým profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontrola připojení zařízení k Azure AD

Pokud si chcete ověřit stav synchronizace, klikněte v **Nastavení** na stránce **Přístup do práce nebo do školy** do oblasti **Připojeno k** _ \<organization name\> _, aby se zobrazila tlačítka **Informace** a **Odpojit**. Kliknutím na možnost **Informace** zjistíte stav synchronizace. 
  
Pokud chcete pro tento počítač získat nejnovější zásady správy mobilních zařízení, klikněte na stránce Stav synchronizace na Synchronizovat.
  
Když chcete začít účet Microsoft 365 Business používat, klikněte na tlačítko **Start** systému Windows, pravým tlačítkem klikněte na obrázek současného účtu a vyberte **Přepnout účet**. Přihlaste se e-mailem a heslem vaší organizace.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Kontrola upgradu zařízení na Windows 10 Business

Zkontrolujte, jestli zařízení s Windows 10 připojená k Azure AD byla v rámci předplatného Microsoft 365 Business upgradována na Windows 10 Business.
  
1. Přejděte na **Nastavení** \> **Systém** \> **O systému**.
    
2. Zkontrolujte, jestli **Edice** je **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Další kroky

Pokud chcete nastavit mobilní zařízení, přečtěte si článek [Nastavení mobilních zařízení pro uživatele služby Microsoft 365 Business](set-up-mobile-devices.md). Pokud chcete nastavit zásady ochrany zařízení nebo aplikací, přečtěte si článek [Správa Microsoft 365 Business](manage.md).
  
