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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564927"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="b927b-103">Povolení správy zařízení s Windows 10 s doménou pomocí Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b927b-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="b927b-104">Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.</span><span class="sxs-lookup"><span data-stu-id="b927b-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="b927b-105">Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení spojené Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="b927b-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="b927b-106">Tato zařízení jsou připojena k místnímu službě Active Directory i k vašemu službě Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b927b-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="b927b-107">Toto video popisuje postup, jak nastavit tento scénář pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.</span><span class="sxs-lookup"><span data-stu-id="b927b-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="b927b-108">Než začnete, ujistěte se, že provedete tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="b927b-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="b927b-109">Synchronizujte uživatele s Azure AD pomocí služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b927b-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="b927b-110">Dokončete synchronizaci organizační jednotky Azure AD Connect (OU).</span><span class="sxs-lookup"><span data-stu-id="b927b-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="b927b-111">Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence k Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b927b-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b927b-112">Postup naleznete v tématu [Synchronizace uživatelů domény](manage-domain-users.md) společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b927b-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="b927b-113">1. Ověření autority MDM v Intune</span><span class="sxs-lookup"><span data-stu-id="b927b-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="b927b-114">Přejděte na portal.azure.com a v horní části stránky vyhledejte Intune.</span><span class="sxs-lookup"><span data-stu-id="b927b-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="b927b-115">Na stránce Microsoft Intune vyberte **Registrace zařízení** a na stránce **Přehled** se ujistěte, že **autorita MDM** je **Intune**.</span><span class="sxs-lookup"><span data-stu-id="b927b-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="b927b-116">Pokud **autorita MDM** není **žádná**, klepněte na **autoritu MDM a** nastavte ji na **Intune**.</span><span class="sxs-lookup"><span data-stu-id="b927b-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="b927b-117">Pokud je **autorita MDM** **Microsoft Office 365**, přejděte na **Zařízení**  >  **pro registraci zařízení** a použijte dialogové okno Přidat **autoritu MDM** vpravo k přidání autority **Intune MDM** (dialogové okno **Přidat autoritu MDM je** k dispozici jenom v případě, že je **autorita MDM** nastavená na Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="b927b-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="b927b-118">2. Ověření, že azure ad je povolena pro připojení k počítačům</span><span class="sxs-lookup"><span data-stu-id="b927b-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="b927b-119">Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte **Azure Active Directory** (v seznamu **Centra pro správu** vyberte Zobrazit vše, pokud azure active directory není viditelná).</span><span class="sxs-lookup"><span data-stu-id="b927b-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="b927b-120">V **Centru pro správu Služby Active Directory Azure**přejděte na **Azure Active Directory** , zvolte **Zařízení** a potom **nastavení zařízení**.</span><span class="sxs-lookup"><span data-stu-id="b927b-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="b927b-121">Ověřit, že**uživatelé mohou připojit zařízení k Azure AD** je povolena</span><span class="sxs-lookup"><span data-stu-id="b927b-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="b927b-122">Chcete-li povolit všechny uživatele, nastavte hodnotu **Vše**.</span><span class="sxs-lookup"><span data-stu-id="b927b-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="b927b-123">Chcete-li povolit konkrétní uživatele, nastavte na **Hodnotu Vybrané,** která povolí určitou skupinu uživatelů.</span><span class="sxs-lookup"><span data-stu-id="b927b-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="b927b-124">Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="b927b-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="b927b-125">Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="b927b-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="b927b-126">3. Ověření, že azure ad je povolena pro MDM</span><span class="sxs-lookup"><span data-stu-id="b927b-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="b927b-127">Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte možnost **Endpoint Managemen**t (vyberte **Zobrazit vše,** pokud **endpoint Manager** není viditelný)</span><span class="sxs-lookup"><span data-stu-id="b927b-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="b927b-128">V **Centru pro správu Správce koncových bodů společnosti Microsoft**přejděte na **Položku**Automatické  >  **Windows**  >  registrace**systému**Windows  >  **Automatic Enrollment**zařízení .</span><span class="sxs-lookup"><span data-stu-id="b927b-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="b927b-129">Ověřte, zda je povolen obor uživatele MDM.</span><span class="sxs-lookup"><span data-stu-id="b927b-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="b927b-130">Chcete-li zaregistrovat všechny počítače, nastavte na **Vše,** abyste automaticky zaregistrovali všechny uživatelské počítače, které jsou připojeny k Azure AD a novým počítačům, když uživatelé přidají pracovní účet do Windows.</span><span class="sxs-lookup"><span data-stu-id="b927b-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="b927b-131">Chcete-li zaregistrovat počítače určité skupiny uživatelů, nastavte hodnotu **Některé.**</span><span class="sxs-lookup"><span data-stu-id="b927b-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="b927b-132">Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="b927b-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="b927b-133">Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="b927b-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="b927b-134">4. Nastavení spojovacího bodu služby (SCP)</span><span class="sxs-lookup"><span data-stu-id="b927b-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="b927b-135">Tyto kroky jsou zjednodušeny [z konfigurace hybridního spojení Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="b927b-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="b927b-136">Chcete-li provést kroky, které potřebujete k použití Azure AD Connect a vašich globálních administrátorů Microsoft 365 Business Premium a hesel pro správce služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b927b-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="b927b-137">Spusťte Azure AD Connect a pak vyberte **Konfigurovat**.</span><span class="sxs-lookup"><span data-stu-id="b927b-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="b927b-138">Na stránce **Další úkoly** vyberte **Konfigurovat možnosti zařízení**a pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="b927b-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="b927b-139">Na stránce **Přehled** vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="b927b-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="b927b-140">Na stránce **Připojení k Azure AD** zadejte přihlašovací údaje globálního správce pro Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b927b-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="b927b-141">Na stránce **Možnosti zařízení** vyberte **Konfigurovat hybridní spojení Azure AD**a pak vyberte **Další**.</span><span class="sxs-lookup"><span data-stu-id="b927b-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="b927b-142">Na stránce **SCP** pro každou doménovou strukturu, ve které chcete azure ad connect nakonfigurovat SCP, proveďte následující kroky a pak vyberte **Další**:</span><span class="sxs-lookup"><span data-stu-id="b927b-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="b927b-143">Zaškrtněte políčko vedle názvu doménové struktury.</span><span class="sxs-lookup"><span data-stu-id="b927b-143">Check the box beside the forest name.</span></span> <span data-ttu-id="b927b-144">Doménová struktura by měla být název domény služby AD.</span><span class="sxs-lookup"><span data-stu-id="b927b-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="b927b-145">Ve sloupci **Ověřovací služba** otevřete rozevírací seznam a vyberte odpovídající název domény (měla by existovat pouze jedna možnost).</span><span class="sxs-lookup"><span data-stu-id="b927b-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="b927b-146">Vyberte **Přidat** a zadejte pověření správce domény.</span><span class="sxs-lookup"><span data-stu-id="b927b-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="b927b-147">Na stránce **Operační systémy Zařízení** vyberte jenom zařízení připojená k Windows 10 nebo novějším doménovým systémům.</span><span class="sxs-lookup"><span data-stu-id="b927b-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="b927b-148">Na stránce **Připraveno ke konfiguraci** vyberte **Konfigurovat**.</span><span class="sxs-lookup"><span data-stu-id="b927b-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="b927b-149">Na stránce **Konfigurace dokončení** vyberte **Exit**.</span><span class="sxs-lookup"><span data-stu-id="b927b-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="b927b-150">5. Vytvoření objektu zásad skupiny pro registraci Intune – metoda ADMX</span><span class="sxs-lookup"><span data-stu-id="b927b-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="b927b-151">Použít. soubor šablony ADMX.</span><span class="sxs-lookup"><span data-stu-id="b927b-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="b927b-152">Přihlaste se k serveru AD, vyhledejte a otevřete **Server Manager**  >  **Tools**  >  **správu zásad skupiny**Nástroje správce serveru .</span><span class="sxs-lookup"><span data-stu-id="b927b-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="b927b-153">Vyberte název domény v části **Domény** a vyberte položku **Nový**klepnutím pravým tlačítkem myši na **položku Objekty zásad skupiny** .</span><span class="sxs-lookup"><span data-stu-id="b927b-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="b927b-154">Pojmenujte nový objekt zásad skupiny, například "*Cloud_Enrollment*" a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="b927b-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="b927b-155">Klepněte pravým tlačítkem myši na nový objekt zásad skupiny v části **Objekty zásad skupiny** a vyberte příkaz **Upravit**.</span><span class="sxs-lookup"><span data-stu-id="b927b-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="b927b-156">V **Editoru správy zásad skupiny** **přejděte**na  >  **položku Šablony správy zásad**konfigurace  >  **Administrative Templates**  >  **počítače, součásti systému Windows**  >  **MDM**.</span><span class="sxs-lookup"><span data-stu-id="b927b-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="b927b-157">Klikněte pravým tlačítkem myši na **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD** a pak vyberte **povoleno**  >  **OK**.</span><span class="sxs-lookup"><span data-stu-id="b927b-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="b927b-158">Zavřete okno editoru.</span><span class="sxs-lookup"><span data-stu-id="b927b-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b927b-159">Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , přečtěte [si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si nejnovější šablony pro správu](#get-the-latest-administrative-templates).</span><span class="sxs-lookup"><span data-stu-id="b927b-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="b927b-160">6. Nasazení zásad skupiny</span><span class="sxs-lookup"><span data-stu-id="b927b-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="b927b-161">Ve Správci serveru v části **Domains** > Group Policy objects vyberte objekt zásad skupiny z výše uvedeného kroku 3, například "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="b927b-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="b927b-162">Vyberte kartu **Obor** pro objekt zásad skupiny.</span><span class="sxs-lookup"><span data-stu-id="b927b-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="b927b-163">Na kartě Obor objektu zásad skupiny klikněte pravým tlačítkem myši na odkaz na doménu v části **Odkazy**.</span><span class="sxs-lookup"><span data-stu-id="b927b-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="b927b-164">Chcete-li na obrazovce potvrzení nasadit objekt zásad skupiny, vyberte možnost **Vynuceno** a potom **OK.**</span><span class="sxs-lookup"><span data-stu-id="b927b-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="b927b-165">Získejte nejnovější šablony pro správu</span><span class="sxs-lookup"><span data-stu-id="b927b-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="b927b-166">Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , může to být způsobeno tím, že nemáte nainstalované kódY ADMX pro Systém Windows 10 verze 1803, verze 1809 nebo verze 1903.</span><span class="sxs-lookup"><span data-stu-id="b927b-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="b927b-167">Chcete-li tento problém vyřešit, postupujte takto (Poznámka: nejnovější MDM.admx je zpětně kompatibilní):</span><span class="sxs-lookup"><span data-stu-id="b927b-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="b927b-168">Ke stažení: [Šablony pro správu (.admx) pro Windows 10 Květen 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="b927b-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="b927b-169">Nainstalujte balíček do primárního řadiče domény (PDC).</span><span class="sxs-lookup"><span data-stu-id="b927b-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="b927b-170">Navigace v závislosti na verzi složky: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="b927b-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="b927b-171">Přejmenujte složku **Definice zásad** ve výše uvedené cestě k **policydefinition .**</span><span class="sxs-lookup"><span data-stu-id="b927b-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="b927b-172">Zkopírujte složku **PolicyDefinitions** do **souboru C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="b927b-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="b927b-173">Pokud máte v plánu použít centrální úložiště zásad pro celou doménu, přidejte obsah PolicyDefinitions tam.</span><span class="sxs-lookup"><span data-stu-id="b927b-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="b927b-174">Chcete-li, aby byla tato zásada k dispozici, restartujte primární řadič domény.</span><span class="sxs-lookup"><span data-stu-id="b927b-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="b927b-175">Tento postup bude fungovat i pro všechny budoucí verze.</span><span class="sxs-lookup"><span data-stu-id="b927b-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="b927b-176">V tomto okamžiku byste měli vidět zásady **Povolit automatické registrace MDM pomocí výchozích přihlašovacích údajů Azure AD** k dispozici.</span><span class="sxs-lookup"><span data-stu-id="b927b-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

