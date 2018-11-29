---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Informace o povolení 365 Microsoft chránit místní AD připojené zařízení Windows 10.
ms.openlocfilehash: 6e66a2c5417c9037232c1ada654d4cac3c520607
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982651"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business

Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních. To lze nastavit tak, že první synchronizace služby Active Directory s Azure Active Directory, následuje zápis zařízení Windows 10 s Azure AD a zápis je pro správu mobilních zařízení pomocí Microsoft 365 Business.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Nastavit zařízení připojeno k doméně, které jsou spravovány Microsoft 365 Business

Chcete-li nastavit zařízení připojeno k doméně organizace využívat funkce poskytované službou Active Directory Azure kromě místního Active Directory, můžete implementovat **hybridní Azure AD připojené zařízení**. Jedná se o zařízení, které jsou připojeny do adresáře služby Active Directory v prostorách a Azure AD. Hybridní zařízení Azure AD, které jsou spojeny mohou být chráněné a spravovány Microsoft 365 Business... 
  
Postupujte podle pokynů níže vytvořit hybridní Azure AD připojen a spravovány Microsoft 365 Business zařízení Windows 10.
  
1. K synchronizaci uživatelů, skupin a kontaktů z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresáře a Azure Active Directory připojení jak je popsáno v [Nastavení synchronizace adresáře služeb Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Kroky jsou přesně Microsoft 365 Business. 
  
2. Před provedením kroku 3, chcete-li povolit zařízení Windows 10 bude hybridní připojen k Azure AD, je třeba Ujistěte se, že jsou splněny následující předpoklady:
    
   - Používáte nejnovější verzi Azure AD připojit.
    
   - Azure AD připojit synchronizaci všech objektů počítače zařízení má být hybridní připojen k Azure AD. Pokud objekty počítače patří do určité organizační jednotky (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v Azure AD připojte také.
    
3. Registrace existující zařízení Windows 10 doméně hybridní Azure AD Joined a zapsat je spravovat mobilní zařízení pomocí Intune (Microsoft 365 Business):
    
4. Postupujte podle pokynů krok za krokem [Konfigurace hybridní zařízení Azure Active Directory připojen](https://go.microsoft.com/fwlink/p/?linkid=872870). To umožní synchronizaci služby Active Directory v prostorách připojené počítače Windows 10 a je připraveno v cloudu.
    
5. K zápisu Windows 10 zařízení, Správa mobilního zařízení, pokyny naleznete v tématu [zápis Windows 10 zařízení s Intune pomocí Zásady skupiny](https://go.microsoft.com/fwlink/p/?linkid=872871) . Můžete nastavit Zásady skupiny v místním počítači úrovni nebo pro hromadné operace, můžete vytvořit na serveru řadiče domény toto nastavení zásad skupiny. 
    

