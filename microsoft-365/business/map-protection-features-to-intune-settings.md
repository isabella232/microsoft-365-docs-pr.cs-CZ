---
title: Jak se funkce ochrany v Microsoft 365 Business Premium mapovat na nastavení Intune
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Zjistěte, jak se funkce ochrany Microsoft 365 Business Premium mapovat na nastavení Intune. Předplatné vám poskytuje licenci na úpravu nastavení Intune.
ms.openlocfilehash: 844b83bca9483f72fd322d666803c42b90fee41d3e0047ea93b4b6b07717b0dd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852725"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Jak se funkce ochrany v Microsoft 365 Business Premium mapovat na nastavení Intune

## <a name="android-and-ios-application-protection-settings"></a>Nastavení ochrany aplikace pro Android a iOS

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení zásad aplikace pro Android a iOS na nastavení Intune.
  
Pokud chcete nastavení Intune najít, přihlaste se pomocí přihlašovacích údajů Microsoft 365 Business Premium správce, přejděte na **Centra pro** správu a potom **na Intune.**
  
 > [!IMPORTANT]
 > 
 > Předplatné Microsoft 365 Business Premium licence k úpravě všech nastavení Intune. Začínáme [v tématu Úvod do Intune.](/intune/introduction-intune)
  
Vyberte název zásady, který chcete použít, například Zásady aplikace pro Android a &mdash; pak zvolte Nastavení &mdash; **zásad**.
  
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
|Resetovat PIN kód v případě, že se přihlášení tolikrát nepovede (pokud pin kód není povinný)  <br/> |Počet pokusů před resetem PIN kódu  <br/> |
|Vyžadovat, aby se uživatelé znovu přihlašoval Office aplikace byly nečinné (toto je zakázané, pokud pin kód není povinný)  <br/> | Překontrolovat požadavky na přístup za (minuty)  <br/>  Tímto se zároveň nastaví:  <br/> **Časový limit** se nastaví na počet minut.  <br/>  Jedná se o stejný počet minut, který nastavíte v aplikaci Microsoft 365 Business.  <br/> **Období odkladu pro offline režim** je ve výchozím nastavení nastavené na 720 minut.  <br/> |
|Odepřít přístup k pracovním souborům ze zařízení s jailbreakem nebo rootem  <br/> |Blokovat spouštění spravovaných aplikací na zařízeních s jailbreakem nebo rootem  <br/> |
|Povolit uživatelům kopírovat obsah z aplikací Office do osobních aplikací  <br/> | Omezení vyjmutí, kopírování a vkládání s jinými aplikacemi  <br/>  Pokud je možnost Microsoft 365 Business Premium nastavená na **Hodnotu Za**, pak jsou tyto tři možnosti taky nastavené na Všechny **aplikace** v Intune:  <br/> **Povolit aplikaci posílat data do jiných aplikací** <br/> **Povolit aplikaci přijímat data z jiných aplikací** <br/> **Zakázat operace vyjmutí, kopírování a vložení s jinými aplikacemi** <br/>  Pokud je možnost Microsoft 365 Business nastavená na **Zapnuto**, pak se všechny možnosti Intune nastaví na:  <br/> **Povolit aplikaci posílat data do jiných aplikací** se nastaví na **Aplikace spravované podle zásad**. <br/> **Povolit aplikaci přijímat data z jiných aplikací** se nastaví na **Všechny aplikace**. <br/> **Zakázat operace vyjmutí, kopírování a vložení s jinými aplikacemi** se nastaví na **Aplikace s vložením spravované podle zásad**. <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Nastavení ochrany aplikace pro Windows 10

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení zásad aplikace pro Windows 10 na nastavení Intune.
  
Pokud chcete najít nastavení Intune, přihlaste se pomocí přihlašovacích Microsoft 365 Business Premium správce a přejděte na [portál Azure Portal.](https://portal.azure.com) Vyberte **Další služby** a do pole Filtr zadejte **Intune.** Vyberte **Zásady aplikace Intune App Protection.** \> 
  
 > [!IMPORTANT]
 >
 >Předplatné Microsoft 365 Business Premium licence k úpravě jenom nastavení Intune, která se mapuje na nastavení dostupná v Microsoft 365 Business Premium. 
  
Pokud chcete prozkoumat dostupná nastavení, vyberte požadovaný název zásady a v levém navigačním podokně  zvolte **Obecné,** Zadání **,** Povolené aplikace **,** Aplikace s výjimkami **,** Požadovaná nastavení nebo Upřesnit nastavení. 
  
|**Nastavení zásad aplikace pro Windows 10**|**Nastavení Intune**|
|:-----|:-----|
|Šifrovat pracovní soubory  <br/> |**Upřesnit nastavení** \> **Ochrana dat**: **Odvolat šifrovací klíče při zrušení registrace** i **Odvolat přístup k chráněným datům, když se zařízení zaregistruje k MDM** se nastaví na **Zapnuto**.  <br/> |
|Bránit uživatelům v kopírování dat společnosti do osobních souborů  <br/> |**Požadované nastavení** \> režim **Windows Information Protection**. **On** in Microsoft 365 Business Premium mapy to: **Hide Overrides**, **Off** in Microsoft 365 Business Premium maps to: **Off**.  <br/> |
|Řízení přístupu k dokumentům Office  <br/> | Pokud je tato možnost **v** Microsoft 365 Business Premium nastavená,  <br/> **Upřesnit nastavení** \> **Přístup**, **Používat Windows Hello pro firmy jako metody přihlašování do Windows** nastaví na **Zapnuto** spolu s následujícími dalšími nastaveními:  <br/> **Nastavte minimální počet znaků vyžadovaných pro PIN kód** se nastaví na **4**.  <br/> **Nakonfigurujte využití velkých písmen v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání velkých písmen v PIN kódu**.  <br/> **Nakonfigurujte využití malých písmen v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání malých písmen v PIN kódu**.  <br/> **Nakonfigurujte využití speciálních znaků v PIN kódu Windows Hello pro firmy** se nastaví na **Nepovolit používání speciálních znaků v PIN kódu**.  <br/> **Zadejte časové období (ve dnech),** po které se může PIN kód použít před tím, než systém vyžaduje, aby se uživatel změnil, na **hodnotu 0**.  <br/> **Zadejte počet předchozích PIN kódů přidružených k uživatelskému účtu, které se nedají použít znovu** se nastaví na **0**.  <br/> **Počet povolených neúspěšných přihlášení, než se zařízení vymaže** se nastaví stejně jako v aplikaci Microsoft 365 Business (ve výchozím nastavení je to 5).  <br/> **Maximální doba (v minutách), po kterou může zařízení zůstat neaktivní, než se zamkne PIN kódem nebo heslem**, se nastaví na stejnou hodnotu jako v aplikaci Microsoft 365 Business.  <br/> |
|Povolit obnovení chráněných dat  <br/> |**Upřesnit nastavení** \> **Ochrana dat**: **Zobrazit ikonu ochrany podnikových dat** a **Použít Azure RMS pro WIP** se nastaví na **Zapnuto**.  <br/> |
|Chránit další umístění v cloudu společnosti  <br/> |**Upřesnit nastavení** \> **Chráněné domény** a **Cloudové prostředky** zobrazují domény a weby SharePointu.  <br/> |
|Soubory používané těmito aplikacemi jsou chráněny.  <br/> |Seznam chráněných aplikací najdete pod položkou **Povolené aplikace**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Nastavení ochrany zařízení s Windows 10

V následující tabulce najdete podrobnosti o tom, jak namapovat nastavení konfigurace zařízení s Windows 10 na nastavení Intune.
  
Pokud chcete najít nastavení Intune, přihlaste se pomocí přihlašovacích údajů správce Microsoft 365 Business Premium přejděte na [Portál Azure,](https://portal.azure.com)vyberte Další služby a zadejte Intune do filtru **a** vyberte Profily konfigurace zařízení  \>  \> Intune. Potom vyberte **Zásada zařízení pro Windows 10** \> **Vlastnosti** \> **Nastavení**.
  
|**Nastavení zásad zařízení s Windows 10**|**Nastavení Intune**|
|:-----|:-----|
|Zvýšit ochranu počítačů před viry a dalšími hrozbami pomocí Antivirové ochrany v programu Windows Defender  <br/> |Povolit sledování v reálném čase = ZAPNUTO  <br/> Povolit ochranu cloudu = ZAPNUTO  <br/> Vyzývat uživatele k odesílání vzorků = Posílat bezpečné vzorky automaticky (výchozí nastavení s automatickým odesíláním údajů kromě identifikovatelných osobních údajů)  <br/> |
|Chránit počítače před webovými hrozbami v prohlížeči Microsoft Edge  <br/> |**SmartScreen** v **nastavení prohlížeče Microsoft Edge** se nastaví na **Povinné**.  <br/> |
|Vypnout obrazovku zařízení po nečinnosti (v minutách)  <br/> |Maximální počet minut nečinnosti, po kterém se zamkne obrazovka (v minutách)  <br/> |
|Povolit uživatelům stahovat aplikace z webu Microsoft Store  <br/> |Vlastní zásada identifikátoru URI  <br/> |
|Umožnit uživatelům přístup ke Cortaně  <br/> |**Obecné** \> **Cortana** je nastavená na blokování **v** Intune, když **je** v Microsoft 365 Business Premium.  <br/> |
|Povolit uživatelům přijímat tipy pro Windows a reklamy od společnosti Microsoft  <br/> |**Windows vybrané** oblasti jsou všechny zablokované, pokud **je** tato možnost v Microsoft 365 Business Premium.  <br/> |
|Automaticky aktualizovat zařízení s Windows 10  <br/> | Toto nastavení je v **Microsoft Intune** \> **service updates ( Windows 10 Update Rings**), zvolte Update policy for Windows 10 **devices**(Zásady aktualizace pro Windows 10 zařízení) a **potom Vlastnosti** \> **Nastavení**.  <br/>  Pokud je Microsoft 365 Business Premium nastavená možnost **Na**, nastaví se všechna následující nastavení:  <br/> **Větev služby** je nastavená na **CB** (CBB, pokud je tato větev vypnutá v Microsoft 365 Business Premium).  <br/> **Aktualizace produktů Microsoft** se nastaví na **Povolit**.  <br/> **Ovladače Windows** se nastaví na **Povolit**.  <br/> **Chování automatické aktualizace** se nastaví na **Automaticky nainstalovat v době údržby** spolu s následujícím:  <br/> **Začátek aktivní doby** se nastaví na **6:00**.  <br/> **Konec aktivní doby** se nastaví na **22:00**.  <br/> **Odložení aktualizace kvality (ve dnech)** se nastaví na **0**.  <br/> **Odložení aktualizace funkcí (ve dnech)** se nastaví na **0**.  <br/> **Režim stahování pro optimalizaci doručení** se nastaví na **HTTP v kombinaci s partnery za stejným překladem NAT**.  <br/> |
|||
