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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Přečtěte si, jak ověřit nastavení ochrany aplikací Microsoft 365 Business na zařízeních s Windows 10.
ms.openlocfilehash: 6573519ee2fe2d1eb82545755fa98b8c018e08ff
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594989"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany aplikací na počítačích s Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních

Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů. Pokud jste **zapnuli** možnost **Zabránit uživatelům v kopírování firemních dat do osobních souborů a vynutit je ukládat pracovní soubory do nastavení OneDrivu pro firmy** pro zařízení vlastněná společností, můžete to zkontrolovat na zařízení uživatele poté, co se připojí k Azure AD a přihlásí se. 
  
 **Ověření nastavení připojení**
  
1. Až se přihlásíte pomocí přihlašovacích údajů Microsoft 365 Business a připojíte se k Azure AD, jak je popsáno v části [Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business](set-up-windows-devices.md), přejděte na **Nastavení systému Windows** \> **Účty** \> **Přístup do práce nebo do školy**. Zvolte **Připojeno k \<název tenanta\> Azure AD** a pak zvolte **Informace**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Na stránce **Spravovaný** \<podle názvu\> klienta se zobrazí **informace o připojení,** které obsahují adresu serveru pro **správu,** jako je adresa zobrazená na následujícím obrázku. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Ověření, že nelze vložit firemní data do nespravované aplikace.**
  
1. Otevřete Outlook 2016 nainstalovaný přes Microsoft 365 Business.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních

 **Ověření nastavení připojení**
  
1. Na osobním zařízení s Windows 10, kde jste přihlášeni jako místní uživatel, přejděte do **nastavení systému Windows**a klikněte nebo klepněte na Položky Přístup k **účtům** \> **do práce nebo školy**.
    
2. V části **Přístup do práce nebo do školy** zvolte **Připojit**.
    
3. Zadejte přihlašovací údaje Microsoft 365 Business do dialogu **Nastavení pracovního nebo školního účtu** \> **Přihlásit se**.
    
4. Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.
    
    ![Klikněte nebo klepněte na Informace v dialogovém okně Pracovní nebo školní účet.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Na stránce **Práce nebo Škola aplikace Access** se zobrazí informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku, a obsahuje slova *wip* a *mam* uvnitř. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Ověření, že nelze vložit firemní data do nespravované aplikace.**
  
1. Otevřete Outlook 2016 a přidejte svůj účet Microsoft 365 Business (pokud je to potřeba) a přihlaste se přihlašovacími údaji Microsoft 365 Business.
    
2. Otevřete e-mail a zkopírujte z něj nějaký obsah.
    
    Otevřete Poznámkový blok a pokuste se do něho obsah vložit.
    
    Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Stejný obsah ale můžete vložit do Wordu 2016.
    

