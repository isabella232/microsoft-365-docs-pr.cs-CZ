---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Ověřte Microsoft 365 Business Premium nastavení ochrany aplikací na Windows 10 zařízeních a ověřte, že uživatelé nemohou kopírovat data společnosti do osobních souborů nebo nespravovaných aplikací.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861694"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany aplikací na počítačích s Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních

Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů. Pokud jste  zapnuli nastavení Zabránit uživatelům v kopírování firemních dat do osobních souborů OneDrive pro firmy přinutili je ukládat pracovní soubory do zařízení vlastněných společností, můžete to zkontrolovat na zařízení uživatele po připojení k Azure AD **OneDrive pro firmy** přihlášení. 
  
 **Ověření nastavení připojení**
  
1. Po přihlášení pomocí přihlašovacích údajů Microsoft 365 Business Premium připojte se k Azure AD, jak je popsáno v článku  Nastavení zařízení Windows pro uživatele [Microsoft 365 Business Premium](set-up-windows-devices.md), přejděte na Windows Nastavení Přístup k účtům v práci nebo ve \>  \> **škole.** Zvolte **Připojeno \<tenant name\> k Azure AD** a pak zvolte **Informace**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stránce **Spravovaný** podle se zobrazí informace o připojení, které obsahují adresu serveru pro správu, jak je \<tenant name\> znázorněno na následujícím obrázku.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Ověřte, že nemůžete vložit data společnosti do nespravovaná aplikace.**
  
1. Otevřete Outlook 2016, který jste nainstalovali Microsoft 365 Business Premium.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chybová zpráva, že aplikace nemůže získat přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních

 **Ověření nastavení připojení**
  
1. Na osobním Windows 10, na kterém jste přihlášení jako místní uživatel, přejděte na **Windows Nastavení** a klikněte nebo klepněte na **Účty** Access v práci nebo ve \> **škole**.
    
2. V části **Přístup do práce nebo do školy** zvolte **Připojit**.
    
3. Zadejte Microsoft 365 Business Premium přihlašovací údaje do **dialogového** okna Nastavení pracovního nebo školního \> **účtu Přihlásit se**.
    
4. Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.
    
    ![V dialogovém okně Pracovní nebo školní účet klikněte nebo klepněte na Informace.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na pracovní nebo školní stránce **Accessu** uvidíte informace o připojení, které obsahují adresu serveru pro správu, jako je adresa uvedená na následujícím obrázku, **a** obsahuje slova *wip* a *mam* uvnitř.  
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Ověřte, že nemůžete vložit data společnosti do nespravovaná aplikace.**
  
1. Otevřete Outlook 2016 a v případě potřeby přidejte svůj Microsoft 365 Business Premium účet a přihlaste se pomocí Microsoft 365 Business Premium přihlašovacích údajů.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chybová zpráva, že aplikace nemůže získat přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    

