---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Zjistěte, jak Windows autopilota k nastavení nových Windows 10 zařízení pro vaši firmu, aby byla připravená k použití pro zaměstnance.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393433"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

Pomocí Windows AutoPilot můžete nastavit nová **Windows 10** zařízení pro vaši firmu, aby byla připravená k použití, když je dáte svým zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musí splňovat tyto požadavky:
  
- Windows 10 verze 1703 nebo novější
    
- Nová zařízení, která ještě Windows prostředí
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

Pokud jste skupiny zařízení nebo profily ještě nevytáčili, nejlepší způsob, jak začít, je použití podrobného průvodce. Můžete také [přidávat zařízení a](create-and-edit-autopilot-devices.md) [přiřazovat jim](create-and-edit-autopilot-profiles.md) profily bez použití průvodce. 
  
1. Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. V levém navigačním podokně zvolte **Zařízení** \> **AutoPilota**.

    ![V Centru pro správu vyberte zařízení a pak AutoPilot.](../media/AutoPilot.png)
  
2. Na stránce **AutoPilot** klikněte nebo klepněte na **Úvodní příručka**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na Upload .csv **souboru se seznamem** zařízení přejděte do umístění, kde máte připravený soubor .CSV a pak **otevřít** \> **další.** Soubor musí mít tři záhlaví:
    
    - Sloupec A: Sériové číslo zařízení
    
    - Sloupec B: ID produktu Windows
    
    - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete ke generování souboru CSV použít skript [Get-WindowsAutoPilotInfo PowerShellu.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](../admin/misc/device-list.md). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
> [!NOTE]
> Tento skript používá službu WMI k načtení vlastností potřebných k registraci zařízení u Windows Autopilota. Všimněte si, že je normální, že výsledný soubor CSV neshromažďuje hodnotu ID produktu Windows (PKID), protože to není nutné k registraci zařízení a PKID je NULL ve výstupním souboru CSV je zcela v pořádku. Vyplní se jenom sériové číslo a hardwarová hodnota hash.
    
4. Na **stránce Přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový. Pokud ho ještě nemáte, zobrazí se výzva k jeho vytvoření. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou povinné a automaticky se nastavují. Výchozí funkce:
    
    - Přeskočte Cortana, OneDrive a registraci OEM.
    
    - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
    - Připojení na zařízeních Azure Active Directory účty a automaticky je zaregistrujte, aby je Microsoft 365 Business Premium.
    
    Další informace najdete v tématu [O nastavení profilu AutoPilota](autopilot-profile-settings.md). 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. **Hotovo znamená,** že profil, který jste vytvořili (nebo zvolili) se použije u skupiny zařízení, kterou jste vytvořili tak, že nahrajete seznam zařízení. Nastavení se projeví, když se uživatelé zařízení přihlásí příště. Zvolte **Zavřít**.

## <a name="related-content"></a>Související obsah

[Nastavení profilu AutoPilota](autopilot-profile-settings.md) (článek)\
[Možnosti ochrany vašich zařízení a dat aplikací](../admin/devices/choose-device-security.md) (článek)
