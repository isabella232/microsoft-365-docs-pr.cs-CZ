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
description: Přečtěte si, jak pomocí Windows AutoPilota nastavit nová zařízení s Windows 10 pro vaši firmu, aby byla připravená k použití pro zaměstnance.
ms.openlocfilehash: f263cc90656ae5e7be1a89e3c7f56bfb2d0e3651
ms.sourcegitcommit: 3b369a44b71540c8b8214ce588a7aa6f47c3bb1e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/04/2021
ms.locfileid: "50099744"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

Pomocí Windows AutoPilota můžete nastavit nová zařízení s **Windows** 10 pro vaši firmu, aby byla připravená k použití, když je předáte zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musí splňovat tyto požadavky:
  
- Windows 10 verze 1703 nebo novější
    
- Nová zařízení, na která se nevyužívá předchycené zařízení s Windows
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

[![Popis s informacemi o tom, jak se mění centrum pro správu. Další podrobnosti najdete na aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Pokud jste skupiny zařízení nebo profily zařízení ještě nevytáčili, je nejlepší začít pomocí podrobného průvodce. Můžete taky přidat [zařízení a](create-and-edit-autopilot-devices.md) přiřadit k nim [profily](create-and-edit-autopilot-profiles.md) bez použití průvodce. 
  
1. Přejděte do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. V levém navigačním podokně zvolte **Devices** \> **AutoPilot (Zařízení AutoPilota).**

    ![V Centru pro správu zvolte zařízení a pak AutoPilota.](../media/AutoPilot.png)
  
2. Na stránce **AutoPilota** klikněte nebo klepněte na **Úvodní příručku.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na stránce **Upload .csv file with list of devices** (Nahrát soubor CSV se seznamem zařízení) přejděte na místo, kde máte připravené zařízení. CSV a pak **Otevřít** \> **další.** Soubor musí mít tři záhlaví:
    
    - Sloupec A: Sériové číslo zařízení
    
    - Sloupec B: ID produktu Windows
    
    - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od dodavatele hardwaru nebo můžete použít skript [PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) k vygenerování souboru CSV. 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
> [!NOTE]
> Tento skript používá FUNKCI BLUETOOTH k načtení vlastností potřebných k registraci zařízení v programu Windows Autopilot. Všimněte si, že výsledný soubor CSV obvykle neshromažďuje hodnotu ID produktu Windows (PKID), protože to není potřeba k registraci zařízení a PKID being NULL ve výstupním SOUBORU CSV je úplně v pořádku. Vyplní se jenom sériové číslo a hodnota hash hardwaru.
    
4. Na stránce **Přiřadit profil** můžete vybrat existující profil nebo vytvořit nový profil. Pokud ho ještě nemáte, zobrazí se výzva k jeho vytvoření. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou povinné a nastavují se automaticky. Výchozí funkce:
    
    - Přeskočit registraci Cortany, OneDrivu a OEM.
    
    - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
    - Připojte zařízení k účtům Azure Active Directory a automaticky je zaregistrujte, aby je bylo možné spravovat pomocí Microsoft 365 Business Premium.
    
    Další informace najdete v tématu [o nastavení profilu AutoPilota.](autopilot-profile-settings.md) 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. **Máte hotovo, že** profil, který jste vytvořili (nebo vybrali), se použije u skupiny zařízení, kterou jste vytvořili nahráněním seznamu zařízení. Toto nastavení bude mít vliv na to, když se uživatelé zařízení přihlásí příště. Zvolte **Zavřít**.
    
