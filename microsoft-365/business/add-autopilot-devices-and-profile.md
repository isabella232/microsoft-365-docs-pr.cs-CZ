---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
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
description: Naučte se používat funkci Windows AutoPilot k nastavení nových zařízení systému Windows 10 pro váš podnik.
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323089"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

Pomocí systému Windows AutoPilot můžete nastavit **nové** systémy Windows 10 pro váš podnik, takže jsou připraveny k použití, když je dáte svým zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musí splňovat tyto požadavky:
  
- Windows 10, verze 1703 nebo novější
    
- Nová zařízení, která nebyla součástí systému Windows,
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Pokud jste ještě nevytvořili skupiny zařízení nebo profily, nejlepším způsobem, jak začít, je použití podrobných vodítek. Můžete také [Přidat zařízení](create-and-edit-autopilot-devices.md) a [přiřadit jim profily](create-and-edit-autopilot-profiles.md) bez použití průvodce. 
  
1. Přejděte do centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>adrese.

2. V levém navigačním podokně vyberte položku **zařízení** \> **autopilot**.

    ![V centru pro správu zvolte zařízení a pak položku AutoPilot.](media/AutoPilot.png)
  
2. Na stránce **autopilot** klikněte na tlačítko nebo na položku **Start Guide**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. V **souboru upload. CSV se seznamem zařízení** přejděte do umístění, kde je připraven. CSV a potom **otevřete** \> **Další**. Soubor musí obsahovat tři hlavičky:
    
    - Sloupec A: Sériové číslo zařízení
    
    - Sloupec B: ID produktu Windows
    
    - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete vytvořit soubor CSV pomocí [skriptu PowerShell Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) . 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
4. Na stránce **přiřadit profil** můžete buď vybrat existující profil, nebo vytvořit nový. Pokud ještě žádnou nemáte, budete vyzváni k jeho vytvoření. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou vyžadovány a jsou nastaveny automaticky. Výchozí funkce:
    
    - Vynechejte Cortana, OneDrive a registraci OEM.
    
    - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
    - Připojte zařízení k účtům služby Active Directory společnosti Azure a automaticky je zapište, aby byly spravovány společností Microsoft 365 Business.
    
    Další informace naleznete v tématu [o nastavení profilu AutoPilot](autopilot-profile-settings.md). 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. **Vaše práce** znamená, že vytvořený profil (nebo zvolený) bude použit u skupiny zařízení, kterou jste vytvořili, uložením seznamu zařízení. Nastavení bude platné po přihlášení uživatelů zařízení. Zvolte **Zavřít**.
    