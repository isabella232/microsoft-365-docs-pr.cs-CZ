---
title: Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Dozvíte se, jak získat přístup k prostorovým zdrojům, jako je například obchodní aplikace, sdílení souborů a tiskárny z Azure Active Directory do zařízení Windows 10.
ms.openlocfilehash: fdc1eca6913ba6af4f6b65691fdee2165e7c827e
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323389"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="5041c-103">Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="5041c-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="5041c-104">Všechna zařízení systému Windows 10, která jsou připojena ke službě Active Directory, mají přístup ke všem prostředkům založeným na cloudu, jako jsou například aplikace sady Office 365, a může být chráněna společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5041c-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="5041c-105">Můžete také povolit přístup k interním zdrojům, jako jsou obchodní aplikace (LOB), sdílení souborů a tiskárny.</span><span class="sxs-lookup"><span data-stu-id="5041c-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="5041c-106">Chcete-li umožnit přístup, použijte [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) k synchronizaci svých prostor služby Active Directory s Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5041c-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="5041c-107">Další informace naleznete v tématu [Úvod k správě zařízení v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="5041c-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="5041c-108">Tyto kroky jsou také shrnuty v následujících oddílech.</span><span class="sxs-lookup"><span data-stu-id="5041c-108">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="5041c-109">Spustit Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="5041c-109">Run Azure AD Connect</span></span>

<span data-ttu-id="5041c-110">Chcete-li umožnit přístup k prostředkům v rámci podniku, proveďte následující kroky, které umožní připojení k zařízením Azure AD vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="5041c-110">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="5041c-111">Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresářů a funkci Azure AD Connect, jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="5041c-111">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="5041c-112">Po dokončení synchronizace adresářů se přesvědčte, zda jsou zařízení systému Windows 10 v organizaci připojena k programu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5041c-112">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="5041c-113">Tento krok se provádí jednotlivě na každém zařízení se systémem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5041c-113">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="5041c-114">Podrobnosti naleznete v části [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="5041c-114">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="5041c-115">Jakmile jsou zařízení se systémem Windows 10 připojena k serveru Azure AD, musí každý uživatel restartovat svá zařízení a přihlásit se pomocí svých obchodních pověření společnosti Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5041c-115">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="5041c-116">Všechna zařízení mají nyní přístup i k prostředkům na místě.</span><span class="sxs-lookup"><span data-stu-id="5041c-116">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="5041c-117">K získání přístupu k prostředkům na místě pro zařízení spojená s Azure AD nejsou zapotřebí žádné další kroky.</span><span class="sxs-lookup"><span data-stu-id="5041c-117">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="5041c-118">Tato funkce je integrována do systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5041c-118">This functionality is built into Windows 10.</span></span> 
  
<span data-ttu-id="5041c-119">Pokud vaše organizace není připravena k nasazení ve výše popsané konfiguraci zařízení Azure AD, zvažte nastavení [Konfigurace zařízení připojené k hybridní síti Azure](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="5041c-119">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="5041c-120">Důležité informace o spojení zařízení se systémem Windows s Azure AD</span><span class="sxs-lookup"><span data-stu-id="5041c-120">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="5041c-121">Pokud se zařízení systému Windows, které jste připojili Azure-AD, dříve připojilo k doméně nebo v pracovní skupině, zvažte následující omezení:</span><span class="sxs-lookup"><span data-stu-id="5041c-121">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="5041c-122">Když se zařízení připojí k Azure AD, vytvoří nového uživatele bez odkazu na existující profil.</span><span class="sxs-lookup"><span data-stu-id="5041c-122">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="5041c-123">Profily je nutné migrovat ručně.</span><span class="sxs-lookup"><span data-stu-id="5041c-123">Profiles must be manually migrated.</span></span> <span data-ttu-id="5041c-124">Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start.</span><span class="sxs-lookup"><span data-stu-id="5041c-124">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="5041c-125">Nejlepším přístupem je najít nástroj jiného výrobce pro mapování existujících souborů a nastavení na nový profil.</span><span class="sxs-lookup"><span data-stu-id="5041c-125">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="5041c-126">Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune obdobu [zprostředkovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP).</span><span class="sxs-lookup"><span data-stu-id="5041c-126">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="5041c-127">Chcete-li vyhledat srovnatelné zprostředkovatele kryptografických služeb pro existující objekty GPO, spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .</span><span class="sxs-lookup"><span data-stu-id="5041c-127">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="5041c-128">Uživatelé nebudou moci provádět ověření u aplikací, které závisejí na ověřování služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5041c-128">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="5041c-129">Vyhodnoťte starší verzi aplikace a zvažte aktualizaci aplikace, která používá moderní ověřování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="5041c-129">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="5041c-130">Zjišťování tiskárny služby Active Directory nebude fungovat.</span><span class="sxs-lookup"><span data-stu-id="5041c-130">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="5041c-131">Můžete poskytnout přímé cesty k tiskárnám pro všechny uživatele nebo použít [hybridní shluk tisku](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="5041c-131">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
