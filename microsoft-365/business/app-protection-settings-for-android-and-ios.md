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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Naučte se vytvářet, upravovat nebo odstraňovat zásady správy aplikací a chránit pracovní soubory na zařízeních Android nebo iOS.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321839"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

![To je nápis https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přejděte do centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>adrese. 
    
2. V levém navigačním okně zvolte položku **** \> **zásady** \> zařízení **Add**.
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásady**vyberte položku **Správa aplikací pro Android** nebo **správu aplikací pro iOS**podle toho, kterou sadu zásad chcete vytvořit. 
    
5. Rozbalení **chránit pracovní soubory při ztrátě nebo odcizení zařízení** a **správě přístupu uživatelů k souborům sady Office na mobilních zařízeních** Nastavte požadované nastavení. **Správa přístupu uživatelů k souborům sady Office na mobilních zařízeních** je ve výchozím nastavení **vypnuta** , doporučujeme jej však **zapnout a přijmout** výchozí hodnoty. Další informace naleznete v tématu [dostupné nastavení](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **All Users** , zvolte možnost **změnit**, zvolte skupiny zabezpečení, které \> **Toto nastavení zvolí**.
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="edit-an-app-management-policy"></a>Úprava zásady správy aplikací

1. Na kartě **zásady** zvolte možnost **upravit zásady**.
    
2. V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit. 
    
3. Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Změníte-li hodnotu, bude automaticky uložena do zásady.
    
4. Po dokončení zavřete podokno **zásad úprav** . 
    
## <a name="delete-an-app-management-policy"></a>Odstranění zásady správy aplikací

1. Na stránce **zásady** zvolte zásadu a pak ji **odstraňte**.
    
2. V podokně **zásad odstranění** zvolte možnost **Potvrdit** odstranění zvolených zásad nebo zásad. 
    
## <a name="available-settings"></a>Dostupná nastavení

Následující tabulky obsahují podrobné informace o dostupných nastaveních pro ochranu pracovních souborů na zařízeních a nastavení, které řídí způsob, jakým uživatelé přistupují k souborům sady Office z mobilních zařízení.
  
 Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud zařízení není používáno po dobu, kterou zde zadáte, budou všechny pracovní soubory uložené v zařízení automaticky odstraněny.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **zapnuto**, jediné dostupné umístění pro uložení pracovních souborů je OneDrive for Business.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. I když dojde ke ztrátě nebo odcizení zařízení, nikdo nemůže číst data vaší společnosti.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **zapnuto** , musí uživatelé před použitím aplikací sady Office na mobilních zařízeních poskytnout další způsob ověřování, a to kromě uživatelského jména a hesla.<br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se znovu zobrazí výzva k přihlášení.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací  <br/> |Tuto možnost ve výchozím nastavení povolíte, ale pokud je toto nastavení **zapnuto**, může uživatel zkopírovat informace v pracovním souboru do osobního souboru. Pokud je toto nastavení **vypnuto**, nebude uživatel moci kopírovat informace z pracovního účtu do osobní aplikace nebo osobního účtu.  <br/> |
