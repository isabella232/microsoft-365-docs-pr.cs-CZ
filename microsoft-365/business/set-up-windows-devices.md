---
title: Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Dozvíte se, jak nastavit zařízení systému Windows se systémem Windows 10 pro pro Microsoft 365 obchodní uživatele. '
ms.openlocfilehash: b377c1e69d117b893b256880cd3b9972e33345c7
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2019
ms.locfileid: "39812872"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business

## <a name="prerequisites"></a>Požadavky

Než začnete uživatelům služby Microsoft 365 Business nastavovat zařízení s Windows, ověřte, že na všech zařízeních běží Windows 10 Pro verze 1703 (Creators Update). Windows 10 Pro je předpokladem nasazení Windows 10 Business, což je sada cloudových služeb a funkcí pro správu zařízení. Tyto funkce a služby doplňují Windows 10 Pro a umožňují centralizovat ovládací prvky pro správu a zabezpečení systému Microsoft 365 Business.
  
Pokud máte zařízení, na kterých běží Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, máte v rámci předplatného Microsoft 365 Business nárok na upgrade na Windows 10.
  
Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Další informace naleznete [v tématu ověření, zda je zařízení připojeno k Azure AD](#verify-the-device-is-connected-to-azure-ad) , abyste ověřili, zda máte upgrade nebo zda upgrade fungoval.

Sledujte krátké video o připojení systému Windows k aplikaci Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Pokud jste toto video našli, podívejte se na [kompletní tréninkové řady pro malé firmy a ty nové do společnosti Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Připojení zařízení s Windows 10 ke službě Azure AD organizace

Pokud byla všechna zařízení systému Windows ve vaší organizaci upgradována na systém Windows 10 pro autory nebo je již spuštěna aktualizace systému Windows 10 pro autory, můžete tato zařízení připojit k Azure Active Directory vaší organizace. Jakmile jsou zařízení připojena, budou automaticky upgradována na systém Windows 10 Business, který je součástí předplatného aplikace Microsoft 365 Business.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Zcela nové nebo nově upgradované zařízení s Windows 10 Pro

U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.
  
1. Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Na této stránce zvolte **Nastavit pro organizaci** a zadejte uživatelské jméno a heslo Microsoft 365 Business. 
    
3. Dokončete nastavení zařízení s Windows 10.
    
   Po dokončení nastavení bude uživatel připojen k Azure AD organizace. Pokud chcete nastavení zkontrolovat, přečtěte si část [Kontrola připojení zařízení k Azure AD](#verify-the-device-is-connected-to-azure-ad). 
  
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
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Na stránce **Zkontrolujte** , zda se jedná o stránku organizace, ověřte správnost informací a klepněte na tlačítko **připojit**.
  
   Na stránce **Máte všechno nastavené** klikněte na **Hotovo**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače. Pokud jste k migraci profilů a souborů použili nástroj jiného výrobce, synchronizujte je také s novým profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontrola připojení zařízení k Azure AD

Pokud si chcete ověřit stav synchronizace, klikněte v **Nastavení** na stránce **Přístup do práce nebo do školy** do oblasti **Připojeno k** _ \<organization name\> _, aby se zobrazila tlačítka **Informace** a **Odpojit**. Kliknutím na možnost **Informace** zjistíte stav synchronizace. 
  
Pokud chcete pro tento počítač získat nejnovější zásady správy mobilních zařízení, klikněte na stránce Stav synchronizace na Synchronizovat.
  
Chcete-li začít používat obchodní účet Microsoft 365 Business, přejděte na tlačítko **Start** systému Windows, klepněte pravým tlačítkem myši na aktuální obrázek účtu a poté **účet přepněte**. Přihlaste se e-mailem a heslem vaší organizace.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Kontrola upgradu zařízení na Windows 10 Business

Zkontrolujte, jestli zařízení s Windows 10 připojená k Azure AD byla v rámci předplatného Microsoft 365 Business upgradována na Windows 10 Business.
  
1. Přejděte na **Nastavení** \> **Systém** \> **O systému**.
    
2. Zkontrolujte, jestli **Edice** je **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Další kroky

Pokud chcete nastavit mobilní zařízení, přečtěte si článek [Nastavení mobilních zařízení pro uživatele služby Microsoft 365 Business](set-up-mobile-devices.md). Pokud chcete nastavit zásady ochrany zařízení nebo aplikací, přečtěte si článek [Správa Microsoft 365 Business](manage.md).
  
## <a name="see-also"></a>Viz také

[Microsoft 365 Business Training video](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
