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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Přečtěte si, jak pomocí automatického pilotního projektu Windows nastavit nová zařízení s Windows 10 pro vaši firmu.
ms.openlocfilehash: e5774b1e2079a5249e0f6e9e7142de19268253b5
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068519"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

Pomocí aplikace Windows AutoPilot můžete nastavit **nová** zařízení s Windows 10 pro vaši firmu, aby byla připravena k použití, když je dáte svým zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která neprošla systémem Windows, jsou v rámečku
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Pokud jste ještě nevytvořili skupiny zařízení nebo profily, nejlepší způsob, jak začít, je použití podrobného průvodce. Můžete také [přidat zařízení](create-and-edit-autopilot-devices.md) a přiřadit jim [profily](create-and-edit-autopilot-profiles.md) bez použití průvodce. 
  
1. Přejděte do centra <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>pro správu na adrese .

2. V levém navigačním podokně zvolte **Zařízení** \> **AutoPilot**.

    ![V Centru pro správu zvolte zařízení a pak AutoPilot.](../media/AutoPilot.png)
  
2. Na stránce **AutoPilot** klikněte nebo klepněte na **Úvodní příručka**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na **stránce Upload .csv se seznamem zařízení** vyhledejte místo, kde máte připravené . CSV soubor, pak **Otevřít** \> **další**. Soubor musí mít tři záhlaví:
    
    - Sloupec A: Sériové číslo zařízení
    
    - Sloupec B: ID produktu Windows
    
    - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete použít [skript Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) ke generování souboru CSV. 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
4. Na stránce **Přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový. Pokud ještě ho nemáte, budete vyzváni k jeho vytvoření. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou povinné a jsou nastaveny automaticky. Výchozí funkce:
    
    - Přeskočit registraci Cortany, OneDrivu a OEM.
    
    - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
    - Připojte svá zařízení k účtům Služby Azure Active Directory a automaticky je zaregistrujte, aby je spravoval Microsoft 365 Business.
    
    Další informace naleznete v tématu [O nastavení profilu automatického pilota](autopilot-profile-settings.md). 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. **Jste hotovi** znamená, že profil, který jste vytvořili (nebo jste zvolili) bude použit pro skupinu zařízení, kterou jste vytvořili nahráním seznamu zařízení. Nastavení bude v platnosti, když se uživatelé zařízení přihlašují příště. Zvolte **Zavřít**.
    
