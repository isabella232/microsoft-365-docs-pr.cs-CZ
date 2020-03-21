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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Přečtěte si, jak vytvořit, upravit nebo odstranit zásady správy aplikací a jak chránit pracovní soubory na zařízeních s Androidem nebo iOS.
ms.openlocfilehash: 0adb103ac3bef72e340c1f5daf54a6b8a184d85c
ms.sourcegitcommit: fce0d5cad32ea60a08ff001b228223284710e2ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/21/2020
ms.locfileid: "42894274"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

![Banner, který https://aka.ms/aboutM365previewpřejděte na .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přejděte do Centra <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>pro správu na adrese . 
    
2. V levém nánosu zvolte **Přidat zásady** \> **Add** **zařízení** \> .
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásad**zvolte Správa aplikací **pro Android** nebo Správa aplikací **pro iOS**podle toho, kterou sadu zásad chcete vytvořit. 
    
5. Rozbalte **Možnost Chránit pracovní soubory při ztrátě nebo odcizení zařízení** a Správa **způsobu, jakým uživatelé přistupují k souborům Office na mobilních zařízeních**. Nakonfigurujte nastavení podle nejraději. **Spravujte, jak budou uživatelé přistupovat k souborům Office na mobilních zařízeních,** je ve výchozím nastavení **vypnutý,** ale doporučujeme je **zapnout** a přijmout výchozí hodnoty. Další informace naleznete v [tématu Available settings](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete používat výchozí skupinu zabezpečení **Všichni uživatelé,** zvolte **Změnit**, \> zvolte skupiny zabezpečení, které tato nastavení **získají Vyberte**.
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="edit-an-app-management-policy"></a>Úprava zásady správy aplikací

1. Na kartě **Zásady** zvolte **Upravit zásady**.
    
2. V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit. 
    
3. Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když změníte hodnotu, automaticky se uloží do zásady.
    
4. Po dokončení zavřete podokno **zásad úpravy.** 
    
## <a name="delete-an-app-management-policy"></a>Odstranění zásady správy aplikací

1. Na stránce **Zásady** zvolte zásadu a **potom odstranit**.
    
2. V podokně **Odstranit zásady** zvolte **Potvrdit,** chcete-li odstranit zásady nebo zásady, které jste zvolili. 
    
## <a name="available-settings"></a>Dostupná nastavení

V následujících tabulkách jsou uvedeny podrobné informace o nastaveních, která jsou k dispozici pro ochranu pracovních souborů na zařízeních, a o nastaveních, která řídí způsob, jakým uživatelé přistupují ke souborům Office ze svých mobilních zařízení.
  
 Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud se zařízení nepoužívá po dobu, kterou zde zadáte, všechny pracovní soubory uložené v zařízení se automaticky odstraní.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **Zapnuto**, je jediným dostupným umístěním pro uložení pracovních souborů OneDrive pro firmy.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. I v případě ztráty nebo odcizení zařízení nikdo nemůže číst údaje vaší společnosti.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **Zapnuto,** musí uživatelé před použitím aplikací Office na svých mobilních zařízeních kromě svého uživatelského jména a hesla poskytnout i jinou formu ověřování.<br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se zobrazí výzva k opětovnému přihlášení.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Nepovolit uživatelům kopírování obsahu z aplikací Office do osobních aplikací  <br/> |Ve výchozím nastavení to povolujeme, ale pokud je nastavení **zapnuto**, může uživatel zkopírovat informace v pracovním souboru do osobního souboru. Pokud je nastavení **vypnuto**, uživatel nebude moci kopírovat informace z pracovního účtu do osobní aplikace nebo osobního účtu.  <br/> |
