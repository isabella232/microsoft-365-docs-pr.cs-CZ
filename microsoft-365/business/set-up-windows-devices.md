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
description: Přečtěte si, jak nastavit zařízení s Windows s Windows 10 Pro pro uživatele Microsoft 365 Business Premium, což umožňuje centralizovanou správu a bezpečnostní kontroly.
ms.openlocfilehash: ecd9f5aa348d29d34e77061657619c015b09c41a
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402952"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Požadavky na nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium

Než budete moci nastavit zařízení s Windows pro uživatele Microsoft 365 Business Premium, ujistěte se, že všechna zařízení s Windows používají Windows 10 Pro verze 1703 (Aktualizace tvůrců). Windows 10 Pro je předpokladem pro nasazení Windows 10 Business, což je sada cloudových služeb a funkcí pro správu zařízení, které doplňují Windows 10 Pro a umožňují centralizovanou správu a bezpečnostní kontroly Microsoft 365 Business Premium.
  
Pokud máte zařízení s Windows 7 Pro, Windows 8 Pro nebo Windows 8.1 Pro, vaše předplatné Microsoft 365 Business Premium vás opravňuje k upgradu na Windows 10.
  
Další informace o upgradu zařízení s Windows na Windows 10 Pro Creators Update najdete v krocích popsaných v tomto tématu: [Upgrade zařízení s Windows na Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Viz [Ověření zařízení připojeného k Azure AD](#verify-the-device-is-connected-to-azure-ad) ověřit, že máte upgrade, nebo ujistěte se, že upgrade funguje.

Podívejte se na krátké video o připojení Windows k Microsoftu 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Pokud bylo pro vás toto video užitečné, můžete se podívat na [kompletní sérii školení určených pro malé firmy a pro firmy, které se s Microsoftem 365 teprve seznamují](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Připojení zařízení s Windows 10 ke službě Azure AD organizace

Když byla všechna zařízení s Windows ve vaší organizaci upgradována na aktualizaci Windows 10 Pro Creators Update nebo už používáte aktualizaci Windows 10 Pro Creators Update, můžete se k těmto zařízením připojit do služby Azure Active Directory vaší organizace. Jakmile se zařízení připojí, automaticky se upgradují na Windows 10 Business, který je součástí vašeho předplatného Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Zcela nové nebo nově upgradované zařízení s Windows 10 Pro

U zcela nového zařízení, na kterém běží Windows 10 Pro Creators Update, nebo u zařízení, které sice bylo upgradováno na Windows 10 Pro Creators Update, ale neproběhlo u něj nastavení zařízení s Windows 10, použijte tento postup.
  
1. Projděte nastavení zařízení s Windows 10, dokud se nezobrazí stránka **Jak se má zařízení nastavit**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Tady zvolte **Nastavit pro organizaci** a zadejte své uživatelské jméno a heslo pro Microsoft 365 Business Premium. 
    
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
  
6. Na stránce **Ujistěte se, že se jedná** o organizaci, ověřte, zda jsou informace správné, a klepněte na tlačítko **Připojit se**.
  
   Na stránce **Máte všechno nastavené** klikněte na **Hotovo**.
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Pokud jste nahráli soubory na OneDrive pro firmy, synchronizujte je zpět do počítače. Pokud jste k migraci profilu a souborů použili nástroj jiného výrobce, synchronizujte je také s novým profilem.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontrola připojení zařízení k Azure AD

Chcete-li ověřit stav synchronizace, klikněte na stránce **Práce nebo škola aplikace Access** v **nastavení**v oblasti **Připojeno k aplikaci** _ a \<organization name\> zpřístupněte tlačítka **Informace** a **Odpojit**. Kliknutím na možnost **Informace** zjistíte stav synchronizace. 
  
Pokud chcete pro tento počítač získat nejnovější zásady správy mobilních zařízení, klikněte na stránce Stav synchronizace na Synchronizovat.
  
Pokud chcete začít používat účet Microsoft 365 Business Premium, přejděte na tlačítko **Start** systému Windows, klikněte pravým tlačítkem myši na obrázek aktuálního účtu a potom **přepněte účet**. Přihlaste se e-mailem a heslem vaší organizace.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Kontrola upgradu zařízení na Windows 10 Business

Ověřte, že vaše azure ad připojená zařízení s Windows 10 byla upgradována na Windows 10 Business jako součást předplatného Microsoft 365 Business Premium.
  
1. Přejděte na **Nastavení** \> **Systém** \> **O systému**.
    
2. Zkontrolujte, jestli **Edice** je **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Další kroky

Informace o nastavení mobilních zařízení najdete v tématu [Nastavení mobilních zařízení pro uživatele Služby Microsoft 365 Business Premium](set-up-mobile-devices.md), Nastavení ochrany zařízení nebo zásad ochrany aplikací najdete v [tématu Správa Microsoftu 365 pro firmy](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Další informace o nastavení a používání Microsoft 365 Business Premium

[Microsoft 365 pro firemní školicí videa](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
