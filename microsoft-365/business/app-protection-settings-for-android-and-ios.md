---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
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
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Přečtěte si, jak vytvořit, upravit nebo odstranit zásady správy aplikací a jak chránit pracovní soubory na zařízeních s Androidem nebo iOS.
ms.openlocfilehash: 67e7aaec5ff5a28f1e2d489913246c1c15c2f7b6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471193"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

Tento článek se týká Microsoft 365 Business Premium.

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přejděte do centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. V levém navigačním zařízení zvolte **Přidat** \> **zásady zařízení** \> **Add**.
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásad**zvolte Správa aplikací **pro Android** nebo Správa aplikací **pro iOS**v závislosti na tom, kterou sadu zásad chcete vytvořit. 
    
5. Rozbalte **Možnost Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a Spravovat přístup uživatelů k **souborům Office na mobilních zařízeních**. Nakonfigurujte nastavení podle chcení. **Správa způsobu, jakým uživatelé přistupují k souborům Office na mobilních zařízeních,** je ve výchozím nastavení **vypnutá,** ale doporučujeme **je** zapnout a přijmout výchozí hodnoty. Další informace naleznete v tématu [Dostupná nastavení](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete používat výchozí skupinu zabezpečení **Všichni uživatelé,** zvolte **Změnit**, zvolte skupiny zabezpečení, které tato nastavení \> **získají, vyberte**.
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="edit-an-app-management-policy"></a>Úprava zásady správy aplikací

1. Na kartě **Zásady** zvolte **Upravit zásady**.
    
2. V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit. 
    
3. Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když změníte hodnotu, automaticky se uloží do zásady.
    
4. Po dokončení zavřete podokno **Zásad úprav.** 
    
## <a name="delete-an-app-management-policy"></a>Odstranění zásady správy aplikací

1. Na stránce **Zásady** zvolte zásadu a potom **delete**.
    
2. V podokně **zásad Odstranit** zvolte Potvrdit, **chcete-li** odstranit zásady nebo zásady, které jste zvolili. 
    
## <a name="available-settings"></a>Dostupná nastavení

V následujících tabulkách jsou uvedeny podrobné informace o nastaveních, která jsou k dispozici pro ochranu pracovních souborů na zařízeních, a nastavení, která řídí přístup uživatelů k souborům Office ze svých mobilních zařízení.
  
 Další informace najdete v tématu [Jak se funkce ochrany v mapě Microsoft 365 Business Premium na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud se zařízení nepoužívá po dobu, po kterou zde zadáte, všechny pracovní soubory uložené v zařízení budou automaticky odstraněny.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **Zapnuto**, jediné dostupné umístění pro uložení pracovních souborů je OneDrive pro firmy.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. I když dojde ke ztrátě nebo odcizení zařízení, nikdo nemůže číst vaše firemní data.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **On** Uživatelé musí poskytnout jinou formu ověřování, kromě svého uživatelského jména a hesla, než budou moci používat aplikace Office na svých mobilních zařízeních.<br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se zobrazí výzva k opětovnému přihlášení.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Nepovolit uživatelům kopírování obsahu z aplikací Office do osobních aplikací  <br/> |Ve výchozím nastavení to povolujeme, ale pokud je nastavení **zapnuto**, může uživatel zkopírovat informace v pracovním souboru do osobního souboru. Pokud je nastavení **vypnuto**, uživatel nebude moci zkopírovat informace z pracovního účtu do osobní aplikace nebo osobního účtu.  <br/> |
