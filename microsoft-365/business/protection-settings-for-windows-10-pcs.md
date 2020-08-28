---
title: Úprava nebo vytvoření nastavení ochrany zařízení pro počítače s Windows 10
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Informace o nastaveních dostupných v Microsoft 365 pro firmy pro zabezpečení zařízení s Windows 10.
ms.openlocfilehash: bd992113403c7134fb32bc6cced5bf216843241b
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289149"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Úprava nebo vytvoření nastavení ochrany zařízení pro počítače s Windows 10

Tento článek se týká Microsoft 365 Business Premium.

Po nastavení nastavení ochrany systému Windows na stránce nastavení můžete přidat nové, které platí pro všechny uživatele nebo pro skupinu uživatelů. Můžete také upravit některé z vytvořených.

## <a name="create-protection-settings-for-windows-10-devices"></a>Vytvoření nastavení ochrany pro zařízení s Windows 10

Podívejte se na video o tom, jak zabezpečit zařízení s Windows 10 pomocí Microsoft 365 Business Premium:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Přejděte do centra pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Na levém navigačním panelu zvolte zásady **zařízení** \> **Policies** \> **Add**.
3. V podokně **Přidat zásadu** zadejte název, který je jedinečný. 
4. V části **Typ zásady** zvolte **Konfigurace zařízení s Windows 10**.
5. Rozbalte **Zabezpečit zařízení s Windows 10** \> nakonfigurujte nastavení požadovaným způsobem. Další informace najdete v článku [dostupná nastavení](#available-settings). 
    
    Pokud se chcete vrátit k výchozímu nastavení, použijte odkaz **Obnovit výchozí nastavení**. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
7. Nakonec zvolte **Hotovo**, abyste zásadu uložili a přiřadili ji zařízením. 

## <a name="edit-windows-10-protection-settings"></a>Úprava nastavení ochrany ve Windows 10
 
1. Přejděte do centra pro správu <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Na levém navigačním panelu zvolte zásady **zařízení** \> **Policies** .
1. Zvolte existující zásady zařízení s Windows a pak **Úpravy**.
1. Zvolte **Upravit** vedle nastavení, které chcete změnit, a pak ho **uložte**.

## <a name="available-settings"></a>Dostupná nastavení

Ve výchozím nastavení jsou všechny možnosti **zapnuté**. K dispozici jsou následující nastavení.
  
Další informace najdete v článku [o nastavení funkcí ochrany v Microsoft 365 Premium na nastavení Intune](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Nastavení  <br/> |Popis  <br/> |
|Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender  <br/> |Vyžaduje zapnutí antivirové ochrany v programu Windows Defender, aby bylo možné počítače chránit před nebezpečím spočívajícím v připojení k internetu.  <br/> |
|Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge  <br/> |Zapne nastavení v Edgi, které pomáhá chránit uživatele před škodlivými weby a nebezpečným stahováním.  <br/> |
|Použít pravidla k omezení potenciálních oblastí útoku na zařízení  <br/> |Pokud je omezování potenciálních oblastí útoku zapnuté, pomáhá blokovat akce a aplikace, které obvykle používá malware k napadnutí zařízení. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace získáte v článku o [omezování potenciálních oblastí útoku](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Chránit složky před hrozbami, jako je ransomware  <br/> |Toto nastavení využívá řízený přístup ke složkám a chrání data společnosti před úpravami prostřednictvím podezřelých nebo škodlivých aplikací, jako je ransomware. Těmto typům aplikací se v chráněných složkách nepovolí provést změny. Toto nastavení je dostupné jenom v případě, že je zapnutá Antivirová ochrana v programu Windows Defender. Další informace najdete v tématu [uzamčení složek s řízeným přístupem ke složce](https://docs.microsoft.com/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) .  <br/> |
|Bránit síťovému přístupu k potenciálně škodlivému obsahu na internetu  <br/> |Toto nastavení slouží k blokování odchozích uživatelských připojení k internetovým umístěním s nízkou pověstí, která můžou hostit podvodné podvodné zprávy, zneužít nebo jiný škodlivý obsah. Toto nastavení je dostupné jenom v případě, že je antivirový program Windows Defender nastavený na **zapnuto**. Další informace najdete v tématu [Ochrana sítě](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  <br/> |
|Chránit soubory a složky na počítačích před neoprávněným přístupem pomocí BitLockeru  <br/> |Nástroj BitLocker chrání data šifrováním pevných disků počítače a chrání před expozicí dat při ztrátě nebo odcizení počítače. Další informace najdete v článku [Časté otázky k nástroji BitLocker](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|Povolit uživatelům stahovat aplikace z webu Microsoft Store  <br/> |Umožňuje uživatelům stahovat a instalovat aplikace z webu Microsoft Store. Aplikací může být cokoli, od her až po nástroje na zvyšování produktivity, proto nechte toto nastavení **zapnuté**. Kvůli větší bezpečnosti ho ale můžete vypnout.  <br/> |
|Umožnit uživatelům přístup ke Cortaně  <br/> |Cortana může být velmi užitečná! Cortana může nastavení zapnout nebo vypnout, dát vám pokyny a zkontrolovat, jestli máte čas pro události, takže **Toto nastavení budeme udržovat ve výchozím** nastavení.  <br/> |
|Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft  <br/> |Praktické tipy k Windows mohou uživatelům pomoci zorientovat se v nově vydaných funkcích.  <br/> |
|Automaticky aktualizovat zařízení s Windows 10  <br/> |Zajistí, aby zařízení s Windows 10 automaticky dostávala nejnovější aktualizace.  <br/> |
|Vypnout obrazovku zařízení po nečinnosti  <br/> |Zajistí ochranu dat společnosti, když uživatel zařízení nepoužívá. Uživatel může pracovat na veřejném místě, jako je kavárna, a může si na chvilku odskočit nebo ho někdo vyruší. Informací na zařízení si může všimnout náhodný kolemjdoucí. Toto nastavení určuje, jak dlouho smí být uživatel nečinný, než se obrazovka vypne.  <br/> |
