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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Přečtěte si, jak ověřit, že nastavení ochrany aplikací Microsoft 365 Business se projevilo na zařízeních uživatelů s Windows 10.
ms.openlocfilehash: 1b661b41a8042e81f653463cbd32fc6bf6428b53
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/06/2020
ms.locfileid: "42549951"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany zařízení v počítačích s Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověření nastavené zásady zařízení s Windows 10

Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může trvat až několik hodin, než se zásady projeví na zařízeních uživatelů. Můžete potvrdit, že zásady se projevily, a to tak, že se podíváte na různé obrazovky Nastavení systému Windows na zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moci na svých zařízeních se systémem Windows 10 upravovat nastavení programu Windows Update a programu Windows Defender, bude mnoho možností zobrazeno šedě.
  
1. Přejděte na **možnosti** **zabezpečení aktualizace &amp; ** \> **Nastavení** \> **Windows Update** \> Restart a zkontrolujte, zda jsou všechna nastavení zobrazena šedě. 
    
    ![Všechny možnosti restartování jsou šedě.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte na **možnosti &amp; zabezpečení** \> aktualizace **nastavení** \> **služby Windows Update** \> **Upřesňující možnosti** a potvrďte, že všechna nastavení jsou zašedlá. 
    
    ![Možnosti rozšířených aktualizací systému Windows jsou všechny zobrazeny šedě.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejděte na **zabezpečení aktualizace** \> \> \> \> **** ** &amp; ** nastavení **Možnosti Windows Update** **Upřesnit způsob doručení aktualizací**.
    
    Zkontrolujte, zda se zobrazí zpráva (červeně), že některá nastavení jsou skryta nebo spravována vaší organizací, a že všechny možnosti jsou zobrazeny šedě.
    
    ![Zvolte způsob doručení aktualizací, protože nastavení je skryto nebo spravuje vaše organizace.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte na **položku** \> Zabezpečení \> **aktualizace &amp; ** nastavení **programu Windows Defender** \> klepněte na tlačítko **Otevřít program Windows Defender Security Center** \> **Ochrana &amp; vláken Ochrana vláken Ochrana** \> ** &amp; před virovou ochranou proti ohrožení mantinela**. 
    
5. Ověřte, zda jsou všechny možnosti zobrazeny šedě. 
    
    ![Nastavení ochrany proti virům a hrozbám jsou zobrazena šedě.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Příbuzná témata

[Dokumentace a zdroje informací o Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Začínáme s Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Správa Microsoft 365 Business](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  

