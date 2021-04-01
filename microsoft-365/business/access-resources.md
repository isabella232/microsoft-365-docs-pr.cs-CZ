---
title: Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Zjistěte, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny z zařízení s Windows 10 připojeného k Azure Active Directory.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445342"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="8a33e-103">Přístup k místním prostředkům ze zařízení připojeného k Azure AD v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="8a33e-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="8a33e-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8a33e-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="8a33e-105">Všechna zařízení s Windows 10, ke které je připojená služba Azure Active Directory, má přístup ke všem cloudovým prostředkům, jako jsou vaše aplikace Microsoft 365, a může být chráněno službou Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8a33e-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="8a33e-106">Můžete také povolit přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky souborů a tiskárny.</span><span class="sxs-lookup"><span data-stu-id="8a33e-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="8a33e-107">Pokud chcete povolit přístup, [použijte Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místní služby Active Directory s Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a33e-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="8a33e-108">Další informace najdete v tématu [Úvod ke správě zařízení v Azure Active Directory](/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="8a33e-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="8a33e-109">Tyto kroky jsou také shrnuty v následujících částech.</span><span class="sxs-lookup"><span data-stu-id="8a33e-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="8a33e-110">Spuštění služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8a33e-110">Run Azure AD Connect</span></span>

<span data-ttu-id="8a33e-111">Proveďte následující kroky, abyste zařízením připojeným k Azure AD vaší organizace umožnili přístup k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="8a33e-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="8a33e-112">Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v článku Nastavení synchronizace adresářů pro [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="8a33e-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>
    
2. <span data-ttu-id="8a33e-113">Po dokončení synchronizace adresářů se ujistěte, že jsou zařízení s Windows 10 vaší organizace připojená k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a33e-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="8a33e-114">Tento krok se provádí jednotlivě na každém zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8a33e-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="8a33e-115">Podrobnosti najdete v tématu Nastavení zařízení s Windows pro [uživatele Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="8a33e-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="8a33e-116">Jakmile jsou zařízení s Windows 10 připojená k Azure AD, musí každý uživatel restartovat svá zařízení a přihlásit se pomocí přihlašovacích údajů Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8a33e-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="8a33e-117">Všechna zařízení teď mají přístup i k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="8a33e-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="8a33e-118">K získání přístupu k místním prostředkům pro zařízení připojená k Azure AD nejsou potřeba žádné další kroky.</span><span class="sxs-lookup"><span data-stu-id="8a33e-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="8a33e-119">Tato funkce je integrovaná ve Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8a33e-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="8a33e-120">Pokud máte v plánu přihlásit se k jinému zařízení AADJ, než je metoda hesla, třeba PIN/Biometric přes přihlašovací údaje WHFB, a pak získat přístup k místním prostředkům (sdílené složky, tiskárny.). atd.), postupujte podle https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="8a33e-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="8a33e-121">Pokud vaše organizace není připravená nasadit v konfiguraci zařízení připojené k Azure AD popsané výše, zvažte nastavení konfigurace zařízení připojeného k hybridní službě [Azure AD.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="8a33e-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="8a33e-122">Důležité informace při připojení zařízení s Windows k Azure AD</span><span class="sxs-lookup"><span data-stu-id="8a33e-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="8a33e-123">Pokud zařízení s Windows, ke které jste připojili Azure-AD, bylo dříve připojené k doméně nebo v pracovní skupině, zvažte následující omezení:</span><span class="sxs-lookup"><span data-stu-id="8a33e-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="8a33e-124">Když se zařízení Azure AD připojí, vytvoří nového uživatele bez odkazu na existující profil.</span><span class="sxs-lookup"><span data-stu-id="8a33e-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="8a33e-125">Profily se musí migrovat ručně.</span><span class="sxs-lookup"><span data-stu-id="8a33e-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="8a33e-126">Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start.</span><span class="sxs-lookup"><span data-stu-id="8a33e-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="8a33e-127">Nejlepším přístupem je najít nástroj jiného výrobce, který namapuje existující soubory a nastavení na nový profil.</span><span class="sxs-lookup"><span data-stu-id="8a33e-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="8a33e-128">Pokud zařízení používá objekty Zásady skupiny (GPO), nemusí některé objekty zásad skupiny v Intune mít srovnatelného poskytovatele služeb konfigurace. [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers)</span><span class="sxs-lookup"><span data-stu-id="8a33e-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="8a33e-129">Spusťte nástroj [MMAT,](https://www.microsoft.com/download/details.aspx?id=45520) abyste našli srovnatelné csP pro stávající objekty zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="8a33e-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="8a33e-130">Uživatelé nemusí být schopni ověřit aplikace, které jsou závislé na ověřování služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a33e-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="8a33e-131">Vyhodnoťte starší aplikaci a zvažte aktualizaci na aplikaci, která používá moderní ověřování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="8a33e-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="8a33e-132">Zjišťování tiskárny ve službě Active Directory nebude fungovat.</span><span class="sxs-lookup"><span data-stu-id="8a33e-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="8a33e-133">Můžete zadat přímé cesty tiskárny pro všechny uživatele nebo použít [Univerzální tisk](/universal-print/).</span><span class="sxs-lookup"><span data-stu-id="8a33e-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="8a33e-134">Související články</span><span class="sxs-lookup"><span data-stu-id="8a33e-134">Related Articles</span></span>

[<span data-ttu-id="8a33e-135">Předpoklady pro Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8a33e-135">Prerequisites for Azure AD Connect</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
