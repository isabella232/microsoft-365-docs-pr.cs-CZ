---
title: Podrobné pokyny k přidání zařízení a profilů Autopilota
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Další informace o použití AutoPilot systému Windows k nastavení nových Windows 10 zařízení pro vaše podnikání.
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660652"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Podrobné pokyny k přidání zařízení a profilů Autopilota

AutoPilot systému Windows slouží k nastavení **nových** Windows 10 zařízení pro vaše podnikání tak, aby byly připraveny pro produktivní využití co nejdříve poskytnout vašim zaměstnancům.
  
## <a name="device-requirements"></a>Požadavky na zařízení

Zařízení musejí splňovat tyto podmínky:
  
- Windows 10 verze 1703 nebo novější.
    
- Nová zařízení, na kterých nedošlo ke spuštění softwaru Windows používaného při prvním zapnutí počítače.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Vytvoření zařízení a profilů pomocí průvodce instalací

![Banner odkazující na https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Pokud jste ještě nevytvořili skupiny zařízení ani jejich profily, bude nejlepší, když na začátku použijete podrobného průvodce. [Přidat zařízení](create-and-edit-autopilot-devices.md) a [přiřadit profily](create-and-edit-autopilot-profiles.md) ale můžete i bez průvodce. 
  
1. Přejděte na stránku Správce na <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. Na navigace vlevo zvolte **zařízení** \> **AutoPilot**.

    ![V Centru správy vyberte zařízení a pak AutoPilot.](media/AutoPilot.png)
  
2. Na stránce **AutoPilot** klepněte na položku nebo klepněte na tlačítko **Spustit Průvodce**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Na stránce **Nahrát soubor .csv obsahující seznam zařízení** přejděte k místu, kde máte připravený soubor CSV, a vyberte **Otevřít** \> **Další**. Soubor musí mít tři záhlaví:
    
  - Sloupec A: Sériové číslo zařízení
    
  - Sloupec B: ID produktu Windows
    
  - Sloupec C: Hodnota hash hardwaru
    
    Tyto informace můžete získat od svého dodavatele hardwaru nebo můžete použít [skript PowerShellu Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), který vygeneruje soubor CSV. 
    
    Další informace najdete v článku [Soubor CSV se seznamem zařízení](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Můžete si také stáhnout ukázkový soubor, který je na stránce **Nahrát soubor .csv obsahující seznam zařízení**. 
    
4. Na stránce **Přiřadit profil** můžete vybrat stávající profil nebo můžete vytvořit profil nový. Pokud ho ještě nemáte, zobrazí se výzva k vytvoření nového profilu. 
    
    Profil je kolekce nastavení, kterou můžete použít u jednotlivých zařízení nebo u skupiny zařízení.
    
    Výchozí funkce jsou povinné a nastaví se automaticky. Výchozí funkce:
    
  - Přeskočení Cortany, OneDrivu a registrace OEM.
    
  - Vytvoření postupu přihlášení doplněného o značku společnosti.
    
  - Zařízení se připojí k účtům adresářové služby Azure Active Directory a automaticky se zaregistrují, aby je bylo možné spravovat ve službě Microsoft 365 Business.
    
    Další informace najdete v článku
    
    [Informace o nastavení profilu AutoPilota](autopilot-profile-settings.md) . 
    
5. Další nastavení jsou **Přeskočit nastavení ochrany osobních údajů** a **Nepovolit uživateli stát se místním správcem**. Obě volby jsou automaticky nastavené na **Vypnuto**. 
    
    Zvolte **Další**.
    
6. Stránka **Hotovo!** znamená, že vytvořený (nebo zvolený) profil se použije u skupiny zařízení vytvořené nahráním seznamu zařízení. Tato nastavení platí i při příštím přihlášení uživatelů zařízení. Zvolte **Zavřít**.
    