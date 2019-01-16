---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Zjistěte, jak vytvořit, upravit, nebo odstranit zásadu správy aplikace a ochrana souborů práce na Android nebo iOS zařízení.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983661"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přihlaste se k [Microsoft 365 Business](https://portal.office.com) pod uživatelským jménem a heslem globálního správce. 
    
2. V Centru pro správu přejděte na kartu **Zásady zařízení** a zvolte **Přidat zásadu**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásady** zvolte **Správa aplikací pro Android** nebo **Správa aplikací pro iOS** (podle toho, jakou sadu zásad chcete vytvořit). 
    
5. Rozbalte položku **Zamknout pracovní soubory, pokud jsou ztráty nebo krádeže zařízení** a **Správa přístupu uživatelů na soubory sady Office na mobilních zařízeních** \> nastavit, jakým způsobem. **Správa přístupu uživatelů na soubory sady Office na mobilních zařízeních** je **Vypnuto** ve výchozím nastavení, ale je vhodné **jej zapnout** a přijměte výchozí hodnoty. Další informace naleznete v tématu [nastavení k dispozici](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) . 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="edit-an-app-management-policy"></a>Úprava zásady správy aplikací

1. Na kartě **zásady** klepněte na příkaz **Upravit zásady**.
    
2. V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit. 
    
3. Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když hodnotu změníte, automaticky se do zásady uloží. 
    
4. Jakmile skončíte, podokno **Upravit zásadu** zavřete. 
    
## <a name="delete-an-app-management-policy"></a>Odstranění zásady správy aplikací

1. Na kartě **Zásady** zvolte **Odstranit zásadu**.
    
2. V podokně **Odstranit zásadu** zvolte zásady, které chcete odstranit \> **Vybrat** a potom vybranou zásadu nebo zásady odstraňte kliknutím na **Potvrdit**. 
    
## <a name="available-settings"></a>Dostupná nastavení

Následující tabulky poskytují podrobné informace o dostupných nastaveních, která chrání pracovní soubory na zařízeních, a nastaveních, která spravují přístup uživatelů k souborům Office z mobilních zařízení.
  
 Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Následující nastavení jsou k dispozici pro ochranu pracovních souborů, když se zařízení uživatele ztratí nebo je odcizeno:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud se zařízení nebude používat určený počet dní, budou všechny pracovní soubory uložené na zařízení automaticky odstraněny.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **zapnuté**, jediným možným úložištěm pracovních souboru bude OneDrive pro firmy.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení ponechte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. Ani v případě ztráty nebo odcizení nebude moct nikdo data vaší společnosti přečíst.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.  <br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. Uživatel takového zařízení může měnit operační systém, ale jeho zařízení je náchylnější k malwarovým útokům. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací  <br/> |Nám umožňují ve výchozím nastavení, ale jestliže je nastavena **na**uživatele by mohl zkopírovat informace v souboru pracovní soubor osobních. Pokud je toto nastavení **Vypnuto**, uživatel nebude možné kopírovat informace z pracovního účtu do osobní aplikace nebo osobní účet.<br/> |
   

  

