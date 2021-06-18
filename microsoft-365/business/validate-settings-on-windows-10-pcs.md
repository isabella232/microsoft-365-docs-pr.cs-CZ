---
title: Ověření nastavení ochrany aplikací pro Windows 10 počítače
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
description: Zjistěte, jak ověřit, Microsoft 365 nastavení ochrany aplikací pro firmy na zařízeních Windows 10 uživatelů.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925253"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Ověření nastavení ochrany zařízení pro Windows 10 počítače

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověření, Windows 10 jsou nastavené zásady zařízení

Po nastavení [zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásada projeví na zařízeních uživatelů. Můžete potvrdit, že se zásady projeví, když se podíváme na Windows Nastavení obrazovkách na zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moct změnit nastavení aktualizace Windows a Antivirová ochrana v programu Windows Defender na svých Windows 10 zařízeních, zobrazí se řada možností šedě.
  
1. Přejděte na **Nastavení** Aktualizace zabezpečení Windows Možnosti restartování aktualizace a potvrďte, že jsou všechna \> **&amp;** \>  \>  nastavení šedá. 
    
    ![Všechny možnosti restartování jsou šedé.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte na **Nastavení** Aktualizace zabezpečení Windows Upřesnit možnosti aktualizace a potvrďte, že jsou všechna \> **&amp;** \>  \>  nastavení šedá. 
    
    ![Windows Rozšířené možnosti aktualizací jsou všechny šedé.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejděte na **Nastavení** Aktualizace \> **&amp; zabezpečení** Windows Upřesnit možnosti Zvolte \>  \>  \> **způsob doručení aktualizací.**
    
    Potvrďte, že vidíte zprávu (červeně), že některá nastavení jsou skrytá nebo spravovaná vaší organizací a všechny možnosti jsou šedé.
    
    ![Výběr způsobu doručení aktualizací označuje, že nastavení je ve vaší organizaci skryté nebo spravované.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Pokud chcete otevřít Windows Defender Security Center, přejděte na **Nastavení** \> **Aktualizace &amp; zabezpečení** \> **Windows Defender** na Otevřít \> Windows Defender Security **Center** \> **Ochrana &amp;** \> **&amp;** před viry Nastavení ochrany před viry . 
    
5. Ověřte, jestli jsou všechny možnosti šedé. 
    
    ![Nastavení ochrany před viry a hrozbou jsou šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Související témata

[Microsoft 365 pro obchodní dokumentaci a zdroje informací](./index.yml)
  
[Začínáme s Microsoft 365 pro firmy](microsoft-365-business-overview.md)
  
[Správa Microsoft 365 pro firmy](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
