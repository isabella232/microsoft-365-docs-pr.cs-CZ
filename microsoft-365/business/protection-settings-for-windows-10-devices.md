---
title: Nastavení ochrany aplikací pro zařízení s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Naučte se vytvořit zásadu správy aplikací a ochrany pracovních souborů v zařízení Windows 10.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982821"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Nastavení ochrany aplikací pro zařízení s Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>Vytvoření zásady správy aplikací pro Windows 10

Pokud mají uživatelé osobní zařízení s Windows 10, na kterých dělají pracovní úkoly, můžete chránit vaše data i na těchto zařízeních.
  
1. Přihlaste se k [Microsoft 365 Business](https://portal.office.com) pod uživatelským jménem a heslem globálního správce. Vyberte dlaždici **Správce** a přejděte do Centra pro správu. 
    
2. Na kartě **Zásady zařízení** portálu pro správce zvolte **Přidat zásadu**.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásady** zvolte **Správa aplikací pro Windows 10**.
    
5. Pod ** typ zařízení **, zvolte **osobní** nebo **Ve vlastnictví společnosti**.
    
6. Možnost **Šifrovat pracovní soubory** je zapnutá automaticky. 
    
7. Pokud nechcete, aby uživatelé ukládali pracovní soubory na své počítače, **zapněte** možnost **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**. 
    
8. Rozbalte položku **Spravovat přístup uživatelů k souborů sady Office na zařízení** \> nastavit, jakým způsobem. **Spravovat přístup uživatelů k zařízení Office na mobilních zařízeních** je **Vypnuto** ve výchozím nastavení, ale je vhodné **jej zapnout** a přijměte výchozí hodnoty. Další informace naleznete v tématu [nastavení k dispozici](protection-settings-for-windows-10-devices.md#bkmk_settings) . 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
9. Rozbalte možnost **Obnovit data na zařízeních s Windows**, kterou vám doporučujeme **Zapnout**.
    
    Než budete moct přejít do umístění certifikátu agenta obnovování dat, musíte nějaký nejprve vytvořit. Pokyny najdete v článku o [vytvoření a ověření certifikátu agenta obnovování dat (DRA) systému souborů EFS](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Ve výchozím nastavení jsou pracovní soubory šifrované pomocí tajného klíče, který je uložený v zařízení a přidružený k profilu uživatele. Soubor může otevřít a dešifrovat jenom uživatel. Pokud ovšem dojde ke ztrátě zařízení nebo odebrání uživatele, soubor může zůstat zašifrovaný. Může ho dešifrovat správce pomocí certifikátu agenta obnovování dat (DRA).
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Pokud chcete přidat další domény nebo umístění SharePointu Online, abyste se ujistili, že soubory ve všech uvedených aplikacích budou chráněné, rozbalte možnost **Chránit další umístění v síti a cloudu**. Pokud potřebujete zadat do jednoho z polí více než jednu položku, oddělte tyto položky středníkem (;). 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. V dalším kroku rozhodněte, **pro koho tato nastavení platí**. Pokud nechcete použít výchozí skupinu zabezpečení **Všichni uživatelé**, zvolte **Změnit** a vyberte skupinu zabezpečení, pro kterou se tato nastavení použijí \> **Vybrat**.
    
12. Volbou **Přidat** nakonec zásadu uložíte a přiřadíte ji zařízením. 
    
## <a name="available-settings"></a>Dostupná nastavení

Následující nastavení slouží ke správě přístupu uživatelů k pracovním souborům Office.
  
Další informace najdete v článku o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md).
  
|**Nastavení**|**Popis**|
|:-----|:-----|
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> |Pokud je toto nastavení **Zapnuté**, uživatelé musí kromě svého uživatelského jména a hesla poskytnout i jinou formu ověření, než budou moct aplikace Office na svém mobilním zařízení používat.  <br/> |
|Resetovat PIN po tomto počtu neúspěšných přihlášení  <br/> |Aby se zabránilo náhodnému uhodnutí PINu neoprávněným uživatelem, resetuje se PIN po vámi určeném počtu špatných pokusů.  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu  <br/> |Toto nastavení určí dobu, po kterou může být uživatel nečinný, než se bude muset znovu přihlásit.  <br/> |
   

