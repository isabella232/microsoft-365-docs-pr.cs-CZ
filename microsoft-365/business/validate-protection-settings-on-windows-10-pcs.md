---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
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
description: Ověřte nastavení ochrany aplikací Microsoft 365 Business Premium na zařízeních s Windows 10 a ověřte, zda uživatelé nemohou kopírovat firemní data do osobních souborů nebo do nespravovaných aplikací.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403384"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany aplikací na počítačích s Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních

Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů. Pokud jste **zapnuli možnost** **Zabránit uživatelům v kopírování firemních dat do osobních souborů a vynutit jim uložení pracovních souborů do nastavení OneDrivu pro firmy** pro zařízení vlastněná společností, můžete to zkontrolovat na zařízení uživatele po připojení k Azure AD a přihlášení. 
  
 **Ověření nastavení připojení**
  
1. Po přihlášení pomocí přihlašovacích údajů k Microsoft 365 Business Premium a připojení k Azure AD, jak je popsáno v [části Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md), přejděte na pracovní nebo školní téma Windows **Settings** \> **Accounts** \> **Access**. Zvolte **Připojeno k \<tenant name\> Azure AD**a pak zvolte **Informace**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stránce **Správa podle** \<tenant name\> uvidíte informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Ověření, že nelze vložit firemní data do nespravované aplikace**
  
1. Otevřete Outlook 2016, který nainstaloval Microsoft 365 Business Premium.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních

 **Ověření nastavení připojení**
  
1. Na osobním zařízení s Windows 10, kde jste přihlášení jako místní uživatel, přejděte do **Nastavení Windows**a klikněte nebo klepněte na Přístup **k** \> **účtům v práci nebo ve škole**.
    
2. V části **Přístup do práce nebo do školy** zvolte **Připojit**.
    
3. Zadejte své přihlašovací údaje microsoft 365 Business Premium do **dialogového okna Nastavit pracovní nebo školní účet** \> **Přihlášení**.
    
4. Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.
    
    ![Klikněte nebo klepněte na Informace v dialogovém okně Pracovní nebo školní účet.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stránce **Práce nebo škola aplikace Access** se zobrazí informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku, a uvnitř obsahuje slova *stírací* a *mam.* 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Ověření, že nelze vložit firemní data do nespravované aplikace**
  
1. Otevřete Outlook 2016 a v případě potřeby přidejte svůj účet Microsoft 365 Business Premium a přihlaste se pomocí přihlašovacích údajů microsoft 365 Business Premium.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    

