---
title: Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Zjistěte, jak vytvářet, upravovat nebo odstraňovat zásady správy aplikací a jak chránit pracovní soubory na zařízeních s Androidem nebo iOS.
ms.openlocfilehash: 0f1e509de728654eef543449741a89f7f04001bb46ee3f06fe9b96038650eb6f
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896341"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem

Tento článek se týká Microsoft 365 Business Premium.

## <a name="create-an-app-management-policy"></a>Vytvoření zásady správy aplikací

1. Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. V levém navigačním panelu zvolte **Zásady** \> **zařízení –** \> **přidat**.
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V **části Typ zásad** zvolte Správa aplikací pro **Android** nebo Správa aplikací pro **iOS** podle toho, kterou sadu zásad chcete vytvořit. 
    
5. Rozbalte **Zamknout pracovní soubory při** ztrátě nebo odcizení zařízení a Správa přístupu uživatelů **Office souborů na mobilních zařízeních**. Nakonfigurujte nastavení podle toho, jak chcete. **Ve výchozím nastavení můžete Office** přístup k  souborům na mobilních zařízeních  vypnutý, ale doporučujeme ho zapnout a přijmout výchozí hodnoty. Další informace najdete v tématu [Dostupná nastavení](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni** uživatelé, zvolte **Změnit**, zvolte skupiny zabezpečení, které mají tato nastavení \> **vybrat.**
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="edit-an-app-management-policy"></a>Úprava zásady správy aplikací

1. Na kartě **Zásady** zvolte **Upravit zásadu**.
    
2. V podokně **Upravit zásadu** zvolte zásadu, kterou chcete změnit. 
    
3. Zvolte **Upravit** vedle každého nastavení, abyste upravili hodnoty dané zásady. Když změníte hodnotu, automaticky se uloží do zásady.
    
4. Až skončíte, zavřete **podokno Upravit zásadu.** 
    
## <a name="delete-an-app-management-policy"></a>Odstranění zásady správy aplikací

1. Na stránce **Zásady** zvolte zásadu a potom **odstranit**.
    
2. V podokně **Odstranit zásadu** zvolte **Potvrdit a** odstraňte tak zásady, které jste zvolili. 
    
## <a name="available-settings"></a>Dostupná nastavení

Následující tabulky obsahují podrobné informace o dostupných nastaveních pro ochranu pracovních souborů na zařízeních a nastavení, která řídí přístup uživatelů Office soubory ze svých mobilních zařízení.
  
 Další informace najdete v tématu Jak se funkce ochrany v [Microsoft 365 Business Premium namapovat na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Nastavení chránící pracovní soubory

Pokud se zařízení uživatele ztratí nebo je odcizeno, jsou k dispozici pro ochranu pracovních souborů následující nastavení:


|Nastavení  <br/> |Popis  <br/> |
|:-----|:-----|
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Pokud se zařízení po dobu, po kterou tady zadáte, nepoužít, odstraní se všechny pracovní soubory uložené na zařízení automaticky.  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> |Pokud je toto nastavení **na ,** je pro pracovní soubory k dispozici pouze OneDrive pro firmy.  <br/> |
|Šifrovat pracovní soubory  <br/> |Toto nastavení nechejte **zapnuté**, aby byly pracovní soubory chráněné šifrováním. I když dojde ke ztrátě nebo odcizení zařízení, nikdo nemůže číst data vaší společnosti.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Nastavení spravující přístup uživatelů k souborům Office na mobilních zařízeních

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office:


|Nastavení  <br/> |Popis  <br/> |
|:-----|:-----|
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **Nastaveno:** Uživatelé musí kromě uživatelského jména a hesla zadat i jinou formu ověřování, aby mohli na svých mobilních zařízeních používat Office aplikace.<br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určuje, jak dlouho může být uživatel nečinný, než se zobrazí výzva k opětovnému přihlášení.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Zruční uživatelé mohou mít zařízení s jailbreakem nebo rootem. To znamená, že takový uživatel může upravovat operační systém, což může zařízení učinit náchylnější vůči malwaru. Když je nastavení **zapnuté**, jsou tato zařízení blokovaná.  <br/> |
|Nepovolovat uživatelům kopírování obsahu z Office aplikací do osobních aplikací  <br/> |Ve výchozím nastavení to povolíme, ale pokud je nastavení **Na**, může uživatel zkopírovat informace v pracovním souboru do osobního souboru. Pokud je nastavení **vypnuté,** nebude uživatel moci zkopírovat informace z pracovního účtu do osobní aplikace nebo osobního účtu.  <br/> |
