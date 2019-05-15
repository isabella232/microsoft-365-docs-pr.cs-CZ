---
title: Mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 8/13/2018
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
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Zjistěte, jak mapovat funkce ochrany v Microsoft 365 Business nastavení Intune. Předplatné vám poskytuje licenci k úpravě nastavení Intune.
ms.openlocfilehash: a6aaf6cc06c31b870eb85582f5aa47699919d75d
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074254"
---
# <a name="how-do-protection-features-in-microsoft-365-business-map-to-intune-settings"></a>Mapování funkcí ochrany v Microsoft 365 Business na nastavení Intune

## <a name="android-and-ios-application-protection-settings"></a>Nastavení ochrany aplikace pro Android a iOS

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení zásad aplikace pro Android a iOS na nastavení Intune.
  
Pokud chcete najít nastavení Intune, když jste přihlášení pomocí přihlašovacích údajů správce plánu Microsoft 365 Business, přejděte na **Centra pro správu** a potom na **Intune**.
  
 **Důležité:** Předplatné Microsoft 365 Business vám poskytuje licenci k úpravě všech nastavení Intune. Viz [Úvod do Intune začít.](https://docs.microsoft.com/intune/introduction-intune)
  
Klikněte na název zásady, kterou chcete vybrat, například Zásady aplikace pro Android, a potom vyberte **Nastavení zásady**.
  
Pod **Chránit pracovní soubory při ztrátě nebo odcizení zařízení**
  
|**Nastavení zásad aplikace pro Android nebo iOS**|**Nastavení Intune**|
|:-----|:-----|
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Doba v offline režimu (ve dnech) před vymazáním dat  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> Nezapomeňte, že je povolený jenom OneDrive pro firmy.  <br/> |Vyberte, do kterých služeb úložiště se můžou ukládat firemní data  <br/> |
|||
   
Pod **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních**
  
|**Nastavení zásad aplikace pro Android nebo iOS**|**Nastavení Intune**|
|:-----|:-----|
|Odstranit pracovní soubory z neaktivního zařízení za  <br/> |Doba v offline režimu (ve dnech) před vymazáním dat  <br/> |
|Vynucovat, aby uživatelé ukládali všechny pracovní soubory na OneDrive pro firmy  <br/> Nezapomeňte, že je povolený jenom OneDrive pro firmy.  <br/> |Vyberte, do kterých služeb úložiště se můžou ukládat firemní data  <br/> |
|Šifrovat pracovní soubory  <br/> |Šifrovat data aplikace  <br/> |
|Pod **Spravovat přístup uživatelů k souborům Office na mobilních zařízeních** <br/> ||
|Vyžadovat pro přístup k aplikacím Office PIN nebo otisk prstu  <br/> | Vyžadovat pro přístup PIN kód  <br/>  Tímto se zároveň nastaví:  <br/> **Povolit jednoduchý PIN kód** na **Ano** <br/> **Délka PIN kódu** na 4  <br/> **Povolit otisk prstu místo PIN kódu** na **Ano** <br/> **Zakázat PIN kód aplikace, když je PIN kód zařízení spravovaný** na **Ne** <br/> |
|Resetovat PIN kód po tomto počtu neúspěšných přihlášení (pokud se nevyžaduje PIN kód, tato možnost se vypne).  <br/> |Počet pokusů před resetem PIN kódu  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlásili, pokud byly aplikace Office nečinné po dobu (pokud se nevyžaduje PIN kód, tato možnost se vypne).  <br/> | Překontrolovat požadavky na přístup za (minuty)  <br/>  Tímto se zároveň nastaví:  <br/> **Časový limit** se nastaví na počet minut.  <br/>  Jedná se o stejný počet minut, který nastavíte v aplikaci Microsoft 365 Business.  <br/> **Období odkladu pro offline režim** je ve výchozím nastavení nastavené na 720 minut.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Blokovat spouštění spravovaných aplikací na zařízeních s jailbreakem nebo rootem  <br/> |
|Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací  <br/> | Zakázat operace vyjmutí, kopírování a vložení s jinými aplikacemi  <br/>  Pokud je možnost Microsoft 365 Business nastavená na **Zapnuto**, pak se v Intune také nastaví následující tři možnosti na **Všechny aplikace**:  <br/> **Povolit aplikaci posílat data do jiných aplikací** <br/> **Povolit aplikaci přijímat data z jiných aplikací** <br/> **Zakázat operace vyjmutí, kopírování a vložení s jinými aplikacemi** <br/>  Pokud je možnost Microsoft 365 Business nastavená na **Zapnuto**, pak se všechny možnosti Intune nastaví na:  <br/> **Povolit aplikaci posílat data do jiných aplikací** se nastaví na **Aplikace spravované podle zásad**. <br/> **Povolit aplikaci přijímat data z jiných aplikací** se nastaví na **Všechny aplikace**. <br/> **Zakázat operace vyjmutí, kopírování a vložení s jinými aplikacemi** se nastaví na **Aplikace s vložením spravované podle zásad**. <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Nastavení ochrany aplikace pro Windows 10

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení zásad aplikace pro Windows 10 na nastavení Intune.
  
Intune nastavení, zatímco přihlášen pomocí pověření správce Microsoft 365 Business naleznete na [portálu Azure](https://portal.azure.com)a potom vyberte **Další služby**a typ v Intune do **filtru**vybrat **Ochranu Intune App** \> ** Aplikace zásad**.
  
 **Důležité**: Předplatné Microsoft 365 Business vám dává právo upravovat pouze nastavení Intune mapovatelná na nastavení, která jsou k dispozici v Microsoft 365 Business. 
  
Klikněte na název zásady, kterou chcete vybrat, a potom zvolte **Obecné, Přiřazení**, **Povolené aplikace**, **Aplikace s výjimkou**, **Požadovaná nastavení** nebo **Upřesnit nastavení** v levém navigačním panelu a podívejte se na dostupná nastavení. 
  
|**Nastavení zásad aplikace pro Windows 10**|**Nastavení Intune**|
|:-----|:-----|
|Šifrovat pracovní soubory  <br/> |**Upřesnit nastavení** \> **Ochrana dat**: **Odvolat šifrovací klíče při zrušení registrace** i **Odvolat přístup k chráněným datům, když se zařízení zaregistruje k MDM** se nastaví na **Zapnuto**.  <br/> |
|Bránit uživatelům v kopírování dat společnosti do osobních souborů  <br/> |**Požadované nastavení** \> režim **Windows Information Protection**. **Zapnuto** v Microsoft 365 Business se namapuje na: **Skrýt potlačení**, **Vypnuto** v Microsoft 365 Business se namapuje na: **Vypnuto**.  <br/> |
|Řízení přístupu k dokumentům Office  <br/> | Pokud je tato možnost v Microsoft 365 Business nastavená na **Zapnuto**, pak se  <br/> **Upřesnit nastavení** \> **Přístup**, **Používat Windows Hello pro firmy jako metody přihlašování do Windows** nastaví na **Zapnuto** spolu s následujícími dalšími nastaveními:  <br/> **Nastavte minimální počet znaků vyžadovaných pro PIN kód** se nastaví na **4**.  <br/> **Nakonfigurujte využití velkých písmen v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání velkých písmen v PIN kódu**.  <br/> **Nakonfigurujte využití malých písmen v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání malých písmen v PIN kódu**.  <br/> **Nakonfigurujte využití speciálních znaků v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání speciálních znaků v PIN kódu**.  <br/> **Zadejte dobu (ve dnech), po kterou se PIN kód může používat, než bude systém vyžadovat, aby ho uživatel změnil** se nastaví na **0**.  <br/> **Zadejte počet předchozích PIN kódů přidružených k uživatelskému účtu, které se nedají použít znovu** se nastaví na **0**.  <br/> **Počet povolených neúspěšných přihlášení, než se zařízení vymaže** se nastaví stejně jako v aplikaci Microsoft 365 Business (ve výchozím nastavení je to 5).  <br/> **Maximální doba (v minutách), po kterou může zařízení zůstat neaktivní, než se zamkne PIN kódem nebo heslem**, se nastaví na stejnou hodnotu jako v aplikaci Microsoft 365 Business.  <br/> |
|Povolit obnovení chráněných dat  <br/> |**Upřesnit nastavení** \> **Ochrana dat**: **Zobrazit ikonu ochrany podnikových dat** a **Použít Azure RMS pro WIP** se nastaví na **Zapnuto**.  <br/> |
|Chránit další umístění v cloudu společnosti  <br/> |**Upřesnit nastavení** \> **Chráněné domény** a **Cloudové prostředky** zobrazují domény a weby SharePointu.  <br/> |
|Soubory používané těmito aplikacemi jsou chráněny.  <br/> |Seznam chráněných aplikací najdete pod položkou **Povolené aplikace**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Nastavení ochrany zařízení s Windows 10

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení konfigurace zařízení s Windows 10 na nastavení Intune.
  
Intune nastavení, zatímco přihlášen pomocí pověření správce Microsoft 365 Business naleznete na [portálu Azure](https://portal.azure.com)a potom vyberte **Další služby**a typ v Intune do **filtru**vyberte **Intune** \> **zařízení Konfigurace** \> **profily**. Potom vyberte **Zásada zařízení pro Windows 10** \> **Vlastnosti** \> **Nastavení**.
  
|**Nastavení zásad zařízení s Windows 10**|**Nastavení Intune**|
|:-----|:-----|
|Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender  <br/> |Povolit sledování v reálném čase = ZAPNUTO  <br/> Povolit ochranu cloudu = ZAPNUTO  <br/> Vyzývat uživatele k odesílání vzorků = Posílat bezpečné vzorky automaticky (výchozí nastavení s automatickým odesíláním údajů kromě identifikovatelných osobních údajů)  <br/> |
|Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge  <br/> |**SmartScreen** v **nastavení prohlížeče Microsoft Edge** se nastaví na **Povinné**.  <br/> |
|Vypnout obrazovku zařízení po nečinnosti (v minutách)  <br/> |Maximální počet minut nečinnosti, po kterém se zamkne obrazovka (v minutách)  <br/> |
|Povolit uživatelům stahovat aplikace z webu Microsoft Store  <br/> |Vlastní zásada identifikátoru URI  <br/> |
|Umožnit uživatelům přístup ke Cortaně  <br/> |**Obecné** \> **Cortana** se v Intune nastaví na **Blokovat**, pokud je tato možnost v Microsoft 365 Business nastavená na **Vypnuto**.  <br/> |
|Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft  <br/> |**Windows Spotlight**: pokud je toto nastavení v Microsoft 365 Business nastavené na **Vypnuto**, je všechno zablokované.  <br/> |
|Automaticky aktualizovat zařízení s Windows 10  <br/> | This setting is in **Microsoft Intune** \> **Service updates - Windows 10 Update Rings**, choose U **pdate policy for Windows 10 devices**, and then **Properties** \> **Settings**.  <br/>  Když je nastavení Microsoft 365 Business nastaveno na **Zapnuto**, nastaví se všechna následující nastavení:  <br/> **Obslužná větev** se nastaví na **CB** (CBB, pokud je tato možnost v Microsoft 365 Business vypnutá).  <br/> **Aktualizace produktů Microsoft** se nastaví na **Povolit**.  <br/> **Ovladače Windows** se nastaví na **Povolit**.  <br/> **Chování automatické aktualizace** se nastaví na **Automaticky nainstalovat v době údržby** spolu s následujícím:  <br/> **Začátek aktivní doby** se nastaví na **6:00**.  <br/> **Konec aktivní doby** se nastaví na **22:00**.  <br/> **Odložení aktualizace kvality (ve dnech)** se nastaví na **0**.  <br/> **Odložení aktualizace funkcí (ve dnech)** se nastaví na **0**.  <br/> **Režim stahování pro optimalizaci doručení** se nastaví na **HTTP v kombinaci s partnery za stejným překladem NAT**.  <br/> |
|||
   

