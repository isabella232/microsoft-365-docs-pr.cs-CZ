---
title: Jak povolit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím Microsoftu 365 pro firmy
f1.keywords:
- CSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Zjistěte, jak povolit Microsoft 365 chránit místní zařízení s Windows 10 připojená ke službě Active Directory v pouhých několika krocích.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407072"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="5b872-103">Jak povolit, aby zařízení s Windows 10 připojená k doméně byla spravovaná prostřednictvím služby Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5b872-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="5b872-104">Pokud vaše organizace používá místní službu Windows Server Active Directory, můžete nastavit Microsoft 365 Business Premium tak, aby chránila vaše zařízení s Windows 10, a přitom udržovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="5b872-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="5b872-105">K nastavení této ochrany můžete implementovat hybridní zařízení připojená **k Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="5b872-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="5b872-106">Tato zařízení jsou připojená k vaší místní službě Active Directory a k Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b872-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="5b872-107">Toto video popisuje kroky nastavení pro nejběžnější scénář, který je podrobně popsaný v krocích popsaných v následujících krocích.</span><span class="sxs-lookup"><span data-stu-id="5b872-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="5b872-108">Než začnete, proveďte tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="5b872-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="5b872-109">Synchronizace uživatelů s Azure AD pomocí Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5b872-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="5b872-110">Dokončete synchronizaci organizační jednotky (OU) služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5b872-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="5b872-111">Ujistěte se, že všichni synchronizovaní uživatelé domény mají licence na Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5b872-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="5b872-112">Postup [najdete v tématu](manage-domain-users.md) Synchronizace uživatelů domény s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="5b872-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="5b872-113">1. Ověření autority MDM v Intune</span><span class="sxs-lookup"><span data-stu-id="5b872-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="5b872-114">Přejděte do [Správce koncových](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) bodů a na stránce Microsoft Intune vyberte Registrace zařízení a pak na stránce **Přehled** zkontrolujte, jestli je autorita **MDM** **Intune.**</span><span class="sxs-lookup"><span data-stu-id="5b872-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="5b872-115">Pokud **oprávnění MDM nemá** hodnotu **Žádné,** klikněte na autoritu **MDM** a nastavte ji na **Intune.**</span><span class="sxs-lookup"><span data-stu-id="5b872-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="5b872-116">Pokud je autorita **MDM** Microsoft Office  **365,** přejděte na Zařízení pro registraci zařízení a vpravo použijte dialog Přidat autoritu MDM k přidání autority MDM Intune (dialogové okno Přidat autoritu MDM je dostupné jenom v případě, že je autorita MDM nastavená na Microsoft Office  >   365).    </span><span class="sxs-lookup"><span data-stu-id="5b872-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="5b872-117">2. Ověření, že pro připojení k počítačům je povolená služba Azure AD</span><span class="sxs-lookup"><span data-stu-id="5b872-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="5b872-118">Přejděte do Centra pro správu v adresáři a v seznamu Centra pro správu vyberte Zobrazit vše, pokud není služba <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> Azure Active Directory viditelná.  </span><span class="sxs-lookup"><span data-stu-id="5b872-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="5b872-119">V Centru **pro správu Azure Active Directory** přejděte na Azure Active **Directory,** zvolte **Zařízení** a pak **Nastavení zařízení.**</span><span class="sxs-lookup"><span data-stu-id="5b872-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="5b872-120">Ověření,**že uživatelé mohou připojit zařízení k Azure AD** je povolené</span><span class="sxs-lookup"><span data-stu-id="5b872-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="5b872-121">Pokud chcete povolit všechny uživatele, nastavte **možnost Všechny.**</span><span class="sxs-lookup"><span data-stu-id="5b872-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="5b872-122">Pokud chcete povolit konkrétní uživatele, **nastavte možnost Selected (Vybráno),** aby se umožnila konkrétní skupina uživatelů.</span><span class="sxs-lookup"><span data-stu-id="5b872-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="5b872-123">Přidejte požadované uživatele domény synchronizované v Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="5b872-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="5b872-124">Výběrem **možnosti Vybrat** skupiny povolíte obor uživatele MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="5b872-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="5b872-125">3. Ověření, že je pro MDM povolený Azure AD</span><span class="sxs-lookup"><span data-stu-id="5b872-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="5b872-126">Přejděte do Centra pro správu at a vyberte Správce koncových bodů (vyberte Zobrazit vše, pokud není správce koncových <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> bodů viditelný).   </span><span class="sxs-lookup"><span data-stu-id="5b872-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="5b872-127">V Centru **pro správu Microsoft Endpoint Manageru** přejděte na **Zařízení,**  >  **do které Windows Windows**  >  **zamíská**  >  **automatickou registraci.**</span><span class="sxs-lookup"><span data-stu-id="5b872-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="5b872-128">Ověřte, jestli je povolený obor uživatele MDM.</span><span class="sxs-lookup"><span data-stu-id="5b872-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="5b872-129">Pokud chcete zaregistrovat všechny  počítače, nastavte možnost Vše tak, aby se při přidání pracovního účtu do Windows automaticky zaregistrovaly všechny uživatelské počítače připojené k Azure AD a nové počítače.</span><span class="sxs-lookup"><span data-stu-id="5b872-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="5b872-130">Pokud chcete **zaregistrovat** počítače konkrétní skupiny uživatelů, nastavte možnost Někteří.</span><span class="sxs-lookup"><span data-stu-id="5b872-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="5b872-131">Přidejte požadované uživatele domény synchronizované v Azure AD do [skupiny zabezpečení.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="5b872-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="5b872-132">Výběrem **možnosti Vybrat** skupiny povolíte obor uživatele MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="5b872-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="5b872-133">4. Vytvoření požadovaných zdrojů</span><span class="sxs-lookup"><span data-stu-id="5b872-133">4. Create the required resources</span></span> 

<span data-ttu-id="5b872-134">Provádění požadovaných úkolů pro konfiguraci hybridního spojení [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) se zjednodušila pomocí rutiny [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5b872-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="5b872-135">Když tuto rutinu vyvoláte, vytvoří a nakonfiguruje potřebný spojovací bod služby a zásady skupiny.</span><span class="sxs-lookup"><span data-stu-id="5b872-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="5b872-136">Tento modul můžete nainstalovat tak, že z instance PowerShellu vytáčíte následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="5b872-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="5b872-137">Doporučujeme tento modul nainstalovat na Windows Server, na který běží Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5b872-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="5b872-138">Pokud chcete vytvořit požadovaný spojovací bod služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="5b872-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="5b872-139">Při provádění tohoto úkolu budete potřebovat přihlašovací údaje globálního správce Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5b872-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="5b872-140">Až budete připravení vytvořit prostředky, vyvolalte tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="5b872-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="5b872-141">První příkaz vytvoří připojení ke cloudu Microsoftu a po zobrazení výzvy zadejte své přihlašovací údaje globálního správce Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5b872-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="5b872-142">5. Propojení Zásady skupiny</span><span class="sxs-lookup"><span data-stu-id="5b872-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="5b872-143">V konzole Zásady skupiny Management Console (GPMC) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad* skupiny.</span><span class="sxs-lookup"><span data-stu-id="5b872-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="5b872-144">Vyberte zásadu vytvořenou v výše uvedeném kroku a klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="5b872-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="5b872-145">Získejte nejnovější šablony pro správu</span><span class="sxs-lookup"><span data-stu-id="5b872-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="5b872-146">Pokud zásadu nevidíte, povolte automatickou registraci MDM pomocí výchozích přihlašovacích údajů **Azure AD,** může to být proto, že nemáte nainstalovaný ADMX pro Windows 10, verzi 1803 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="5b872-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="5b872-147">Pokud chcete tento problém vyřešit, postupujte takto (Poznámka: Nejnovější jazyk MDM.admx je zpětně kompatibilní):</span><span class="sxs-lookup"><span data-stu-id="5b872-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="5b872-148">Stáhnout: Šablony pro správu (.admx) pro Windows 10 – aktualizace z října [2020 (20H2)](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="5b872-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="5b872-149">Nainstalujte balíček v řadiči domény.</span><span class="sxs-lookup"><span data-stu-id="5b872-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="5b872-150">Přejděte do složky v závislosti na verzi šablon pro správu: **C:\Program Files (x86)\Microsoft Zásady skupiny\Windows 10 Aktualizace z října 2020 (20H2)**</span><span class="sxs-lookup"><span data-stu-id="5b872-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="5b872-151">**Přejmenujte složku Definice** zásad ve výše uvedené cestě na **PolicyMis.**</span><span class="sxs-lookup"><span data-stu-id="5b872-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="5b872-152">Zkopírujte **složku PolicySystems** do sdílené složky SYSVOL ve výchozím nastavení v umístění **C:\Windows\SYSVOL\domain\Policies.**</span><span class="sxs-lookup"><span data-stu-id="5b872-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="5b872-153">Pokud plánujete používat centrální úložiště zásad pro celou doménu, přidejte obsah zásad.</span><span class="sxs-lookup"><span data-stu-id="5b872-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="5b872-154">V případě, že máte několik řadičů domény, počkejte, až se funkce SYSVOL replikuje, aby zásady byly k dispozici.</span><span class="sxs-lookup"><span data-stu-id="5b872-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="5b872-155">Tento postup bude fungovat i pro všechny budoucí verze šablon pro správu.</span><span class="sxs-lookup"><span data-stu-id="5b872-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="5b872-156">V tomto okamžiku by se vám měla zobrazit zásada Povolit automatickou registraci MDM pomocí výchozích dostupných přihlašovacích údajů **Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="5b872-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
