---
title: Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Přečtěte si, jak povolit Microsoft 365 chránit místní zařízení se systémem Active Directory připojená k windows 10.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593795"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="444e8-103">Jak nastavit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím plánu Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="444e8-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="444e8-104">Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business k ochraně zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="444e8-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="444e8-105">Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení připojená ke**službě Azure AD .</span><span class="sxs-lookup"><span data-stu-id="444e8-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="444e8-106">Tato zařízení jsou spojena s místní službou Active Directory i s Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="444e8-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="444e8-107">Toto video popisuje postup, jak nastavit tento pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.</span><span class="sxs-lookup"><span data-stu-id="444e8-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="444e8-108">1. Příprava na synchronizaci adresářů</span><span class="sxs-lookup"><span data-stu-id="444e8-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="444e8-109">Před synchronizací uživatelů a počítačů z místní domény služby Active Directory zkontrolujte, že [synchronizace adresářů s Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)najdete v části Příprava na synchronizaci adresářů .</span><span class="sxs-lookup"><span data-stu-id="444e8-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="444e8-110">Zejména:</span><span class="sxs-lookup"><span data-stu-id="444e8-110">In particular:</span></span>

   - <span data-ttu-id="444e8-111">Ujistěte se, že v adresáři neexistují žádné duplikáty pro následující atributy: **pošta**, **proxyAdresy**a **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="444e8-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="444e8-112">Tyto hodnoty musí být jedinečné a všechny duplikáty musí být odebrány.</span><span class="sxs-lookup"><span data-stu-id="444e8-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="444e8-113">Doporučujeme nakonfigurovat atribut **userPrincipalName** (UPN) pro každý místní uživatelský účet tak, aby odpovídal primární e-mailové adrese, která odpovídá licencovanému uživateli Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="444e8-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="444e8-114">Například: *mary.shelley@contoso.com* spíše než *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="444e8-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="444e8-115">Pokud doména služby Active Directory končí nesměrovatelnou příponou, jako *je místní* nebo *.lan*, namísto internetové horečné přípony, jako je *například .com* nebo *.org*, upravte příponu hlavního názvu místních uživatelských účtů, jak je popsáno v [části Příprava nesměrovatelné domény pro synchronizaci adresářů](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="444e8-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="444e8-116">2. Instalace a konfigurace Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="444e8-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="444e8-117">Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, nainstalujte Azure Active Directory Connect a nastavte synchronizaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="444e8-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="444e8-118">Další informace najdete v [tématu Nastavení synchronizace adresářů pro Office 365.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)</span><span class="sxs-lookup"><span data-stu-id="444e8-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="444e8-119">Kroky jsou přesně stejné pro Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="444e8-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="444e8-120">Při konfiguraci možností pro Azure AD Connect doporučujeme povolit **synchronizaci hesel**, **bezproblémové jednotné přihlašování**a funkci **zpětného zápisu hesla,** která je také podporována v Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="444e8-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="444e8-121">Zaškrtávací políčko Azure AD Connect zaškrtávací políčko jsou i další kroky pro zpětný zápis hesla.</span><span class="sxs-lookup"><span data-stu-id="444e8-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="444e8-122">Další informace naleznete v tématu [Postup: konfigurace zpětného zápisu hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="444e8-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="444e8-123">3. Konfigurace hybridního připojení azure reklam</span><span class="sxs-lookup"><span data-stu-id="444e8-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="444e8-124">Než povolíte, aby zařízení s Windows 10 byla připojena k hybridní azure ad, ujistěte se, že splňujete následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="444e8-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="444e8-125">Používáte nejnovější verzi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="444e8-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="444e8-126">Připojení Azure AD synchronizované všechny objekty počítače zařízení, které chcete být hybridní Azure AD připojil.</span><span class="sxs-lookup"><span data-stu-id="444e8-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="444e8-127">Pokud objekty počítače patří do konkrétních organizačních jednotek (OU), ujistěte se, že tyto organizační jednotky jsou nastaveny pro synchronizaci v připojení Azure AD také.</span><span class="sxs-lookup"><span data-stu-id="444e8-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="444e8-128">Chcete-li zaregistrovat existující zařízení s Windows 10 připojenou k doméně jako připojení hybridní azure ad, postupujte podle pokynů v [kurzu: Konfigurace hybridního připojení služby Azure Active Directory pro spravované domény](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="444e8-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="444e8-129">Tento hybrid umožňuje, aby se k počítačům se systémem Windows 10 připojily stávající místní služby Active Directory a připravily je na cloud.</span><span class="sxs-lookup"><span data-stu-id="444e8-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="444e8-130">4. Povolit automatickou registraci pro Windows 10</span><span class="sxs-lookup"><span data-stu-id="444e8-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="444e8-131">Pokud chcete automaticky zaregistrovat zařízení s Windows 10 pro správu mobilních zařízení v Intune, přečtěte si článku [Automatické registrace zařízení s Windows 10 pomocí zásad skupiny](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="444e8-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="444e8-132">Zásady skupiny můžete nastavit na úrovni místního počítače nebo pro hromadné operace, můžete použít šablony Konzoly pro správu zásad skupiny a šablony ADMX k vytvoření tohoto nastavení zásad skupiny v řadiči domény.</span><span class="sxs-lookup"><span data-stu-id="444e8-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="444e8-133">5. Konfigurace bezproblémového jednotného přihlášení</span><span class="sxs-lookup"><span data-stu-id="444e8-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="444e8-134">Bezproblémové jednotné přihlašuje automaticky uživatele do svých cloudových prostředků Microsoft 365, když používají podnikové počítače.</span><span class="sxs-lookup"><span data-stu-id="444e8-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="444e8-135">Jednoduše nasaďte jednu ze dvou možností zásad skupiny popsaných v [Azure Active Directory Bezproblémové jednotné přihlašování: Rychlý start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="444e8-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="444e8-136">Možnost **Zásady skupiny** neumožňuje uživatelům měnit jejich nastavení, zatímco možnost **Předvolby zásad skupiny** nastavuje hodnoty, ale také je ponechá uživatelsky konfigurovatelné.</span><span class="sxs-lookup"><span data-stu-id="444e8-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="444e8-137">6. Nastavení Windows Hello pro firmy</span><span class="sxs-lookup"><span data-stu-id="444e8-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="444e8-138">Windows Hello for Business nahrazuje hesla silným dvoufaktorovým ověřováním (2FA) pro přihlášení k místnímu počítači.</span><span class="sxs-lookup"><span data-stu-id="444e8-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="444e8-139">Jedním z faktorů je asymetrický pár klíčů a druhý je KÓD PIN nebo jiné místní gesto, jako je otisk prstu nebo rozpoznávání obličeje, pokud jej zařízení podporuje.</span><span class="sxs-lookup"><span data-stu-id="444e8-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="444e8-140">Pokud je to možné, doporučujeme nahradit hesla 2FA a Windows Hello pro firmy.</span><span class="sxs-lookup"><span data-stu-id="444e8-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="444e8-141">Chcete-li nakonfigurovat hybridní windows hello pro firmy, přečtěte si [vztah důvěryhodnosti hybridního klíče Windows Hello pro obchodní předpoklady](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="444e8-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="444e8-142">Potom postupujte podle pokynů v [části Konfigurovat hybridní nastavení důvěryhodnosti klíčů systému Windows Hello pro firmy](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span><span class="sxs-lookup"><span data-stu-id="444e8-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
