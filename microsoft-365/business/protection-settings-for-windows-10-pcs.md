---
title: Nastavení ochrany zařízení pro počítače s Windows 10
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Informace o výchozím nastavení a další nastavení, které jsou k dispozici v Microsoft Business 365 k zabezpečení zařízení Windows 10.
ms.openlocfilehash: 095aa2c2f32c3e7b5a5a4e560ea4bc7124d7146e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074504"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Nastavení ochrany zařízení pro počítače s Windows 10

## <a name="secure-windows-10-devices"></a>Zabezpečení zařízení s Windows 10

Podívejte se na video o tom, jak zabezpečit zařízení s Windows 10 s Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. SGo centru pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Na levá navigace zvolte **zařízení** \> **zásad** \> **Přidat**.
  
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
    
4. V části **Typ zásady** zvolte **Konfigurace zařízení s Windows 10**.
    
5. Rozbalte **Zabezpečit zařízení s Windows 10** \> nakonfigurujte nastavení požadovaným způsobem. Další informace najdete v části [Dostupná nastavení](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
    
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 
    
## <a name="available-settings"></a>Dostupná nastavení

Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení.
  
Další informace najdete v tématu o [mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender  <br/> |Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.  <br/> |
|Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge  <br/> |Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.  <br/> |
|Použít pravidla k omezení potenciálních oblastí útoku na zařízení  <br/> |Pokud je omezování potenciálních oblastí útoku zapnuté, pomáhá blokovat akce a aplikace, které obvykle používá malware k napadnutí zařízení. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [omezování potenciálních oblastí útoku](https://go.microsoft.com/fwlink/?linkid=870417).  <br/> |
|Chránit složky před hrozbami, jako je ransomware  <br/> |Toto nastavení využívá řízený přístup ke složkám a chrání data společnosti před úpravami prostřednictvím podezřelých nebo škodlivých aplikací, jako je ransomware. Těmto typům aplikací se v chráněných složkách nepovolí provést změny. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [ochraně složek pomocí řízeného přístupu](https://go.microsoft.com/fwlink/?linkid=870418).  <br/> |
|Bránit síťovému přístupu k potenciálně škodlivému obsahu na internetu  <br/> |Pomocí tohoto nastavení můžete blokovat odchozí uživatelská připojení k umístěním na internetu s nízkou reputací, která můžou být hostiteli podvodů, útoků phishing, zneužití nebo jiného škodlivého obsahu. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [ochraně sítě](https://go.microsoft.com/fwlink/?linkid=870419).  <br/> |
|Chránit soubory a složky na počítačích před neoprávněným přístupem pomocí BitLockeru  <br/> |BitLocker chrání data tím, že šifruje pevné disky počítačů. Brání tak vyzrazení dat v případě ztráty nebo odcizení počítačů. Další informace najdete v [častých otázkách k BitLockeru](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|Povolit uživatelům stahovat aplikace z webu Microsoft Store  <br/> |Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  <br/> |
|Umožnit uživatelům přístup ke Cortaně  <br/> |Cortana může být velice užitečná. Může vám zapínat nebo vypínat nastavení, dávat vám pokyny a postarat se o to, abyste chodili včas na schůzky. Proto jsme nastavení nechali implicitně **zapnuté**.  <br/> |
|Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft  <br/> |Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.  <br/> |
|Automaticky aktualizovat zařízení s Windows 10  <br/> |Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.  <br/> |
|Vypnout obrazovku zařízení po nečinnosti  <br/> |Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.  <br/> |
   
  

