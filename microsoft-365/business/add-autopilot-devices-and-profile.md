---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Zjistěte, jak pomocí Windows AutoPilota nastavit nová zařízení s Windows 10 pro vaši firmu, aby byla připravená k použití pro zaměstnance.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913496"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

Pomocí Windows AutoPilota můžete nastavit nová zařízení **s** Windows 10 pro vaši firmu, aby byla připravená k použití, když je dáte svým zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která ještě nevyužíla prostředí Windows
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)

Pokud jste skupiny zařízení nebo profily ještě nevytáčili, nejlepší způsob, jak začít, je použití podrobného průvodce. Můžete také [přidávat zařízení a](create-and-edit-autopilot-devices.md) [přiřazovat jim](create-and-edit-autopilot-profiles.md) profily bez použití průvodce. 
  
1. Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. V levém navigačním podokně zvolte **Zařízení** \> **AutoPilota**.

    ![V Centru pro správu vyberte zařízení a pak AutoPilot.](../media/AutoPilot.png)
  
2. Na stránce **AutoPilot** klikněte nebo klepněte na **Úvodní příručka**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na stránce **Upload .csv file with list of devices** (Nahrát soubor .csv se seznamem zařízení) přejděte do umístění, kde máte připravené soubory . Soubor CSV a pak **Otevřít** \> **další**. Soubor musí mít tři záhlaví:
    
    - Sloupec A: Sériové číslo zařízení
    
    - Sloupec B: ID produktu Windows
    
    - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete ke generování souboru CSV použít skript [Get-WindowsAutoPilotInfo PowerShellu.](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](../admin/misc/device-list.md). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
> [!NOTE]
> Tento skript používá službu WMI k načtení vlastností potřebných k registraci zařízení u Windows Autopilota. Všimněte si, že je normální, že výsledný soubor CSV neshromažďuje hodnotu ID produktu Windows (PKID), protože to není nutné k registraci zařízení a PKID je NULL ve výstupním souboru CSV je úplně v pořádku. Vyplní se jenom sériové číslo a hardwarová hodnota hash.
    
4. Na **stránce Přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový. Pokud ho ještě nemáte, zobrazí se výzva k jeho vytvoření. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou povinné a automaticky se nastavují. Výchozí funkce:
    
    - Přeskočte registraci Cortany, OneDrivu a OEM.
    
    - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
    - Připojte zařízení k účtům Azure Active Directory a automaticky je zaregistrujte, aby je spravoval Microsoft 365 Business Premium.
    
    Další informace najdete v tématu [O nastavení profilu AutoPilota](autopilot-profile-settings.md). 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. **Hotovo znamená,** že profil, který jste vytvořili (nebo zvolili) se použije u skupiny zařízení, kterou jste vytvořili tak, že nahrajete seznam zařízení. Nastavení se projeví, když se uživatelé zařízení přihlásí příště. Zvolte **Zavřít**.
