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
description: Dozvíte se, jak získat přístup k prostorovým zdrojům, jako jsou například aplikace Business Apps, sdílení souborů a tiskárny z Azure Active Directory do zařízení Windows 10.
ms.openlocfilehash: 92e8ccb99dfece7687c25db84b81fc7bc7158d71
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574672"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="6f94c-103">Přístup k prostředkům v místě z zařízení připojeném Azure AD v Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6f94c-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="6f94c-104">Jakékoli zařízení systému Windows 10, které je připojené ke službě Active Directory, bude mít přístup ke všem cloumovým prostředkům, jako je například aplikace sady Office 365, a mohou být chráněny společností Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6f94c-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="6f94c-105">Chcete-li také povolit přístup k interaktivním prostředkům, jako jsou například aplikace Business (LOB), sdílení souborů a tiskárny, je nutné synchronizovat své prostory Active Directory s Azure Active Directory pomocí [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="6f94c-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="6f94c-106">Další informace naleznete [v tématu Úvod k nástroji Správa zařízení v Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .</span><span class="sxs-lookup"><span data-stu-id="6f94c-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="6f94c-107">Tyto kroky jsou také shrnuty v následujících oddílech.</span><span class="sxs-lookup"><span data-stu-id="6f94c-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="6f94c-108">Spustit Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="6f94c-108">Run Azure AD Connect</span></span>

<span data-ttu-id="6f94c-109">Chcete-li umožnit přístup k prostředkům v rámci podniku, proveďte následující kroky, které umožní připojení k zařízením Azure AD vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="6f94c-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="6f94c-110">Chcete-li synchronizovat uživatele, skupiny a kontakty z místního adresáře Active Directory na Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v [Nastavení synchronizace adresářů pro sadu Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="6f94c-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="6f94c-111">Po dokončení synchronizace adresářů se přesvědčte, zda jsou zařízení systému Windows 10 v organizaci připojena k programu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f94c-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="6f94c-112">Tento krok se provádí jednotlivě na každém zařízení se systémem Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6f94c-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="6f94c-113">Podrobnosti naleznete v části [nastavení zařízení systému Windows pro Microsoft 365 Business Users](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="6f94c-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="6f94c-114">Jakmile se zařízení se systémem Windows 10 připojí k programu Azure AD, měli by každý uživatel restartovat svá zařízení a přihlásit se pomocí svých obchodních pověření společnosti Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6f94c-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="6f94c-115">Všechna zařízení budou mít nyní přístup i k prostředkům na místě.</span><span class="sxs-lookup"><span data-stu-id="6f94c-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="6f94c-116">K získání přístupu k prostředkům na místě pro zařízení spojená s Azure AD nejsou zapotřebí žádné další kroky.</span><span class="sxs-lookup"><span data-stu-id="6f94c-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="6f94c-117">Toto je vestavěná funkce dostupná v systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6f94c-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="6f94c-118">Pokud vaše organizace není připravena k nasazení ve výše popsané konfiguraci zařízení Azure AD, zvažte nastavení [Konfigurace zařízení připojené k hybridní síti Azure](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="6f94c-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="6f94c-119">Důležité informace o připojení zařízení systému Windows k Azure AD</span><span class="sxs-lookup"><span data-stu-id="6f94c-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="6f94c-120">Pokud jste Azure AD, který se připojuje k zařízení systému Windows, které bylo dříve součástí domény nebo pracovní skupiny, je třeba zvážit následující omezení:</span><span class="sxs-lookup"><span data-stu-id="6f94c-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="6f94c-121">Když se zařízení připojí k Azure AD, vytvoří nového uživatele bez odkazu na existující profil.</span><span class="sxs-lookup"><span data-stu-id="6f94c-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="6f94c-122">Chcete-li tento problém odstranit, je třeba profily ručně migrovat.</span><span class="sxs-lookup"><span data-stu-id="6f94c-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="6f94c-123">Profil uživatele obsahuje informace jako oblíbené položky, místní soubory, nastavení prohlížeče, nastavení nabídky Start atd. Nejlepším přístupem je najít nástroj jiného výrobce pro mapování existujících souborů a nastavení na nový profil</span><span class="sxs-lookup"><span data-stu-id="6f94c-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="6f94c-124">Pokud zařízení používá objekty zásad skupiny (GPO), nemusí mít některé objekty GPO v Intune obdobu [zprostředkovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP).</span><span class="sxs-lookup"><span data-stu-id="6f94c-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="6f94c-125">Chcete-li vyhledat srovnatelné zprostředkovatele kryptografických služeb pro existující objekty GPO, spusťte [Nástroj mmat](https://www.microsoft.com/download/details.aspx?id=45520) .</span><span class="sxs-lookup"><span data-stu-id="6f94c-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="6f94c-126">Uživatelé nebudou moci provádět ověření u aplikací, které závisejí na ověřování služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6f94c-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="6f94c-127">Chcete-li se vypořádat s tímto vyhodnotím pomocí starší aplikace a zvažte aktualizaci aplikace, která používá moderní ověřování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="6f94c-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="6f94c-128">Zjišťování tiskárny služby Active Directory nebude funkční.</span><span class="sxs-lookup"><span data-stu-id="6f94c-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="6f94c-129">Chcete-li tento problém vyřešit, zadejte přímé cesty k tiskárnám pro všechny uživatele nebo využijte [hybridní tisk shluku](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="6f94c-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
