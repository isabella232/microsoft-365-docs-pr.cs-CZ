---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit nastavení ochrany aplikace Microsoft 365 Business app v zařízeních systému Windows 10.
ms.openlocfilehash: 66e83df19e44419b37bcc1c5678ab13317162dbc
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288589"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Ověření nastavení ochrany zařízení v počítačích se systémem Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Ověření, zda jsou nastaveny zásady zařízení systému Windows 10

Po [nastavení zásad zařízení](protection-settings-for-windows-10-pcs.md)může zásada trvat až několik hodin, než se zásady projeví na zařízeních uživatelů. Můžete potvrdit, že se zásady projevily na různých obrazovkách nastavení systému Windows na zařízeních uživatelů. Vzhledem k tomu, že uživatelé nebudou moci změnit nastavení systému Windows Update a programu Windows Defender Antivirus na svých zařízeních systému Windows 10, bude mnoho těchto možností šedé.
  
1. Přejděte k **Nastavení** \> **aktualizovat &amp; ** \> **Možnosti restartování** **systému Windows Update** \> a potvrďte, že všechna nastavení jsou šedá. 
    
    ![Všechny možnosti restartování jsou zobrazeny šedě.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Přejděte k **Nastavení** \> **aktualizace &amp; zabezpečení** \> v **systému Windows Update** \> **upřesňující možnosti** a potvrďte, že všechna nastavení jsou šedá. 
    
    ![Možnosti rozšířené aktualizace systému Windows jsou všechny zobrazeny šedě.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Přejít na **Nastavení** \> **aktualizace &amp; zabezpečení** \> **Windows Update** \> **upřesňující možnosti** \> **Zvolte způsob doručování aktualizací**.
    
    Potvrďte, že je zobrazena zpráva (červeně), že některá nastavení jsou skryta nebo spravována organizací, a všechny možnosti jsou zobrazeny šedě.
    
    ![Volba způsobu doručování aktualizací indikuje, že nastavení jsou skryta nebo spravována organizací.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Chcete-li otevřít Centrum zabezpečení programu Windows Defender, přejděte k **Nastavení** \> ** &amp; aktualizace zabezpečení** \> **programu Windows Defender** \> klepněte na možnost **otevřít** \> ** &amp; vlákno programu Centrum zabezpečení Windows Defender ochrany** \> **nastavení &amp; ochrany proti virům**. 
    
5. Ověřte, zda jsou všechny možnosti zobrazeny šedě. 
    
    ![Nastavení ochrany proti virům a ohrožení je šedé.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Příbuzná témata

[Dokumentace a zdroje informací o Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Začínáme s Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Správa Microsoft 365 Business](manage.md)
  
[Nastavení konfigurací zařízení pro počítače s Windows 10](protection-settings-for-windows-10-pcs.md)
  

