---
title: Upgrade na Microsoft 365 Business Premium z Microsoft 365 Business Standard
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
description: Seznamte se s rozdílem mezi Microsoft 365 Business Standard a Microsoft 365 Business Premium a jak můžete upgradovat na Microsoft 365 Business Premium.
ms.openlocfilehash: 20a4162f74a9cb0e943195a589fd2d964f773f48
ms.sourcegitcommit: eb3c7f473e8fe62624f52c9bb38dcd6a96fa58a3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/05/2020
ms.locfileid: "44045974"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a><span data-ttu-id="129a4-103">Upgrade na Microsoft 365 Business Premium z Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="129a4-103">Upgrade to Microsoft 365 Business Premium from Microsoft 365 Business Standard</span></span>

<span data-ttu-id="129a4-104">Pokud máte [předplatné Microsoft 365 pro firmy](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), například Microsoft 365 Business Standard, můžete snadno upgradovat na Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="129a4-104">If you have a [Microsoft 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Microsoft 365 Business Standard, you can easily upgrade to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="129a4-105">Pokud chcete přidat:</span><span class="sxs-lookup"><span data-stu-id="129a4-105">Upgrade to Microsoft 365 Business Premium if you want to add:</span></span>

- <span data-ttu-id="129a4-106">Windows 10 Pro (na počítače s Windows 8 nebo novějším)</span><span class="sxs-lookup"><span data-stu-id="129a4-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>

- <span data-ttu-id="129a4-107">Jednoduché ovládací prvky, které spravují obchodní data na zařízeních</span><span class="sxs-lookup"><span data-stu-id="129a4-107">Simple controls that manage business data on devices</span></span>

- <span data-ttu-id="129a4-108">Pokročilé možnosti zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="129a4-108">Advanced security capabilities.</span></span>
<span data-ttu-id="129a4-109">Další informace o Microsoft 365 Business Premium na [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="129a4-109">Find out more about Microsoft 365 Business Premium at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a><span data-ttu-id="129a4-110">Jaký je rozdíl mezi Microsoft 365 Business Standard a Microsoft 365 Business Premium?</span><span class="sxs-lookup"><span data-stu-id="129a4-110">What's the difference between Microsoft 365 Business Standard and Microsoft 365 Business Premium?</span></span>

<span data-ttu-id="129a4-111">Do [popisu služby Microsoft 365 Business Premium](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)jsme přidali porovnání těchto dvou plánů souběžně.</span><span class="sxs-lookup"><span data-stu-id="129a4-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Premium Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="129a4-112">Než začnete</span><span class="sxs-lookup"><span data-stu-id="129a4-112">Before you get started</span></span>

- <span data-ttu-id="129a4-113">**Kdy se mám rozhodnout pro upgrade?**</span><span class="sxs-lookup"><span data-stu-id="129a4-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="129a4-114">Upgrade je správná volba, pokud chcete upgradovat **všechny uživatele** přiřazené k jednomu plánu.</span><span class="sxs-lookup"><span data-stu-id="129a4-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="129a4-115">Když zvolíte upgrade, všichni uživatelé plánu přejdou na jiný plán současně.</span><span class="sxs-lookup"><span data-stu-id="129a4-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="129a4-116">Pokud nechcete upgradovat všechny přiřazené k jednomu plánu, kupte si licence pro nový plán (v tomto případě Microsoft 365 Business Premium) a [přiřaďte tyto licence jednotlivě](../admin/manage/assign-licenses-to-users.md) každému uživateli, kterého chcete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="129a4-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business Premium), and [assign those licenses individually](../admin/manage/assign-licenses-to-users.md) to each user that you want to upgrade.</span></span>

- <span data-ttu-id="129a4-117">**Některé doplňky mohou bránit upgradu** Pokud se pokusíte spustit upgrade a máte doplněk, který vám brání v pokračování, můžete doplněk nejprve odebrat a později jej přidat zpět, pokud ho stále potřebujete.</span><span class="sxs-lookup"><span data-stu-id="129a4-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span>

- <span data-ttu-id="129a4-118">**Pokud jste svůj plán předplatili** Neexistuje žádná přímá cesta upgradu pro předplacené plány.</span><span class="sxs-lookup"><span data-stu-id="129a4-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="129a4-119">Budete vědět, zda máte předplacený plán, protože jste plán nastavili pomocí ID produktu, které jste si možná zakoupili v obchodě.</span><span class="sxs-lookup"><span data-stu-id="129a4-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="129a4-120">Obraťte se na partnera, přejděte do Obchodu Microsoft Store nebo počkejte, až vyprší platnost předplaceného plánu, abyste přešli na nový plán.</span><span class="sxs-lookup"><span data-stu-id="129a4-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business-premium"></a><span data-ttu-id="129a4-121">Upgrade na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="129a4-121">Upgrade to Microsoft 365 Business Premium</span></span>

1. <span data-ttu-id="129a4-122">Přihlaste se <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>do centra pro správu na adrese .</span><span class="sxs-lookup"><span data-stu-id="129a4-122">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="129a4-123">Přejděte do navigačního podokna a vyberte **Fakturace** \> **produktů**.</span><span class="sxs-lookup"><span data-stu-id="129a4-123">Go to the navigation pane and select **Billing** \> **Your products**.</span></span> <span data-ttu-id="129a4-124">Najděte aktuální předplatné a vyberte ho, chcete-li zobrazit podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="129a4-124">Find your current subscription and select it to view the details.</span></span>

3. <span data-ttu-id="129a4-125">Na další stránce vyberte **Upgradovat**.</span><span class="sxs-lookup"><span data-stu-id="129a4-125">On the next page, select **Upgrade**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="129a4-126">Pokud se zobrazí zpráva, že **upgrade předplatného není ve službě Azure Active Directory podporován pomocí licencování na základě skupiny**, můžete to bez obav ignorovat, pokud nemáte velmi velkou organizaci.</span><span class="sxs-lookup"><span data-stu-id="129a4-126">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="129a4-127">Organizace, které tuto možnost zvolily, si budou uvědomit, že používají skupinové licencování.</span><span class="sxs-lookup"><span data-stu-id="129a4-127">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="129a4-128">Dále můžete zobrazit seznam plánů, na které můžete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="129a4-128">Next, you can view a list of plans that you can upgrade to.</span></span> <span data-ttu-id="129a4-129">V takovém případě vyhledejte plán Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="129a4-129">In this case, find the Microsoft 365 Business Premium plan.</span></span> <span data-ttu-id="129a4-130">Pokud chcete zobrazit všechny aplikace a služby, které jsou součástí tohoto plánu, můžete se posunout dolů.</span><span class="sxs-lookup"><span data-stu-id="129a4-130">You can scroll down if you want to see all the apps and services that are included with this plan.</span></span> <span data-ttu-id="129a4-131">V **části Microsoft 365 Business Premium**vyberte **Upgrade** a přidejte do košíku Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="129a4-131">Under **Microsoft 365 Business Premium**, select **Upgrade** to add Microsoft 365 Business Premium to your cart.</span></span>

5. <span data-ttu-id="129a4-132">V košíku:</span><span class="sxs-lookup"><span data-stu-id="129a4-132">In the cart:</span></span>

    1. <span data-ttu-id="129a4-133">Automaticky zahrneme licence pro všechny vaše stávající uživatele.</span><span class="sxs-lookup"><span data-stu-id="129a4-133">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="129a4-134">Pokud potřebujete více nebo méně licencí, musíte [tyto licence zakoupit a přiřadit jednotlivě](../admin/manage/assign-licenses-to-users.md).</span><span class="sxs-lookup"><span data-stu-id="129a4-134">If you need more or fewer licenses, you need to [buy and assign those licenses individually](../admin/manage/assign-licenses-to-users.md).</span></span>  
    2. <span data-ttu-id="129a4-135">Můžete upravit způsob platby: měsíčně nebo ročně.</span><span class="sxs-lookup"><span data-stu-id="129a4-135">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="129a4-136">Vyberte rozevírací nabídku, kterou si můžete vybrat.</span><span class="sxs-lookup"><span data-stu-id="129a4-136">Select the drop-down menu to make your choice.</span></span>

6. <span data-ttu-id="129a4-137">Vyberte **Přejít na pokladnu,** kde uvidíte souhrn nákupu, včetně způsobu platby pro tento účet.</span><span class="sxs-lookup"><span data-stu-id="129a4-137">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="129a4-138">Můžete také přidat promo kód zde, pokud máte jeden.</span><span class="sxs-lookup"><span data-stu-id="129a4-138">You can also add a promo code here if you have one.</span></span>

7. <span data-ttu-id="129a4-139">Vyberte **Zadejte objednávku** k dokončení nákupu.</span><span class="sxs-lookup"><span data-stu-id="129a4-139">Select **Place order** to complete your purchase.</span></span>\
<span data-ttu-id="129a4-140">Nastavení nových plánů služeb společnosti Microsoft trvá několik minut.</span><span class="sxs-lookup"><span data-stu-id="129a4-140">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="129a4-141">Chcete-li zkontrolovat průběh, vyberte **možnost Zkontrolovat stav upgradu**.</span><span class="sxs-lookup"><span data-stu-id="129a4-141">To check on progress, select **Check upgrade status**.</span></span>

8. <span data-ttu-id="129a4-142">Až bude plán připravený, možná budete muset v Centru pro správu provést některé další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="129a4-142">When your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="129a4-143">V navigačním podokně vyberte **Domů,** abyste dokončili další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="129a4-143">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="129a4-144">Za licence Microsoft 365, které už nepotřebujete, obdržíte poměrnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="129a4-144">You'll receive a prorated refund for the Microsoft 365 licenses that you no longer need.</span></span> <span data-ttu-id="129a4-145">Z vašeho bankovního účtu nebo kreditní karty se účtuje přibližně dva dny po nastavení nového plánu.</span><span class="sxs-lookup"><span data-stu-id="129a4-145">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="129a4-146">Ochrana uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="129a4-146">Protect user devices and files</span></span>

<span data-ttu-id="129a4-147">Teď, když byly přiřazeny licence Microsoft 365 Business Premium, proveďte kroky k zahájení ochrany zařízení a souborů.</span><span class="sxs-lookup"><span data-stu-id="129a4-147">Now that Microsoft 365 Business Premium licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="129a4-148">Budete používat některé nové možnosti zahrnuté v navigačním podokně Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="129a4-148">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="129a4-149">V Centru pro správu přejděte v navigačním podokně na **zásady** **zařízení** \> .</span><span class="sxs-lookup"><span data-stu-id="129a4-149">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="129a4-150">Na stránce **Zásady zařízení** vyberte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="129a4-150">On the **Device policies** page, select **Add**.</span></span>

3. <span data-ttu-id="129a4-151">V podokně **Přidat zásady** pojmenujte zásadu (například Zamknout pracovní soubory) a pak z rozevíracího seznamu zvolte **typ zásad.**</span><span class="sxs-lookup"><span data-stu-id="129a4-151">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span>

    <span data-ttu-id="129a4-152">Můžete nastavit zásady aplikací pro ochranu souborů na zařízeních se systémem Android a iPhone a také na Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení s Windows 10 vlastněná společností.</span><span class="sxs-lookup"><span data-stu-id="129a4-152">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="129a4-153">Podrobnosti naleznete na následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="129a4-153">See the following links for details:</span></span>

    - [<span data-ttu-id="129a4-154">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="129a4-154">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

    - [<span data-ttu-id="129a4-155">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="129a4-155">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

    - [<span data-ttu-id="129a4-156">Nastavení ochrany zařízení pro počítače s Windows 10</span><span class="sxs-lookup"><span data-stu-id="129a4-156">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

4. <span data-ttu-id="129a4-157">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="129a4-157">After you set up policies, you and your employees can set up devices:</span></span>

    - <span data-ttu-id="129a4-158">Pokud vaše zařízení s Windows ještě nepoužívají aktualizaci Windows Pro Creator, budete je muset [upgradovat na aktualizaci Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="129a4-158">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

    - <span data-ttu-id="129a4-159">Postup pro zařízení s Windows najdete v tématu [Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="129a4-159">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span>

    - <span data-ttu-id="129a4-160">Postup pro telefony a iPhony s Androidem najdete v tématu [Nastavení mobilních zařízení pro uživatele Microsoft 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="129a4-160">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span>