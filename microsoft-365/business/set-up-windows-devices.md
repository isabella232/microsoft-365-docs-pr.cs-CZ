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
description: Zjistěte, jak nastavit zařízení s Windows s Windows 10 pro pro Microsoft 365 Business Premium Users, která umožňují centralizované správy a řízení zabezpečení.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841253"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Předpoklady pro nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium

Než budete moct nastavit zařízení s Windows pro uživatele Microsoft 365 Business Premium, ujistěte se, že všechna zařízení s Windows používají Windows 10 pro, verze 1703 (Creators Update). Windows 10 pro je nezbytný předpoklad pro nasazení Windows 10 Business, což je sada cloudových služeb a možností správy zařízení, které doplňují Windows 10 pro a umožňují centralizovanou správu a kontroly zabezpečení Microsoft 365 Business Premium.
  
Pokud máte zařízení s Windows ve Windows 7 pro, Windows 8 pro nebo Windows 8,1 pro, vaše předplatné Microsoft 365 Business Premium vás opravňuje k upgradu na Windows 10.
  
Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Podívejte se na článek [ověření, jestli je zařízení připojené ke službě Azure AD](#verify-the-device-is-connected-to-azure-ad) , abyste ověřili, že máte upgrade, nebo jestli jste upgrade nefungoval.

Podívejte se na krátké video o připojení Windows k Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Připojení zařízení s Windows 10 ke službě Azure AD organizace

Když se všechna zařízení s Windows ve vaší organizaci upgradují na Windows 10 pro Creators Update nebo už používají Windows 10 pro Creator Update, můžete tato zařízení připojit k Azure Active Directory vaší organizace. Jakmile se zařízení připojí, budou se automaticky upgradovat na Windows 10 Business, který je součástí předplatného Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Zcela nové nebo nově upgradované zařízení s Windows 10 Pro

U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.
  
1. Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Tady vyberte **nastavení pro organizaci** a pak zadejte uživatelské jméno a heslo pro Microsoft 365 Business Premium. 
    
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
  
6. Na stránce Ujistěte se, že **je to vaše organizace** , zkontrolujte správnost informací a zvolte **připojit** se.
  
   Na stránce **máte všechno.** Stránka **, Chosse.**
  
   ![Na obrazovce Ujistěte se, že se jedná o vaši organizaci, zvolte připojit se.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače. Pokud jste k migraci profilu a souborů použili nástroj třetí strany, synchronizujte ho taky s novým profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontrola připojení zařízení k Azure AD

Chcete-li ověřit stav synchronizace, vyberte v **Nastavení** na stránce **Access Work nebo School** ( **připojit** do _ _) \<organization name\> **informace** o tlačítkách a **odpojte** se. Zvolte **informace** pro zjištění stavu synchronizace. 
  
Na stránce **stav synchronizace** zvolte **synchronizovat** a získejte nejnovější zásady správy mobilních zařízení na počítači.
  
Pokud chcete začít používat účet Microsoft 365 Business Premium, přejděte na tlačítko **Start** systému Windows, klikněte pravým tlačítkem myši na svůj obrázek aktuálního účtu a potom na **Přepnout účet**. Přihlaste se e-mailem a heslem vaší organizace.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Ověření upgradu počítače na Windows 10 Business

Ověřte, že zařízení s Windows 10 připojená k Azure AD jsou v rámci předplatného Microsoft 365 Business Premium upgradovaná na Windows 10 Business.
  
1. Přejděte na **Nastavení** \> **Systém** \> **O systému**.
    
2. Zkontrolujte, jestli **Edice** je **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Další kroky

Pokud chcete nastavit mobilní zařízení, přečtěte si článek [nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium](set-up-mobile-devices.md), která umožňují nastavit ochranu zařízení nebo [365](manage.md)zásady ochrany aplikací.
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Další informace o nastavení a používání Microsoft 365 Business Premium

[Školicí kurzy pro Microsoft 365 for Business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
