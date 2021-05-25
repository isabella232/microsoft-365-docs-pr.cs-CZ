---
title: Povolte, aby Windows 10 zařízení připojená k doméně spravovaná Microsoft 365 pro firmy
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Zjistěte, jak Microsoft 365 v několika krocích chránit místní Windows 10 připojených ke službě Active Directory.
ms.openlocfilehash: ec80159bdceffd8a13d09a297a2acc1b78c9b1b3
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636080"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="d6913-103">Povolte, aby Windows 10 zařízení připojená k doméně spravovaná Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="d6913-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d6913-104">Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránil vaše zařízení Windows 10, a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="d6913-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="d6913-105">Pokud chcete nastavit tuto ochranu, můžete implementovat hybridní **zařízení připojená ke službě Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="d6913-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="d6913-106">Tato zařízení jsou připojená k místní službě Active Directory i k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6913-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

## <a name="watch-configure-hybrid-azure-active-directory-join"></a><span data-ttu-id="d6913-107">Přehrát: Konfigurace hybridního Azure Active Directory připojení</span><span class="sxs-lookup"><span data-stu-id="d6913-107">Watch: Configure Hybrid Azure Active Directory join</span></span>

<span data-ttu-id="d6913-108">Toto video popisuje postup, jak to nastavit pro nejběžnější scénář, který je také podrobně popsaný v následujících krocích.</span><span class="sxs-lookup"><span data-stu-id="d6913-108">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a><span data-ttu-id="d6913-109">Než začnete</span><span class="sxs-lookup"><span data-stu-id="d6913-109">Before you begin</span></span>

- <span data-ttu-id="d6913-110">Synchronizujte uživatele s Azure AD s Azure AD Připojení.</span><span class="sxs-lookup"><span data-stu-id="d6913-110">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="d6913-111">Dokončete synchronizaci azure AD Připojení organizační jednotky (OU).</span><span class="sxs-lookup"><span data-stu-id="d6913-111">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="d6913-112">Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d6913-112">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="d6913-113">Postup [najdete v tématu Synchronizace uživatelů](manage-domain-users.md) domény s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="d6913-113">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="d6913-114">1. Ověření autority MDM v Intune</span><span class="sxs-lookup"><span data-stu-id="d6913-114">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="d6913-115">Přejděte na [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) a na Microsoft Intune vyberte Registrace zařízení a potom na stránce **Přehled** zkontrolujte, že autoritou **MDM** je **Intune**.</span><span class="sxs-lookup"><span data-stu-id="d6913-115">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="d6913-116">Pokud **má autorita MDM** **hodnotu Žádná,** klikněte na autoritu **MDM a** nastavte ji na **Intune.**</span><span class="sxs-lookup"><span data-stu-id="d6913-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="d6913-117">Pokud je autorita **MDM** **Microsoft Office 365,** přejděte na Zařízení zaregistrovaná zařízení a pomocí dialogového okna Přidat autoritu MDM vpravo přidejte autoritu Intune  >   **MDM** (dialogové okno Přidat autoritu **MDM** je dostupné jenom v případě, že je autorita  **MDM** nastavená na Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="d6913-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="d6913-118">2. Ověřte, jestli je azure AD povolená pro připojení k počítačům</span><span class="sxs-lookup"><span data-stu-id="d6913-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="d6913-119">Přejděte do Centra pro správu a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> v seznamu Centra pro správu vyberte **Azure Active Directory** (v seznamu Centra pro správu vyberte Zobrazit vše, Azure Active Directory není **vidět).**</span><span class="sxs-lookup"><span data-stu-id="d6913-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="d6913-120">V Centru **Azure Active Directory pro správu** přejděte na **Azure Active Directory** , zvolte **Zařízení a** pak Nastavení **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="d6913-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="d6913-121">Ověření,**že se uživatelé smí připojit k azure AD, je** povolené</span><span class="sxs-lookup"><span data-stu-id="d6913-121">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="d6913-122">Pokud chcete povolit všechny uživatele, nastavte na **Vše**.</span><span class="sxs-lookup"><span data-stu-id="d6913-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="d6913-123">Pokud chcete povolit konkrétní uživatele, nastavte **vybranou** možnost tak, aby povolte určitou skupinu uživatelů.</span><span class="sxs-lookup"><span data-stu-id="d6913-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="d6913-124">Přidejte požadované uživatele domény synchronizované ve službě Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d6913-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="d6913-125">Pokud **chcete pro tuto skupinu** zabezpečení povolit rozsah uživatelů MDM, zvolte Vybrat skupiny.</span><span class="sxs-lookup"><span data-stu-id="d6913-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="d6913-126">3. Ověřte, jestli je pro MDM povolené Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6913-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="d6913-127">Přejděte do Centra pro správu a vyberte Správa koncových bodů t (vyberte Zobrazit vše, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Manager** není vidět)  </span><span class="sxs-lookup"><span data-stu-id="d6913-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="d6913-128">V Centru **Microsoft Endpoint Manager pro správu** přejděte na **Zařízení,**  >  **Windows**  >  **Windows registrace automatické**  >  **registrace.**</span><span class="sxs-lookup"><span data-stu-id="d6913-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="d6913-129">Ověřte, jestli je povolený obor uživatele MDM.</span><span class="sxs-lookup"><span data-stu-id="d6913-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="d6913-130">Pokud chcete zaregistrovat všechny  počítače, nastavte na Vše tak, aby se automaticky zaregistrovaly všechny uživatelské počítače, které jsou připojené k Azure AD, a nové počítače, když uživatelé přidávají pracovní účet do Windows.</span><span class="sxs-lookup"><span data-stu-id="d6913-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="d6913-131">Pokud chcete **zaregistrovat** počítače určité skupiny uživatelů, nastavte možnost Některé.</span><span class="sxs-lookup"><span data-stu-id="d6913-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="d6913-132">Přidejte požadované uživatele domény synchronizované ve službě Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d6913-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="d6913-133">Pokud **chcete pro tuto skupinu** zabezpečení povolit rozsah uživatelů MDM, zvolte Vybrat skupiny.</span><span class="sxs-lookup"><span data-stu-id="d6913-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="d6913-134">4. Vytvoření požadovaných zdrojů</span><span class="sxs-lookup"><span data-stu-id="d6913-134">4. Create the required resources</span></span> 

<span data-ttu-id="d6913-135">Provádění požadovaných úkolů pro konfiguraci hybridního připojení [k Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) se zjednodušil pomocí rutiny [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) která se nachází v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d6913-135">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="d6913-136">Když tuto rutinu vyvoláte, vytvoří a nakonfiguruje požadovaný spojovací bod služby a zásady skupiny.</span><span class="sxs-lookup"><span data-stu-id="d6913-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="d6913-137">Tento modul můžete nainstalovat tak, že z instance PowerShellu vyjádříte toto:</span><span class="sxs-lookup"><span data-stu-id="d6913-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="d6913-138">Doporučujeme nainstalovat tento modul na server Windows Azure AD Připojení.</span><span class="sxs-lookup"><span data-stu-id="d6913-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="d6913-139">Pokud chcete vytvořit požadovaný spojovací bod služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="d6913-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="d6913-140">Při provádění tohoto úkolu budete Microsoft 365 Business Premium přihlašovací údaje globálního správce.</span><span class="sxs-lookup"><span data-stu-id="d6913-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="d6913-141">Až budete připravení vytvořit zdroje, vyvolat následující:</span><span class="sxs-lookup"><span data-stu-id="d6913-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="d6913-142">První příkaz vytvoří spojení s cloudem Microsoftu a po zobrazení výzvy zadejte přihlašovací údaje Microsoft 365 Business Premium globálního správce.</span><span class="sxs-lookup"><span data-stu-id="d6913-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="d6913-143">5. Propojení Zásady skupiny</span><span class="sxs-lookup"><span data-stu-id="d6913-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="d6913-144">V Zásady skupiny Management Console (GPMC) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad* skupiny.</span><span class="sxs-lookup"><span data-stu-id="d6913-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="d6913-145">Vyberte zásadu vytvořenou ve výše uvedeném kroku a klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="d6913-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="d6913-146">Získání nejnovějších šablon pro správu</span><span class="sxs-lookup"><span data-stu-id="d6913-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="d6913-147">Pokud nevidíte zásadu Povolit automatickou registraci **MDM** pomocí výchozích přihlašovacích údajů Azure AD , může to být proto, že nemáte admx nainstalovaný pro Windows 10, verzi 1803 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="d6913-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="d6913-148">Pokud chcete tento problém vyřešit, postupujte takto (Poznámka: nejnovější mdm.admx je zpětně kompatibilní):</span><span class="sxs-lookup"><span data-stu-id="d6913-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="d6913-149">Stáhnout: [Šablony pro správu (.admx) Windows 10 aktualizace z října 2020 (20H2).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="d6913-149">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="d6913-150">Nainstalujte balíček na řadič domény.</span><span class="sxs-lookup"><span data-stu-id="d6913-150">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="d6913-151">V závislosti na verzi Šablon pro správu přejděte do **složky: C:\Program Files (x86)\Microsoft Zásady skupiny\Windows 10 Aktualizace z října 2020 (20H2).**</span><span class="sxs-lookup"><span data-stu-id="d6913-151">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="d6913-152">**Přejmenujte složku Definice** zásad ve výše uvedené cestě na **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="d6913-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="d6913-153">Zkopírujte **složku PolicyDefinitions** do sdílené složky SYSVOL ve výchozím nastavení umístěnou ve **složce C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="d6913-153">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="d6913-154">Pokud máte v plánu používat centrální úložiště zásad pro celou doménu, přidejte tam obsah PolicyDefinitions.</span><span class="sxs-lookup"><span data-stu-id="d6913-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="d6913-155">V případě, že máte několik řadičů domény, počkejte, až se funkce SYSVOL replikuje, aby byly zásady dostupné.</span><span class="sxs-lookup"><span data-stu-id="d6913-155">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="d6913-156">Tento postup bude fungovat i pro všechny budoucí verze šablon pro správu.</span><span class="sxs-lookup"><span data-stu-id="d6913-156">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="d6913-157">V tomto okamžiku byste měli mít možnost zobrazit zásadu Povolit automatickou registraci **MDM pomocí výchozích přihlašovacích údajů Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="d6913-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="d6913-158">Související obsah</span><span class="sxs-lookup"><span data-stu-id="d6913-158">Related content</span></span>

<span data-ttu-id="d6913-159">[Synchronizace uživatelů domény s Microsoft 365](manage-domain-users.md) (článek)</span><span class="sxs-lookup"><span data-stu-id="d6913-159">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>\
<span data-ttu-id="d6913-160">[Vytvoření skupiny v Centru pro správu](../admin/create-groups/create-groups.md) (článek)</span><span class="sxs-lookup"><span data-stu-id="d6913-160">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>\
<span data-ttu-id="d6913-161">[Kurz: Konfigurace hybridního Azure Active Directory připojení ke spravovaným doménám](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (článek)</span><span class="sxs-lookup"><span data-stu-id="d6913-161">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>