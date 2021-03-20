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
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit, že se nastavení ochrany aplikací Microsoft 365 pro firmy projeví na zařízeních s Windows 10 vašich uživatelů.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912408"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany zařízení na počítačích s Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověření nastavení zásad zařízení s Windows 10

Po nastavení [zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásada projeví na zařízeních uživatelů. Můžete potvrdit, že se zásady projeví, když se podíváme na různé obrazovky nastavení Windows na zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moct na svých zařízeních s Windows 10 upravovat nastavení Antivirové ochrany v programu Windows Update a Windows Defender, mnoho možností se zobrazí šedě.
  
1. Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **Možnosti restartování** a potvrďte, že jsou všechna nastavení šedá. 
    
    ![Všechny možnosti restartování jsou šedé.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte na **Nastavení Aktualizace** zabezpečení Windows Update – upřesnit možnosti a ověřte, že všechna nastavení \> **&amp;** jsou \>  \>  šedá. 
    
    ![Možnosti upřesňujících aktualizací systému Windows jsou všechny šedé.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **– upřesnit možnosti** \> **Zvolte způsob doručení aktualizací.**
    
    Potvrďte, že vidíte zprávu (červeně), že některá nastavení jsou skrytá nebo spravovaná vaší organizací a všechny možnosti jsou šedé.
    
    ![Výběr způsobu doručení aktualizací označuje, že nastavení je ve vaší organizaci skryté nebo spravované.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Pokud chcete otevřít Centrum zabezpečení  v programu Windows Defender, přejděte na Nastavení Aktualizace zabezpečení Windows Defenderu klikněte na Otevřít Centrum zabezpečení v programu Windows Defender Ochrana proti virům ochrana před vlákny \> **&amp;** Nastavení \>  \> ochrany  \> **&amp;** \> **&amp; před viry**. 
    
5. Ověřte, jestli jsou všechny možnosti šedé. 
    
    ![Nastavení ochrany před viry a hrozbou jsou šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Související témata

[Dokumentace a materiály k Microsoftu 365 pro firmy](./index.yml)
  
[Začínáme s Microsoft 365 pro firmy](microsoft-365-business-overview.md)
  
[Správa Microsoftu 365 pro firmy](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
