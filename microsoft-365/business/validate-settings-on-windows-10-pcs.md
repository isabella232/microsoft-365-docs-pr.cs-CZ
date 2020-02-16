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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Přečtěte si, jak ověřit nastavení ochrany aplikací Microsoft 365 Business na zařízeních s Windows 10.
ms.openlocfilehash: 1762382aec00a80e006cf38b66c28d02c0c25989
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42056637"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany zařízení v počítačích s Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověření nastavení zásad zařízení s Windows 10

Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásady projeví na zařízeních uživatelů. Zásady se projevily na různých obrazovkách nastavení systému Windows v zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení Windows Update a Windows Defender Antivirus na svých zařízeních s Windows 10, mnoho možností bude šedě.
  
1. Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> Restart **možnosti** a zkontrolujte, zda všechna nastavení jsou šedě. 
    
    ![Všechny možnosti restartování jsou šedě.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Update** \> **Upřesnit možnosti** a zkontrolujte, zda všechna nastavení jsou šedě. 
    
    ![Možnosti aktualizací rozšířené systému Windows jsou zobrazeny šedě.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Rozšířené možnosti** \> **služby Windows Update** \> **Zvolte způsob doručení aktualizací**.
    
    Zkontrolujte, zda se zobrazí zpráva (červeně), že některá nastavení jsou skryta nebo spravována vaší organizací a všechny možnosti jsou šedě.
    
    ![Zvolte, jak jsou aktualizace doručovány, na stránce indikuje, že nastavení jsou skrytá nebo spravovaná vaší organizací.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte **na** \> **nastavení zabezpečení aktualizace &amp; ** \> **Windows Defender,** \> klepněte na příkaz Otevřít program Windows **Defender Security Center** \> **Anti &amp; thread protection** \> **Anti-hrozeb &amp; **. 
    
5. Ověřte, zda jsou všechny možnosti šedě. 
    
    ![Nastavení ochrany proti virům a hrozbám je šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Související témata

[Dokumentace a zdroje informací o Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Začínáme s Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Správa Microsoft 365 Business](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  

