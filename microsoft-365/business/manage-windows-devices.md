---
title: Povolení správy zařízení s Windows 10 s doménou microsoftem 365 pro firmy
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
description: Přečtěte si, jak v několika krocích povolit microsoftu 365 ochranu místních zařízení se systémem Windows 10 připojenými k adresáři A active Directory.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533779"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="3482b-103">Povolení správy zařízení s Windows 10 s doménou pomocí Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="3482b-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="3482b-104">Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="3482b-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="3482b-105">Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení spojené Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="3482b-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="3482b-106">Tato zařízení jsou připojena k místnímu službě Active Directory i k vašemu službě Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3482b-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="3482b-107">Toto video popisuje postup, jak nastavit tento scénář pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.</span><span class="sxs-lookup"><span data-stu-id="3482b-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="3482b-108">Než začnete, ujistěte se, že provedete tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="3482b-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="3482b-109">Synchronizujte uživatele s Azure AD pomocí služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3482b-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="3482b-110">Dokončete synchronizaci organizační jednotky Azure AD Connect (OU).</span><span class="sxs-lookup"><span data-stu-id="3482b-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="3482b-111">Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence k Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3482b-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="3482b-112">Postup naleznete v tématu [Synchronizace uživatelů domény](manage-domain-users.md) společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3482b-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="3482b-113">1. Ověření autority MDM v Intune</span><span class="sxs-lookup"><span data-stu-id="3482b-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="3482b-114">Přejděte na portal.azure.com a v horní části stránky vyhledejte Intune.</span><span class="sxs-lookup"><span data-stu-id="3482b-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="3482b-115">Na stránce Microsoft Intune vyberte **Registrace zařízení** a na stránce **Přehled** se ujistěte, že **autorita MDM** je **Intune**.</span><span class="sxs-lookup"><span data-stu-id="3482b-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="3482b-116">Pokud **autorita MDM** není **žádná**, klepněte na **autoritu MDM a** nastavte ji na **Intune**.</span><span class="sxs-lookup"><span data-stu-id="3482b-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="3482b-117">Pokud je **autorita MDM** **Microsoft Office 365**, přejděte na **Zařízení**  >  **pro registraci zařízení** a použijte dialogové okno Přidat **autoritu MDM** vpravo k přidání autority **Intune MDM** (dialogové okno **Přidat autoritu MDM je** k dispozici jenom v případě, že je **autorita MDM** nastavená na Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="3482b-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="3482b-118">2. Ověření, že azure ad je povolena pro připojení k počítačům</span><span class="sxs-lookup"><span data-stu-id="3482b-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="3482b-119">Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte **Azure Active Directory** (v seznamu **Centra pro správu** vyberte Zobrazit vše, pokud azure active directory není viditelná).</span><span class="sxs-lookup"><span data-stu-id="3482b-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="3482b-120">V **Centru pro správu Služby Active Directory Azure**přejděte na **Azure Active Directory** , zvolte **Zařízení** a potom **nastavení zařízení**.</span><span class="sxs-lookup"><span data-stu-id="3482b-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="3482b-121">Ověřit, že**uživatelé mohou připojit zařízení k Azure AD** je povolena</span><span class="sxs-lookup"><span data-stu-id="3482b-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="3482b-122">Chcete-li povolit všechny uživatele, nastavte hodnotu **Vše**.</span><span class="sxs-lookup"><span data-stu-id="3482b-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="3482b-123">Chcete-li povolit konkrétní uživatele, nastavte na **Hodnotu Vybrané,** která povolí určitou skupinu uživatelů.</span><span class="sxs-lookup"><span data-stu-id="3482b-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="3482b-124">Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="3482b-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="3482b-125">Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="3482b-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="3482b-126">3. Ověření, že azure ad je povolena pro MDM</span><span class="sxs-lookup"><span data-stu-id="3482b-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="3482b-127">Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte možnost **Endpoint Managemen**t (vyberte **Zobrazit vše,** pokud **endpoint Manager** není viditelný)</span><span class="sxs-lookup"><span data-stu-id="3482b-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="3482b-128">V **Centru pro správu Správce koncových bodů společnosti Microsoft**přejděte na **Položku**Automatické  >  **Windows**  >  registrace**systému**Windows  >  **Automatic Enrollment**zařízení .</span><span class="sxs-lookup"><span data-stu-id="3482b-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="3482b-129">Ověřte, zda je povolen obor uživatele MDM.</span><span class="sxs-lookup"><span data-stu-id="3482b-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="3482b-130">Chcete-li zaregistrovat všechny počítače, nastavte na **Vše,** abyste automaticky zaregistrovali všechny uživatelské počítače, které jsou připojeny k Azure AD a novým počítačům, když uživatelé přidají pracovní účet do Windows.</span><span class="sxs-lookup"><span data-stu-id="3482b-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="3482b-131">Chcete-li zaregistrovat počítače určité skupiny uživatelů, nastavte hodnotu **Některé.**</span><span class="sxs-lookup"><span data-stu-id="3482b-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="3482b-132">Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="3482b-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="3482b-133">Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="3482b-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="3482b-134">4. Vytvořte požadované zdroje</span><span class="sxs-lookup"><span data-stu-id="3482b-134">4. Create the required resources</span></span> 

<span data-ttu-id="3482b-135">Provádění požadovaných úloh pro [konfiguraci hybridního spojení Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) bylo zjednodušeno použitím rutiny [Initialize-SecMgmtHybirdDeviceEnrollment,](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) která se nachází v modulu [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3482b-135">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="3482b-136">Při vyvolání této rutiny vytvoří a nakonfiguruje požadovaný bod připojení služby a zásady skupiny.</span><span class="sxs-lookup"><span data-stu-id="3482b-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="3482b-137">Tento modul můžete nainstalovat vyvoláním následující z instance prostředí PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3482b-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="3482b-138">Doporučujeme nainstalovat tento modul na Windows Server se systémem Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3482b-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="3482b-139">Chcete-li vytvořit požadovaný bod připojení služby a zásady skupiny, vyvoláte rutinu [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="3482b-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="3482b-140">Při provádění tohoto úkolu budete potřebovat pověření globálního správce Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3482b-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="3482b-141">Až budete připraveni k vytvoření prostředků, vyvolat následující:</span><span class="sxs-lookup"><span data-stu-id="3482b-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="3482b-142">První příkaz naváže spojení s cloudem Microsoftu a po zobrazení výzvy zadejte přihlašovací údaje globálního správce Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3482b-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="3482b-143">5. Propojení zásad skupiny</span><span class="sxs-lookup"><span data-stu-id="3482b-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="3482b-144">V Konzole GPMC (Group Policy Management Console) klikněte pravým tlačítkem myši na místo, kde chcete zásadu propojit, a v místní nabídce vyberte Propojit existující objekt *zásad skupiny.*</span><span class="sxs-lookup"><span data-stu-id="3482b-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="3482b-145">Vyberte zásadu vytvořenou ve výše uvedeném kroku a klepněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="3482b-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="3482b-146">Získejte nejnovější šablony pro správu</span><span class="sxs-lookup"><span data-stu-id="3482b-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="3482b-147">Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , může to být způsobeno tím, že nemáte nainstalované kódY ADMX pro Systém Windows 10 verze 1803, verze 1809 nebo verze 1903.</span><span class="sxs-lookup"><span data-stu-id="3482b-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="3482b-148">Chcete-li tento problém vyřešit, postupujte takto (Poznámka: nejnovější MDM.admx je zpětně kompatibilní):</span><span class="sxs-lookup"><span data-stu-id="3482b-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="3482b-149">Ke stažení: [Šablony pro správu (.admx) pro Windows 10 Květen 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="3482b-149">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="3482b-150">Nainstalujte balíček do primárního řadiče domény (PDC).</span><span class="sxs-lookup"><span data-stu-id="3482b-150">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="3482b-151">Navigace v závislosti na verzi složky: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="3482b-151">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="3482b-152">Přejmenujte složku **Definice zásad** ve výše uvedené cestě k **policydefinition .**</span><span class="sxs-lookup"><span data-stu-id="3482b-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="3482b-153">Zkopírujte složku **PolicyDefinitions** do **souboru C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="3482b-153">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="3482b-154">Pokud máte v plánu použít centrální úložiště zásad pro celou doménu, přidejte obsah PolicyDefinitions tam.</span><span class="sxs-lookup"><span data-stu-id="3482b-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="3482b-155">Chcete-li, aby byla tato zásada k dispozici, restartujte primární řadič domény.</span><span class="sxs-lookup"><span data-stu-id="3482b-155">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="3482b-156">Tento postup bude fungovat i pro všechny budoucí verze.</span><span class="sxs-lookup"><span data-stu-id="3482b-156">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="3482b-157">V tomto okamžiku byste měli vidět zásady **Povolit automatické registrace MDM pomocí výchozích přihlašovacích údajů Azure AD** k dispozici.</span><span class="sxs-lookup"><span data-stu-id="3482b-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
