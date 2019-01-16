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
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982651"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="fe1d7-103">Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fe1d7-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="fe1d7-p101">Pokud vaše organizace používá služby Active Directory systému Windows Server na prostory, můžete nastavit Microsoft 365 Business chránit vaše zařízení Windows 10, ale zároveň zachovat přístup k místním prostředkům, které vyžadují ověřování pomocí místních. To lze nastavit tak, že první synchronizace služby Active Directory s Azure Active Directory, následuje zápis zařízení Windows 10 s Azure AD a zápis je pro správu mobilních zařízení pomocí Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-p101">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication. You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="fe1d7-106">Nastavit zařízení připojeno k doméně, které jsou spravovány Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fe1d7-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="fe1d7-p102">Chcete-li nastavit zařízení připojeno k doméně organizace využívat funkce poskytované službou Active Directory Azure kromě místního Active Directory, můžete implementovat **hybridní Azure AD připojené zařízení**. Jedná se o zařízení, které jsou připojeny do adresáře služby Active Directory v prostorách a Azure AD. Hybridní zařízení Azure AD, které jsou spojeny mohou být chráněné a spravovány Microsoft 365 Business...</span><span class="sxs-lookup"><span data-stu-id="fe1d7-p102">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**. These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory. Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business..</span></span> 
  
<span data-ttu-id="fe1d7-110">Postupujte podle pokynů níže vytvořit hybridní Azure AD připojen a spravovány Microsoft 365 Business zařízení Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="fe1d7-111">K synchronizaci uživatelů, skupin a kontaktů z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresáře a Azure Active Directory připojení jak je popsáno v [Nastavení synchronizace adresáře služeb Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="fe1d7-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="fe1d7-112">Kroky jsou přesně Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="fe1d7-113">Před provedením kroku 3, chcete-li povolit zařízení Windows 10 bude hybridní připojen k Azure AD, je třeba Ujistěte se, že jsou splněny následující předpoklady:</span><span class="sxs-lookup"><span data-stu-id="fe1d7-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>
    
   - <span data-ttu-id="fe1d7-114">Používáte nejnovější verzi Azure AD připojit.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-114">You are running the latest version of Azure AD connect.</span></span>
    
   - <span data-ttu-id="fe1d7-p103">Azure AD připojit synchronizaci všech objektů počítače zařízení má být hybridní připojen k Azure AD. Pokud objekty počítače patří do určité organizační jednotky (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v Azure AD připojte také.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-p103">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined. If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="fe1d7-117">Registrace existující zařízení Windows 10 doméně hybridní Azure AD Joined a zapsat je spravovat mobilní zařízení pomocí Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="fe1d7-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="fe1d7-p104">Postupujte podle pokynů krok za krokem [Konfigurace hybridní zařízení Azure Active Directory připojen](https://go.microsoft.com/fwlink/p/?linkid=872870). To umožní synchronizaci služby Active Directory v prostorách připojené počítače Windows 10 a je připraveno v cloudu.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-p104">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870). This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="fe1d7-p105">K zápisu Windows 10 zařízení, Správa mobilního zařízení, pokyny naleznete v tématu [zápis Windows 10 zařízení s Intune pomocí Zásady skupiny](https://go.microsoft.com/fwlink/p/?linkid=872871) . Můžete nastavit Zásady skupiny v místním počítači úrovni nebo pro hromadné operace, můžete vytvořit na serveru řadiče domény toto nastavení zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="fe1d7-p105">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions. You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span> 
    

