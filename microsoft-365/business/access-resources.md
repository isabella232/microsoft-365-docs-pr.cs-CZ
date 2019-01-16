---
title: Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Zjistěte, jak získat přístup k místním prostředkům jako obchodními apps, sdílených souborů a tiskáren ze služby Active Directory Azure připojené zařízení Windows 10.
ms.openlocfilehash: 0a5d4b0828888fcb99676223000c446479f84ddc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982251"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="406eb-103">Přístup místního zdroje z Azure AD připojené zařízení v Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="406eb-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="406eb-p101">Jakékoli zařízení Windows 10 je Azure Active Directory připojen bude mít přístup ke všem prostředkům cloudové, například aplikací sady Office 365 a Microsoft 365 Business může být chráněna. Umožňuje také přístup k prostředkům místního jako řádku obchodní (LOB) aplikací, sdílené soubory a tiskárny, je třeba provést synchronizaci služby Active Directory v prostorách Azure Active Directory pomocí [Azure AD připojit](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). V tématu [Úvod do správy zařízení v Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) Další informace.</span><span class="sxs-lookup"><span data-stu-id="406eb-p101">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business. To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="406eb-107">Spustit Azure AD připojit</span><span class="sxs-lookup"><span data-stu-id="406eb-107">Run Azure AD Connect</span></span>

<span data-ttu-id="406eb-108">Postupujte takto Chcete-li povolit zařízení Azure AD, které jsou spojeny vaší organizaci získat přístup k prostředkům místního.</span><span class="sxs-lookup"><span data-stu-id="406eb-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="406eb-109">Synchronizace uživatelů, skupin a kontaktů z místní služby Active Directory do Azure Active Directory, spusťte Průvodce synchronizací adresáře a Azure AD připojit jako popsané v [Nastavení synchronizace adresáře služeb Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="406eb-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="406eb-p102">Po dokončení synchronizace adresáře, ujistěte se, že zařízení Windows 10 organizace jsou Azure AD, které jsou připojeny. Tento krok se provádí individuálně na každé zařízení Windows 10. Podrobnosti naleznete v tématu [Nastavení zařízení Windows pro uživatele Microsoft 365 Business](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="406eb-p102">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined. This step is done individually on each Windows 10 device. See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="406eb-p103">Jakmile zařízení Windows 10 jsou spojeny Azure AD, každý uživatel by měl restartovat jejich zařízení a přihlášení pomocí svých pověření Microsoft 365 Business. Všechna zařízení budou mít nyní přístup k místním prostředkům také.</span><span class="sxs-lookup"><span data-stu-id="406eb-p103">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials. All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="406eb-p104">Žádné další kroky jsou požadovány k získání přístupu k místním, že zařízení připojené prostředky k Azure AD. Toto je vestavěné funkce, které jsou k dispozici v systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="406eb-p104">No additional steps are required to get access to on-premise resources for Azure AD joined devices. This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="406eb-117">Pokud vaše organizace není připravena k nasazení v Azure AD připojen konfigurace zařízení popsané výše, zvažte nastavení [Konfigurace zařízení Joined hybridní Azure AD](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="406eb-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="406eb-118">Důležité informace při připojení zařízení Windows Azure AD</span><span class="sxs-lookup"><span data-stu-id="406eb-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="406eb-119">Jestliže používáte Azure AD připojit zařízení systému Windows, které bylo dříve připojeno k doméně nebo v pracovní skupině, je třeba zvážit následující omezení:</span><span class="sxs-lookup"><span data-stu-id="406eb-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="406eb-p105">Pokud se připojí zařízení Azure AD, vytvoří nového uživatele bez odkazování na existující profil. Chcete-li odstranit tento problém, profily nutné přenést ručně. Profil uživatele obsahuje informace jako oblíbené položky, místní soubory, nastavení prohlížeče, nastavení nabídky Start, atd. Nejlepším řešením je najít nástroj jiného výrobce mapovat existující soubory a nastavení do nového profilu</span><span class="sxs-lookup"><span data-stu-id="406eb-p105">When a device Azure AD joins, it creates a new user without referencing an existing profile. To fix this, profiles need to be manually migrated. A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>
    
- <span data-ttu-id="406eb-p106">Pokud zařízení používá objekty Zásady skupiny (GPO), některé objekty GPO nebude mít srovnatelné [Konfiguraci poskytovatele služeb](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) pro Intune. Spusťte [nástroj MMAT](https://www.microsoft.com/download/details.aspx?id=45520) najít srovnatelné CSP pro existující objekty zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="406eb-p106">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune. Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span> 
    
- <span data-ttu-id="406eb-p107">Uživatelé nebudou moci přihlásit k aplikacím, které závisí na ověřování služby Active Directory. Které se zabývají vyhodnotit pomocí starší verze aplikace a aktualizujte aplikaci používající moderní ověřování, pokud je to možné.</span><span class="sxs-lookup"><span data-stu-id="406eb-p107">Users will not be able to authenticate to applications that depend on Active Directory authentication. To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>
    
- <span data-ttu-id="406eb-p108">Active Directory tiskárny zjišťování nebude fungovat. Tento problém lze vyřešit, poskytují přímé tiskárny cesty pro všechny uživatele nebo využít [Hybridní Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="406eb-p108">Active Directory printer discovery will not work. To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
    

