---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit nastavení ochrany Microsoft 365 Business aplikace v zařízení Windows 10.
ms.openlocfilehash: 5ab91d65fa7bd40ebc118df217c9711b7bbfe7a4
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286701"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Ověřit nastavení ochrany zařízení Windows 10 počítačů

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověřte, zda jsou nastaveny zásady Windows 10 zařízení

Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat několik hodin zásady se projeví na zařízeních uživatelů. Můžete ověřit, že zásady ručitelského pohledem na různé obrazovky nastavení systému Windows na zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení služby Windows Update a Windows Defender Antivirus na jejich zařízeních Windows 10, mnoho z těchto možností bude šedé.
  
1. Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Možnosti restartování** a potvrďte, že jsou všechna nastavení šedě. 
    
    ![Všechny možnosti restartování jsou označeny šedou barvou.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Rozšířené možnosti** a potvrďte, že jsou všechna nastavení šedě. 
    
    ![Možnosti aktualizace Windows Advanced se všechny zobrazí šedě.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **Rozšířené možnosti** \> **zvolit způsob doručování aktualizací**.
    
    Potvrďte, že uvidíte zprávu (červeně), některá nastavení jsou skrytá nebo spravovány v organizaci a všech možností se zobrazí šedě.
    
    ![Zvolit způsob doručování aktualizací stránky označuje nastavení skrytých nebo spravuje vaše organizace.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Chcete-li otevřít Centrum zabezpečení systému Windows Defender, přejděte na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Program Windows Defender** \> klepněte na tlačítko **Spustit Centrum zabezpečení v aplikaci Windows Defender** \> **viru &amp; vlákna Ochrana** \> **viru &amp; ochrany proti novým ohrožením ochrany nastavení**. 
    
5. Ověřte, že všechny možnosti jsou označeny šedou barvou. 
    
    ![Nastavení ochrany proti virům a ohrožením jsou označeny šedou barvou.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Příbuzná témata

[Dokumentace a zdroje informací o Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Začínáme s Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Správa Microsoft 365 Business](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  

