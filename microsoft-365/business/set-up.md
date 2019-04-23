---
title: Nastavení Microsoft 365 Business pomocí průvodce nastavením
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Zjistěte, jak nastavit Microsoft 365 Business podle čtyř kroků.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283881"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Nastavení Microsoft 365 Business pomocí průvodce nastavením

Proveďte kroky 1-4 níže.
  
### <a name="set-up-microsoft-365-business"></a>Nastavení Microsoft 365 Business

Podívejte se na video návod, jak nastavit Microsoft 365 Business, pokud nemáte místní služby Active Directory:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Informace o nastavení, které zahrnují místní adresář Active Directory zahrnuje následující kroky instalace. Pokud chcete získat přístup k zařízení připojeno k doméně, přečtěte si následující články pro dva jiný způsob povolení a proveďte kroky před spuštěním Průvodce instalací:
  
- [Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business](manage-windows-devices.md)
    
    -Toto je doporučený způsob.
    
- [Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Krok 1: Přizpůsobit přihlásit se

1. Přihlaste se k [Microsoft 365 Business](https://portal.microsoft.com) pod uživatelským jménem a heslem globálního správce. Vyberte dlaždici **Správce** a přejděte do Centra pro správu. 
    
2. V Centru pro správu zvolte **Spustit nastavení** (v závislosti na stavu se může zobrazit **Pokračovat v nastavení**) a spusťte průvodce. 
    
3. Zadejte název domény, který chcete použít (jako contoso.com).
    
    Zadejte svoji doménu, i pokud jste ji už ověřili například pomocí služby Azure AD Connect. Následující dva kroky na vás nemusí vztahovat, pokud se používá Azure AD připojit k ověření vaší domény.
    
4. Postupujte podle kroků v průvodci [vytvořit DNS záznamy na jakékoliv DNS poskytovatele hostitelských služeb pro Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) ověří, že jste vlastníkem domény. 
    
    Můžete zobrazit příklad video [Video: nastavení služeb Office 365 v nový Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Upozorňujeme, že toto video nezahrnuje postup k ochraně dat Microsoft 365 Business.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Krok 2: Přidání uživatelů a přiřazení licencí

1. Uživatele můžete přidat nyní nebo je můžete [přidat později](add-users-m365b.md) v Centru pro správu. 
    
    Každému přidanému uživateli se automaticky přiřadí licence Microsoft 365 Business.
    
2. Pokud vaše předplatné Microsoft 365 Business již uživatele má (například pokud jste použili službu Azure AD Connect), budete mít možnost jim licence přiřadit nyní. Neváhejte a přidejte licence i jim.
    
3. Budete mít také možnost přihlašovací údaje s nově přidanými uživateli sdílet. Můžete je vytisknout, poslat e-mailem nebo si je stáhnout.
    
4. Přesun e-mailových zpráv přeskočte a na stránce **Migrace e-mailových zpráv** zvolte **Další**. 
    
    Pokud přesouváte od jiného poskytovatele e-mailu a chcete zkopírovat data později, můžete [migrovat e-maily a kontakty do služeb Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Krok 3: Připojení domény

> [!NOTE]
> Pokud používáte domény .onmicrosoft nebo použít Azure AD připojit, nezobrazí se tento krok. 
  
Abyste mohli nastavit služby, musíte aktualizovat některé záznamy u svého hostitele DNS nebo doménového registrátora.
  
1. Průvodce nastavením obvykle rozpozná vašeho registrátora a poskytne odkaz na podrobné pokyny pro aktualizaci vašich záznamů názvového serveru na webu registrátora. Pokud tomu tak není, [Změna nameservers k nastavení služeb Office 365 pomocí libovolného registrátora domény](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. E-mail a další služby budou nastaveny za vás.
    
### <a name="step-4-manage-devices-and-work-files"></a>Krok 4: Správa zařízení a pracovní soubory

1. Na stránce **Chránit pracovní soubory na mobilních zařízení** přepněte možnosti **Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** do stavu **Zapnuto**. Dostanete každé dílčí nastavení klepnutím na šipky vedle každého nastavení.
  
  Všechny pracovní soubory licencovaných uživatelů jsou nyní chráněna na iOS a Android zařízení, jakmile jsou [instalace aplikací sady Office](set-up-mobile-devices.md) (a ověření pomocí pověření Microsoft 365 Business). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. Na stránce **Konfigurace zařízení Windows 10 nastavit** nastavte nastavení **Zabezpečení zařízení Windows 10** **On**.
  
   Dostanete každé dílčí nastavení klepnutím na dvojitou šipku vedle ní.
  
3. Pokud všichni vaši uživatelé mají počítače s Windows 10 a buď nemají existující instalace Office, nebo mají instalace Office Klikni a spusť, nastavte možnost **Instalace Office na zařízeních s Windows 10** na **Ano**. Pokud tomu tak není, nastavte možnost na **Ne**. Office také můžete [nainstalovat automaticky](auto-install-or-uninstall-office.md) z Centra pro správu později, až budete mít počítače uživatelů připravené. Pokyny naleznete v tématu [Příprava instalace klienta sady Office](prepare-for-office-client-deployment.md).
  
    Pracovní soubory licencovaných uživatelů na zařízeních s Windows 10 bude co nejdříve, jakmile budou promítat [připojit své zařízení Windows 10](set-up-windows-devices.md) obchodní Microsoft 365 Azure AD doméně nebo při současně spojující Microsoft 365 [Windows 10 do nového počítače nainstalovat](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) Obchodní domény Azure AD. 
  
4. Klikněte na **Další** a nastavení je hotové. 
  
    Podělte se s námi prosím o svůj názor, abyste nám pomohli vylepšit toto prostředí.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Další nastavení zabezpečení

Kromě zabezpečení a kompatibility nastavení v Průvodci instalací můžete také nastavit další parametry:
  
- Nastavení ochrany proti nebezpečným přílohám. **Advanced Threat Protection** (ATP) označuje škodlivý obsah a pak blokuje dodání nebezpečné přílohy, pomáhá chránit před podvodnými postupy typu phishing a ransomware infekcemi. Aktivaci ochrany přílohy naleznete v tématu [nastavení zásad bezpečné přílohy ATP Office 365](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Chrání vaše prostředí klepnutím na nebezpečné odkazy. ATP kontroluje odkazy v e-mailu v okamžiku kliknutí na ně. Pokud odkaz není bezpečné, uživatel je varován, aby na webu nebo informován, že webu byl zablokován. To pomáhá chránit před podvodnými postupy typu phishing. [Nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) nebo [nastavit zásady bezpečného propojení programů Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Můžete zachovat veškerý obsah poštovní schránky včetně vložením celé poštovní schránky uživatele na **soudní spory podržte**odstraněných položek. Pokyny naleznete v tématu 
- [Nastavení uchovávání e-mailů s Exchange Online archivaci](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Například nastavte vlastní **zásady uchovávání informací**má být zachována po určitou dobu nebo trvale odstranit obsah na konci období uchování informací Můžete povolit zásady uchovávání přizpůsobené s cennými papíry a centra kompatibility, přejděte do **správy věcí veřejných dat** \> **uchovávání informací**a pak postupujte podle kroků v průvodci. Další informace naleznete v tématu [Přehled zásad uchovávání informací](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>Další kroky

Pokud uživatelé mají licenci, nastaví si v dalším kroku zařízení.<br/> Další informace najdete v článcích [Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business](set-up-windows-devices.md) a [Nastavení mobilních zařízení pro uživatele služby Microsoft 365 Business](set-up-mobile-devices.md). <br/>Pokud hledáte odkazy na témata týkající se nastavení zásad ochrany zařízení a aplikací nebo chcete zjistit, jak odebrat data ze zařízení uživatelů, přečtěte si článek [Správa Microsoft 365 Business](manage.md). 
  


