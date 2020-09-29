---
title: Přístup k místním prostředkům ze zařízení Azure AD-JOIN v Microsoft 365 Business
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
description: Přečtěte si, jak získat přístup k místním prostředkům, jako je podnikový podnik, sdílení souborů a tiskárny ze zařízení Azure Active Directory spojené s Windows 10.
ms.openlocfilehash: 2144268f5cbab67c39d5902622c61c0c35e6481c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295304"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="04fc8-103">Přístup k místním prostředkům ze zařízení Azure AD-JOIN v Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="04fc8-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="04fc8-104">Tento článek se týká Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="04fc8-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="04fc8-105">Všechna zařízení s Windows 10, která jsou spojená se službou Azure Active Directory, mají přístup ke všem cloudovým prostředkům, jako jsou aplikace Microsoft 365 a mohou být chráněny Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="04fc8-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="04fc8-106">Můžete taky povolit přístup k místním prostředkům, jako jsou podnikové aplikace (LOB), sdílené soubory a tiskárny.</span><span class="sxs-lookup"><span data-stu-id="04fc8-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="04fc8-107">Pokud chcete povolit přístup, použijte [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci místního adresáře Active Directory s Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04fc8-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="04fc8-108">Další informace najdete v tématu [Úvod do správy zařízení v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="04fc8-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="04fc8-109">Tento postup je také shrnut v následujících částech.</span><span class="sxs-lookup"><span data-stu-id="04fc8-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="04fc8-110">Spuštění služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="04fc8-110">Run Azure AD Connect</span></span>

<span data-ttu-id="04fc8-111">Provedením následujících kroků povolíte zařízením připojeným k Azure AD v organizaci přístup k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="04fc8-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="04fc8-112">Pokud chcete synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect způsobem popsaným v části [Nastavení synchronizace adresářů pro Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="04fc8-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="04fc8-113">Po dokončení synchronizace adresáře zkontrolujte, jestli jsou zařízení s Windows 10 ve vaší organizaci v Azure AD spojená.</span><span class="sxs-lookup"><span data-stu-id="04fc8-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="04fc8-114">Tento krok se provádí jednotlivě na každém zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="04fc8-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="04fc8-115">Podrobnosti najdete v tématu [nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="04fc8-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="04fc8-116">Jakmile se zařízení s Windows 10 připojí ke službě Azure AD, musí každý uživatel restartovat svoje zařízení a přihlásit se pomocí přihlašovacích údajů k Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="04fc8-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="04fc8-117">Všechna zařízení mají teď taky přístup k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="04fc8-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="04fc8-118">K získání přístupu k místním prostředkům pro zařízení s připojením Azure AD nejsou potřeba žádné další kroky.</span><span class="sxs-lookup"><span data-stu-id="04fc8-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="04fc8-119">Tato funkce je integrovaná ve Windows 10.</span><span class="sxs-lookup"><span data-stu-id="04fc8-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="04fc8-120">Pokud máte plány pro přihlášení k zařízení AADJ, jako je třeba PIN/bio-metric prostřednictvím WHFB přihlašovacích údajů, a pak přístup k místním prostředkům (sdílené položky, tiskárny.. atd.), postupujte https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="04fc8-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="04fc8-121">Pokud vaše organizace není připravená k nasazení v konfiguraci zařízení spojené s připojením k Azure AD, zvažte nastavení [Konfigurace hybridního zařízení se službou Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="04fc8-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="04fc8-122">Důležité informace o připojení zařízení se systémem Windows k Azure AD</span><span class="sxs-lookup"><span data-stu-id="04fc8-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="04fc8-123">Pokud bylo zařízení se systémem Windows, které jste připojili prostřednictvím služby Azure-AD dřív v doméně, nebo v pracovní skupině, zvažte následující omezení:</span><span class="sxs-lookup"><span data-stu-id="04fc8-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="04fc8-124">Když se zařízení Azure AD spojuje, vytvoří nového uživatele bez odkazu na existující profil.</span><span class="sxs-lookup"><span data-stu-id="04fc8-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="04fc8-125">Profily je nutné migrovat ručně.</span><span class="sxs-lookup"><span data-stu-id="04fc8-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="04fc8-126">Profil uživatele obsahuje informace, jako jsou oblíbené, místní soubory, nastavení prohlížeče a nastavení nabídky Start.</span><span class="sxs-lookup"><span data-stu-id="04fc8-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="04fc8-127">Nejlepším postupem je vyhledání nástroje třetí strany pro mapování existujících souborů a nastavení na nový profil.</span><span class="sxs-lookup"><span data-stu-id="04fc8-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="04fc8-128">Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune srovnatelného [poskytovatele služeb pro konfiguraci](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) .</span><span class="sxs-lookup"><span data-stu-id="04fc8-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="04fc8-129">K vyhledání srovnatelných CSP pro existující objekty GPO spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .</span><span class="sxs-lookup"><span data-stu-id="04fc8-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="04fc8-130">Uživatelé nebudou moct ověřovat v aplikaci, která závisí na ověřování služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04fc8-130">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="04fc8-131">Vyhodnoťte starší verzi aplikace a zvažte aktualizaci aplikace používající moderní ověřování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="04fc8-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="04fc8-132">Vyhledávání tiskáren Active Directory nefunguje.</span><span class="sxs-lookup"><span data-stu-id="04fc8-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="04fc8-133">Můžete poskytnout přímé tiskové cesty pro všechny uživatele nebo použít [hybridní cloudový tisk](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="04fc8-133">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
