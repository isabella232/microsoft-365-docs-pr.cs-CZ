---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Dozvíte se, jak povolit aplikaci Microsoft 365 chránit místní služby AD připojené k zařízením Windows 10.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992223"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="ea90b-103">Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="ea90b-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="ea90b-104">Pokud vaše organizace používá v místním počítači službu Active Directory systému Windows Server, můžete nastavit ochranu zařízení systému Windows 10 v aplikaci Microsoft 365 Business a současně zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="ea90b-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="ea90b-105">Tuto možnost můžete nastavit tak, že nejprve synchronizujete službu Active Directory s Azure Active Directory a poté zaregistrujete zařízení systému Windows 10 s Azure AD a nastavíte je pro správu mobilních zařízení společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ea90b-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="ea90b-106">Následující video podrobně popisuje postup nastavení tohoto postupu pro nejběžnější scénář.</span><span class="sxs-lookup"><span data-stu-id="ea90b-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="ea90b-107">Nastavení zařízení připojených k doméně, která budou spravována společností Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="ea90b-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="ea90b-108">Chcete-li nastavit zařízení spojená s doménou organizace tak, aby měla užitek z možností poskytovaných službou Active Directory společnosti Azure, můžete kromě prostředí služby Active Directory implementovat také zařízení, která byla připojena k objektu **Hybrid Azure**.</span><span class="sxs-lookup"><span data-stu-id="ea90b-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="ea90b-109">Jedná se o zařízení, která jsou připojena k vaší budově v prostředí Active Directory a k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea90b-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="ea90b-110">Tato zařízení mohou být chráněna a spravována společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ea90b-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="ea90b-111">Dokončete následující kroky a vytvořte tak zařízení Windows 10 Hybrid Azure AD a spravováno společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="ea90b-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="ea90b-112">Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře služby Active Directory na Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure (Active Directory Connect), jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="ea90b-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="ea90b-113">Postup je pro společnost Microsoft 365 Business zcela stejný.</span><span class="sxs-lookup"><span data-stu-id="ea90b-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="ea90b-114">Než dokončíte krok 3 a povolíte, aby zařízení Windows 10 byla připojena k hybridním Azure, musíte zajistit splnění následujících předpokladů:</span><span class="sxs-lookup"><span data-stu-id="ea90b-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="ea90b-115">Používáte nejnovější verzi připojení k programu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ea90b-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="ea90b-116">Azure AD Connect synchronizovalo všechny počítačové objekty zařízení, které chcete použít jako hybridní Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ea90b-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="ea90b-117">Pokud objekty počítače patří do určitých organizačních jednotek, zkontrolujte, zda jsou tyto organizační jednotky nastaveny pro synchronizaci také v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ea90b-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="ea90b-118">Registrovat existující domény spojené se systémem Windows 10 na hybridní Azure AD vstoupil a zapsat je pro správu mobilních zařízení společností Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="ea90b-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="ea90b-119">Postupujte podle podrobných pokynů pro [konfiguraci hybridních zařízení připojených ke službě Active Directory](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="ea90b-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="ea90b-120">Tím umožníte synchronizaci v prostředí služby Active Directory s počítači se systémem Windows 10 a nastavíte jejich připravenost na mraky.</span><span class="sxs-lookup"><span data-stu-id="ea90b-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="ea90b-121">Chcete-li zapsat zařízení systému Windows 10 pro správu mobilních zařízení, naleznete pokyny v části [zápis zařízení Windows 10 s Intune pomocí zásad skupiny](https://go.microsoft.com/fwlink/p/?linkid=872871) .</span><span class="sxs-lookup"><span data-stu-id="ea90b-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="ea90b-122">Zásady skupiny lze nastavit na úrovni místního počítače nebo hromadných operací, na serveru řadiče domény je možné vytvořit toto nastavení zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="ea90b-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>