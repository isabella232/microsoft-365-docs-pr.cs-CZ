---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Zjistěte, jak vytvořit, upravit, nebo odstranit zásadu správy aplikace a ochrana souborů práce na Android nebo iOS zařízení.
ms.openlocfilehash: 21cc1d91c2952c6e9414d3742c26547fc36016a5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073504"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přejděte na stránku Správce na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. V levá navigace zvolte **zařízení** \> **zásad** \> **Přidat**.
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásady** zvolte **Správa aplikací pro Android** nebo **Správa aplikací pro iOS** (podle toho, jakou sadu zásad chcete vytvořit). 
    
5. Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. Další informace naleznete v tématu [nastavení k dispozici](#available-settings) . 
    
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

1. Na stránce **zásady** vyberte zásady a pak **Odstranit**.
    
2. **Odstranění zásady** podokně zvolte **Potvrdit** odstranění zásady nebo zásady, kterou jste zvolili. 
    
## <a name="available-settings"></a>Dostupná nastavení

Následující tabulky poskytují podrobné informace o dostupných nastaveních, která chrání pracovní soubory na zařízeních, a nastaveních, která spravují přístup uživatelů k souborům Office z mobilních zařízení.
  
 Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud se zařízení nebude používat určený počet dní, budou všechny pracovní soubory uložené na zařízení automaticky odstraněny.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **zapnuté**, jediným možným úložištěm pracovních souboru bude OneDrive pro firmy.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. Ani v případě ztráty nebo odcizení nebude moct nikdo data vaší společnosti přečíst.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.  <br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací  <br/> |Nám umožňují ve výchozím nastavení, ale jestliže je nastavena **na**uživatele by mohl zkopírovat informace v souboru pracovní soubor osobních. Pokud je toto nastavení **Vypnuto**, uživatel nebude možné kopírovat informace z pracovního účtu do osobní aplikace nebo osobní účet.  <br/> |
   

  

