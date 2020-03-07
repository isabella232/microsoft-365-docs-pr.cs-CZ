---
title: Upgrade na Microsoft 365 Business z Office 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Seznamte se s rozdílem mezi Office 365 Business Premium a Microsoftem 365 Business a jak můžete upgradovat na Microsoft 365 Business.
ms.openlocfilehash: 2ec77d96bef288bd33e4f67b74f91550f388a2c1
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561414"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="57d93-103">Upgrade na Microsoft 365 Business z Office 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="57d93-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="57d93-104">Pokud máte [předplatné Office 365 pro firmy](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), například Office 365 Business Premium, můžete snadno upgradovat na Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="57d93-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="57d93-105">Pokud chcete přidat:</span><span class="sxs-lookup"><span data-stu-id="57d93-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="57d93-106">Windows 10 Pro (na počítače s Windows 8 nebo novějším)</span><span class="sxs-lookup"><span data-stu-id="57d93-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="57d93-107">Jednoduché ovládací prvky, které spravují obchodní data na zařízeních</span><span class="sxs-lookup"><span data-stu-id="57d93-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="57d93-108">Pokročilé možnosti zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="57d93-108">Advanced security capabilities.</span></span>
<span data-ttu-id="57d93-109">Další informace o Microsoft 365 Business na [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="57d93-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="57d93-110">Jaký je rozdíl mezi Office 365 Business Premium a Microsoftem 365 Business?</span><span class="sxs-lookup"><span data-stu-id="57d93-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="57d93-111">Do [popisu obchodní služby microsoftu 365](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)jsme přidali porovnání těchto dvou plánů souběžně.</span><span class="sxs-lookup"><span data-stu-id="57d93-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="57d93-112">Než začnete</span><span class="sxs-lookup"><span data-stu-id="57d93-112">Before you get started</span></span>

- <span data-ttu-id="57d93-113">**Kdy se mám rozhodnout pro upgrade?**</span><span class="sxs-lookup"><span data-stu-id="57d93-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="57d93-114">Upgrade je správná volba, pokud chcete upgradovat **všechny uživatele** přiřazené k jednomu plánu.</span><span class="sxs-lookup"><span data-stu-id="57d93-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="57d93-115">Když zvolíte upgrade, všichni uživatelé plánu přejdou na jiný plán současně.</span><span class="sxs-lookup"><span data-stu-id="57d93-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="57d93-116">Pokud nechcete upgradovat všechny přiřazené k jednomu plánu, kupte si licence pro nový plán (v tomto případě Microsoft 365 Business) a [přiřaďte tyto licence jednotlivě](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) každému uživateli, kterého chcete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="57d93-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="57d93-117">**Některé doplňky mohou bránit upgradu** Pokud se pokusíte spustit upgrade a máte doplněk, který vám brání v pokračování, můžete doplněk nejprve odebrat a později jej přidat zpět, pokud ho stále potřebujete.</span><span class="sxs-lookup"><span data-stu-id="57d93-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span> 
- <span data-ttu-id="57d93-118">**Pokud jste svůj plán předplatili** Neexistuje žádná přímá cesta upgradu pro předplacené plány.</span><span class="sxs-lookup"><span data-stu-id="57d93-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="57d93-119">Budete vědět, zda máte předplacený plán, protože jste plán nastavili pomocí ID produktu, které jste si možná zakoupili v obchodě.</span><span class="sxs-lookup"><span data-stu-id="57d93-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="57d93-120">Obraťte se na partnera, přejděte do Obchodu Microsoft Store nebo počkejte, až vyprší platnost předplaceného plánu, abyste přešli na nový plán.</span><span class="sxs-lookup"><span data-stu-id="57d93-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="57d93-121">Upgrade na Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="57d93-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="57d93-122">Kupte si licence podle následujících kroků v [novém Centru pro správu](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span><span class="sxs-lookup"><span data-stu-id="57d93-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="57d93-123">Přihlaste se <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>do centra pro správu na adrese .</span><span class="sxs-lookup"><span data-stu-id="57d93-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="57d93-124">Přejděte do navigačního podokna a vyberte **položku Fakturace** \> **produktů & služeb**.</span><span class="sxs-lookup"><span data-stu-id="57d93-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="57d93-125">Najděte si předplatné Office 365 a vyberte ho, abyste si zobrazili podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="57d93-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Snímek obrazovky ukazuje, jak najít a vybrat předplatné v Centru pro správu.](../media/FindYourSubscription.png)

3. <span data-ttu-id="57d93-127">Na další stránce vyberte **Upgradovat**.</span><span class="sxs-lookup"><span data-stu-id="57d93-127">On the next page, select **Upgrade**.</span></span> 

      ![Snímek obrazovky ukazuje, kde vybrat Upgrade v Centru pro správu.](../media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="57d93-129">Pokud se zobrazí zpráva, že **upgrade předplatného není ve službě Azure Active Directory podporován pomocí licencování na základě skupiny**, můžete to bez obav ignorovat, pokud nemáte velmi velkou organizaci.</span><span class="sxs-lookup"><span data-stu-id="57d93-129">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="57d93-130">Organizace, které tuto možnost zvolily, si budou uvědomit, že používají skupinové licencování.</span><span class="sxs-lookup"><span data-stu-id="57d93-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="57d93-131">Dále můžete zobrazit seznam plánů Office, na které můžete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="57d93-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="57d93-132">V takovém případě vyhledejte plán Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="57d93-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="57d93-133">Pokud chcete zobrazit všechny aplikace a služby Office, které jsou součástí tohoto plánu, můžete se posunout dolů.</span><span class="sxs-lookup"><span data-stu-id="57d93-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="57d93-134">V **části Microsoft 365 Business**vyberte **Upgrade** a přidejte microsoft 365 Business do košíku.</span><span class="sxs-lookup"><span data-stu-id="57d93-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="57d93-135">V košíku:</span><span class="sxs-lookup"><span data-stu-id="57d93-135">In the cart:</span></span>
    1. <span data-ttu-id="57d93-136">Automaticky zahrneme licence pro všechny vaše stávající uživatele.</span><span class="sxs-lookup"><span data-stu-id="57d93-136">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="57d93-137">Pokud potřebujete více nebo méně licencí, musíte [tyto licence zakoupit a přiřadit jednotlivě](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="57d93-137">If you need more or fewer licenses, you need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="57d93-138">Můžete upravit způsob platby: měsíčně nebo ročně.</span><span class="sxs-lookup"><span data-stu-id="57d93-138">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="57d93-139">Vyberte rozevírací nabídku, kterou si můžete vybrat.</span><span class="sxs-lookup"><span data-stu-id="57d93-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="57d93-140">Vyberte **Přejít na pokladnu,** kde uvidíte souhrn nákupu, včetně způsobu platby pro tento účet.</span><span class="sxs-lookup"><span data-stu-id="57d93-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="57d93-141">Můžete také přidat promo kód zde, pokud máte jeden.</span><span class="sxs-lookup"><span data-stu-id="57d93-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="57d93-142">Vyberte **Zadejte objednávku** k dokončení nákupu.</span><span class="sxs-lookup"><span data-stu-id="57d93-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="57d93-143">Nastavení nových plánů služeb společnosti Microsoft trvá několik minut.</span><span class="sxs-lookup"><span data-stu-id="57d93-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="57d93-144">Chcete-li zkontrolovat průběh, vyberte **možnost Zkontrolovat stav upgradu**.</span><span class="sxs-lookup"><span data-stu-id="57d93-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="57d93-145">Jakmile bude váš plán připravený, možná budete muset v Centru pro správu provést některé další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="57d93-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="57d93-146">V navigačním podokně vyberte **Domů,** abyste dokončili další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="57d93-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="57d93-147">Za licence Office 365, které už nepotřebujete, obdržíte poměrnou částku.</span><span class="sxs-lookup"><span data-stu-id="57d93-147">You'll receive a prorated refund for the Office 365 licenses that you no longer need.</span></span> <span data-ttu-id="57d93-148">Z vašeho bankovního účtu nebo kreditní karty se účtuje přibližně dva dny po nastavení nového plánu.</span><span class="sxs-lookup"><span data-stu-id="57d93-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="57d93-149">Ochrana uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="57d93-149">Protect user devices and files</span></span>

<span data-ttu-id="57d93-150">Teď, když byly přiřazeny licence Microsoft 365 Business, proveďte kroky k zahájení ochrany zařízení a souborů.</span><span class="sxs-lookup"><span data-stu-id="57d93-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="57d93-151">Budete používat některé nové možnosti zahrnuté v navigačním podokně Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="57d93-151">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="57d93-152">V Centru pro správu přejděte v navigačním podokně na **zásady** **zařízení** \> .</span><span class="sxs-lookup"><span data-stu-id="57d93-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="57d93-153">Na stránce **Zásady zařízení** vyberte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="57d93-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="57d93-154">V podokně **Přidat zásady** pojmenujte zásadu (například Zamknout pracovní soubory) a pak z rozevíracího seznamu zvolte **typ zásad.**</span><span class="sxs-lookup"><span data-stu-id="57d93-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span> 
    
    <span data-ttu-id="57d93-155">Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních se systémem Android a iPhone a také na Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností.</span><span class="sxs-lookup"><span data-stu-id="57d93-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="57d93-156">Podrobnosti naleznete na následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="57d93-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="57d93-157">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="57d93-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="57d93-158">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="57d93-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="57d93-159">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="57d93-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="57d93-160">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="57d93-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="57d93-161">Pokud vaše zařízení s Windows ještě nepoužívají aktualizaci Windows Pro Creator, budete je muset [upgradovat na aktualizaci Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="57d93-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="57d93-162">Postup pro zařízení s Windows najdete v tématu [Nastavení zařízení s Windows pro uživatele Microsoft365 Business.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="57d93-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="57d93-163">Postup pro telefony a iPhony s Androidem najdete v tématu [Nastavení mobilních zařízení pro uživatele Microsoft365 Business.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="57d93-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
