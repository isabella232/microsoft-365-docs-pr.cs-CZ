---
title: Přístup k místním prostředkům ze zařízení se službou Azure AD v Microsoft365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Přečtěte si, jak získat přístup k místním prostředkům, jako jsou obchodní aplikace, sdílené složky a tiskárny z Azure Active Directory se připojil y k windows 10 zařízení.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593227"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="72d26-103">Přístup k místním prostředkům ze zařízení se službou Azure AD v Microsoft365 Business</span><span class="sxs-lookup"><span data-stu-id="72d26-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="72d26-104">Každé zařízení s Windows 10, které je ve službě Azure Active Directory připojeno, má přístup ke všem cloudovým prostředkům, jako jsou aplikace Pro Office 365, a může být chráněno Microsoft365 Business.</span><span class="sxs-lookup"><span data-stu-id="72d26-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="72d26-105">Můžete také povolit přístup k místním prostředkům, jako je obchodní (LOB) aplikace, sdílené složky a tiskárny.</span><span class="sxs-lookup"><span data-stu-id="72d26-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="72d26-106">Pokud chcete povolit přístup, synchronizujte místní službu Active Directory s Azure Active Directory pomocí [azure ad connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="72d26-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="72d26-107">Další informace najdete v [tématu Úvod do správy zařízení ve službě Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="72d26-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="72d26-108">Kroky jsou také shrnuty v následujících částech.</span><span class="sxs-lookup"><span data-stu-id="72d26-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="72d26-109">Tento postup se vztahuje pouze na oauth a NTLM.</span><span class="sxs-lookup"><span data-stu-id="72d26-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="72d26-110">Protokol Kerberos není podporován.</span><span class="sxs-lookup"><span data-stu-id="72d26-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="72d26-111">Spuštění připojení Azure AD</span><span class="sxs-lookup"><span data-stu-id="72d26-111">Run Azure AD Connect</span></span>

<span data-ttu-id="72d26-112">Proveďte následující kroky, abyste umožnili zařízením ve službě Azure AD, která jsou připojena k Azure AD, přístup k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="72d26-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="72d26-113">Chcete-li synchronizovat uživatele, skupiny a kontakty z místní služby Active Directory do služby Azure Active Directory, spusťte Průvodce synchronizací adresářů a Azure AD Connect, jak je popsáno v [nastavení synchronizace adresářů pro Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="72d26-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="72d26-114">Po dokončení synchronizace adresářů zkontrolujte, zda jsou zařízení windows 10 vaší organizace připojena k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72d26-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="72d26-115">Tento krok se provádí individuálně na každém zařízení s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="72d26-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="72d26-116">Podrobnosti najdete v [tématu Nastavení zařízení s Windows pro uživatele Microsoft 365 Business.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="72d26-116">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="72d26-117">Jakmile jsou zařízení s Windows 10 připojena k Azure AD, každý uživatel musí restartovat svá zařízení a přihlásit se pomocí svých přihlašovacích údajů Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="72d26-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="72d26-118">Všechna zařízení mají nyní také přístup k místním prostředkům.</span><span class="sxs-lookup"><span data-stu-id="72d26-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="72d26-119">K získání přístupu k místním prostředkům pro zařízení připojená ke službě Azure AD nejsou nutné žádné další kroky.</span><span class="sxs-lookup"><span data-stu-id="72d26-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="72d26-120">Tato funkce je integrována do systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="72d26-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="72d26-121">Pokud máte v plánu přihlásit se k zařízení AADJ než metodu hesla, jako je PIN / Bio-metric prostřednictvím přihlášení přihlašovacího údaje WHFB a pak přístup k místním prostředkům (sdílené složky, tiskárny.. atd.), postupujte podlehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="72d26-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="72d26-122">Pokud vaše organizace není připravena k nasazení v konfiguraci zařízení se spojeným id Azure AD popsanou výše, zvažte nastavení konfigurace zařízení se spojenými s hybridní azure [službou Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="72d26-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="72d26-123">Důležité informace při připojení zařízení s Windows k Azure AD</span><span class="sxs-lookup"><span data-stu-id="72d26-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="72d26-124">Pokud bylo zařízení windows, ke kterému jste se připojili, dříve připojeno k doméně nebo v pracovní skupině, zvažte následující omezení:</span><span class="sxs-lookup"><span data-stu-id="72d26-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="72d26-125">Když se zařízení Azure AD připojí, vytvoří nového uživatele bez odkazování na existující profil.</span><span class="sxs-lookup"><span data-stu-id="72d26-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="72d26-126">Profily musí být přeneseny ručně.</span><span class="sxs-lookup"><span data-stu-id="72d26-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="72d26-127">Profil uživatele obsahuje informace, jako jsou oblíbené položky, místní soubory, nastavení prohlížeče a nastavení nabídky Start.</span><span class="sxs-lookup"><span data-stu-id="72d26-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="72d26-128">Nejlepším přístupem je najít nástroj třetí strany pro mapování existujících souborů a nastavení na nový profil.</span><span class="sxs-lookup"><span data-stu-id="72d26-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="72d26-129">Pokud zařízení používá objekty zásad skupiny (GPO), některé objekty zásad skupiny nemusí mít v Intune srovnatelného [poskytovatele konfiguračních služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP).</span><span class="sxs-lookup"><span data-stu-id="72d26-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="72d26-130">Spusťte [nástroj MMAT](https://www.microsoft.com/download/details.aspx?id=45520) a vyhledejte srovnatelné csp pro existující objekty zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="72d26-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="72d26-131">Uživatelé se nebudou moci ověřovat v aplikacích, které jsou závislé na ověřování služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="72d26-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="72d26-132">Vyhodnoťte starší aplikaci a zvažte aktualizaci na aplikaci, která používá moderní uvažování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="72d26-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="72d26-133">Zjišťování tiskárny služby Active Directory nebude fungovat.</span><span class="sxs-lookup"><span data-stu-id="72d26-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="72d26-134">Můžete poskytnout přímé cesty tiskárny pro všechny uživatele nebo použít [hybridní cloudový tisk](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="72d26-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
