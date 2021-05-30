---
title: Upgrade na Microsoft 365 Business Premium z Microsoft 365 Business Standard
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Zjistěte rozdíl mezi Microsoft 365 Business Standard a Microsoft 365 Business Premium a tím, jak můžete upgradovat na Microsoft 365 Business Premium.
ms.openlocfilehash: 0968b877820590987f6f3ceca3efbd106b62cbd1
ms.sourcegitcommit: a05f61a291eb4595fa9313757a3815b7f217681d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/29/2021
ms.locfileid: "52705484"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a><span data-ttu-id="fda89-103">Upgrade na Microsoft 365 Business Premium z Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="fda89-103">Upgrade to Microsoft 365 Business Premium from Microsoft 365 Business Standard</span></span>

<span data-ttu-id="fda89-104">Pokud máte předplatné [Microsoft 365 pro firmy](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), například Microsoft 365 Business Standard, můžete snadno upgradovat na Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fda89-104">If you have a [Microsoft 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Microsoft 365 Business Standard, you can easily upgrade to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="fda89-105">Upgradujte na Microsoft 365 Business Premium, pokud chcete přidat:</span><span class="sxs-lookup"><span data-stu-id="fda89-105">Upgrade to Microsoft 365 Business Premium if you want to add:</span></span>

- <span data-ttu-id="fda89-106">Windows 10 Pro (pro počítače s Windows 8 nebo novějším)</span><span class="sxs-lookup"><span data-stu-id="fda89-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>

- <span data-ttu-id="fda89-107">Jednoduché ovládací prvky, které spravují obchodní data na zařízeních</span><span class="sxs-lookup"><span data-stu-id="fda89-107">Simple controls that manage business data on devices</span></span>

- <span data-ttu-id="fda89-108">Rozšířené možnosti zabezpečení</span><span class="sxs-lookup"><span data-stu-id="fda89-108">Advanced security capabilities.</span></span>
<span data-ttu-id="fda89-109">Další informace o Microsoft 365 Business Premium najdete [na Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="fda89-109">Find out more about Microsoft 365 Business Premium at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a><span data-ttu-id="fda89-110">Jaký je rozdíl mezi Microsoft 365 Business Standard a Microsoft 365 Business Premium?</span><span class="sxs-lookup"><span data-stu-id="fda89-110">What's the difference between Microsoft 365 Business Standard and Microsoft 365 Business Premium?</span></span>

<span data-ttu-id="fda89-111">Přidali jsme vedle sebe porovnání těchto dvou plánů s popisem Microsoft 365 Business Premium [služby.](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)</span><span class="sxs-lookup"><span data-stu-id="fda89-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Premium Service Description](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-begin"></a><span data-ttu-id="fda89-112">Než začnete</span><span class="sxs-lookup"><span data-stu-id="fda89-112">Before you begin</span></span>

- <span data-ttu-id="fda89-113">**Kdy se mám rozhodnout upgradovat?**</span><span class="sxs-lookup"><span data-stu-id="fda89-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="fda89-114">Upgrade je správná volba, když chcete upgradovat **všechny uživatele přiřazené** k jednomu plánu.</span><span class="sxs-lookup"><span data-stu-id="fda89-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="fda89-115">Když zvolíte upgrade, přechádí se všichni uživatelé plánu na jiný plán najednou.</span><span class="sxs-lookup"><span data-stu-id="fda89-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="fda89-116">Pokud nechcete upgradovat všechny přiřazené k jednomu plánu, kupte si licence pro nový plán [](../admin/manage/assign-licenses-to-users.md) (v tomto případě Microsoft 365 Business Premium) a přiřaďte tyto licence jednotlivě každému uživateli, kterého chcete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="fda89-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business Premium), and [assign those licenses individually](../admin/manage/assign-licenses-to-users.md) to each user that you want to upgrade.</span></span>

- <span data-ttu-id="fda89-117">**Některé doplňky můžou upgradu zabránit.** Pokud se pokusíte spustit upgrade a máte doplněk, který vám brání v pokračování, můžete ho nejdřív odebrat a později ho přidat zpátky, pokud ho budete dál potřebovat.</span><span class="sxs-lookup"><span data-stu-id="fda89-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span>

- <span data-ttu-id="fda89-118">**Pokud jste si předplatili svůj plán** Neexistuje přímočará cesta upgradu pro předplacené plány.</span><span class="sxs-lookup"><span data-stu-id="fda89-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="fda89-119">Budete vědět, jestli máte předplacený plán, protože jste plán nastavili pomocí ID produktu, které jste si koupili v obchodě.</span><span class="sxs-lookup"><span data-stu-id="fda89-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="fda89-120">Kontaktujte partnera, přejděte na Microsoft Store nebo počkejte, až vyprší platnost předplaceného plánu, a přejděte na nový plán.</span><span class="sxs-lookup"><span data-stu-id="fda89-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business-premium"></a><span data-ttu-id="fda89-121">Upgrade na Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="fda89-121">Upgrade to Microsoft 365 Business Premium</span></span>

1. <span data-ttu-id="fda89-122">Přihlaste se do Centra pro správu na adrese <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="fda89-122">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="fda89-123">Přejděte do navigačního podokna a vyberte **Fakturace** \> **vaše produkty**.</span><span class="sxs-lookup"><span data-stu-id="fda89-123">Go to the navigation pane and select **Billing** \> **Your products**.</span></span> <span data-ttu-id="fda89-124">Najděte si aktuální předplatné a vyberte ho, abyste si prohlíželi podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="fda89-124">Find your current subscription and select it to view the details.</span></span>

3. <span data-ttu-id="fda89-125">Na další stránce vyberte **Upgradovat**.</span><span class="sxs-lookup"><span data-stu-id="fda89-125">On the next page, select **Upgrade**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="fda89-126">Pokud se v aplikaci **Azure Active Directory** zobrazí zpráva s oznámením, že upgrade předplatného není podporován licencí založenými na skupině, můžete tuto možnost bez obav ignorovat, pokud nemáte velkou organizaci.</span><span class="sxs-lookup"><span data-stu-id="fda89-126">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="fda89-127">Organizace, které tuto možnost vybraly, budou vědět, že používají licencování založené na skupině.</span><span class="sxs-lookup"><span data-stu-id="fda89-127">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="fda89-128">Dále můžete zobrazit seznam plánů, na které můžete upgradovat.</span><span class="sxs-lookup"><span data-stu-id="fda89-128">Next, you can view a list of plans that you can upgrade to.</span></span> <span data-ttu-id="fda89-129">V takovém případě najděte Microsoft 365 Business Premium plán.</span><span class="sxs-lookup"><span data-stu-id="fda89-129">In this case, find the Microsoft 365 Business Premium plan.</span></span> <span data-ttu-id="fda89-130">Pokud chcete zobrazit všechny aplikace a služby, které jsou součástí tohoto plánu, můžete se posunout dolů.</span><span class="sxs-lookup"><span data-stu-id="fda89-130">You can scroll down if you want to see all the apps and services that are included with this plan.</span></span> <span data-ttu-id="fda89-131">V **Microsoft 365 Business Premium** vyberte **Upgradovat** a přidejte Microsoft 365 Business Premium do košíku.</span><span class="sxs-lookup"><span data-stu-id="fda89-131">Under **Microsoft 365 Business Premium**, select **Upgrade** to add Microsoft 365 Business Premium to your cart.</span></span>

5. <span data-ttu-id="fda89-132">V košíku:</span><span class="sxs-lookup"><span data-stu-id="fda89-132">In the cart:</span></span>

    1. <span data-ttu-id="fda89-133">Automaticky budeme zahrnovat licence pro všechny vaše aktuální uživatele.</span><span class="sxs-lookup"><span data-stu-id="fda89-133">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="fda89-134">Pokud potřebujete více nebo méně licencí, musíte tyto licence koupit a přiřadit [jednotlivě](../admin/manage/assign-licenses-to-users.md).</span><span class="sxs-lookup"><span data-stu-id="fda89-134">If you need more or fewer licenses, you need to [buy and assign those licenses individually](../admin/manage/assign-licenses-to-users.md).</span></span>  
    2. <span data-ttu-id="fda89-135">Můžete upravit, jak chcete platit: měsíčně nebo ročně.</span><span class="sxs-lookup"><span data-stu-id="fda89-135">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="fda89-136">Vyberte rozevírací nabídku, abyste se volby.</span><span class="sxs-lookup"><span data-stu-id="fda89-136">Select the drop-down menu to make your choice.</span></span>

6. <span data-ttu-id="fda89-137">Vyberte **Přejít na pokladnu,** kde uvidíte souhrn nákupu, včetně způsobu platby pro tento účet.</span><span class="sxs-lookup"><span data-stu-id="fda89-137">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="fda89-138">Pokud ho máte, můžete sem také přidat propagační kód.</span><span class="sxs-lookup"><span data-stu-id="fda89-138">You can also add a promo code here if you have one.</span></span>

7. <span data-ttu-id="fda89-139">Výběrem **možnosti Umístit objednávku** dokončete nákup.</span><span class="sxs-lookup"><span data-stu-id="fda89-139">Select **Place order** to complete your purchase.</span></span>\
<span data-ttu-id="fda89-140">Nastavení nových plánů služeb microsoftu trvá několik minut.</span><span class="sxs-lookup"><span data-stu-id="fda89-140">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="fda89-141">Pokud chcete zkontrolovat průběh, vyberte **Zkontrolovat stav upgradu**.</span><span class="sxs-lookup"><span data-stu-id="fda89-141">To check on progress, select **Check upgrade status**.</span></span>

8. <span data-ttu-id="fda89-142">Až bude plán hotový, budete možná muset v Centru pro správu provést některé další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="fda89-142">When your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="fda89-143">V navigačním podokně vyberte **Domů** a dokončete všechny další kroky nastavení.</span><span class="sxs-lookup"><span data-stu-id="fda89-143">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="fda89-144">Za licence, které už nepotřebujete, dostanete Microsoft 365 refundaci.</span><span class="sxs-lookup"><span data-stu-id="fda89-144">You'll receive a prorated refund for the Microsoft 365 licenses that you no longer need.</span></span> <span data-ttu-id="fda89-145">Bankovní účet nebo platební karta se vám naúčtuje zhruba dva dny po nastavení nového plánu.</span><span class="sxs-lookup"><span data-stu-id="fda89-145">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="fda89-146">Ochrana uživatelských zařízení a souborů</span><span class="sxs-lookup"><span data-stu-id="fda89-146">Protect user devices and files</span></span>

<span data-ttu-id="fda89-147">Teď, Microsoft 365 Business Premium licence byly přiřazeny, proveďte kroky, jak začít chránit zařízení a soubory.</span><span class="sxs-lookup"><span data-stu-id="fda89-147">Now that Microsoft 365 Business Premium licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="fda89-148">Budete používat některé nové možnosti, které jsou součástí navigačního podokna Centra pro správu.</span><span class="sxs-lookup"><span data-stu-id="fda89-148">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="fda89-149">V Centru pro správu v navigačním podokně přejděte na **Zásady** \> **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="fda89-149">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="fda89-150">Na stránce **Zásady zařízení** vyberte **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="fda89-150">On the **Device policies** page, select **Add**.</span></span>

3. <span data-ttu-id="fda89-151">V podokně **Přidat zásadu** pojmete zásadu (například Zamknout pracovní soubory) **a** v rozevíracím seznamu zvolte typ zásady.</span><span class="sxs-lookup"><span data-stu-id="fda89-151">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span>

    <span data-ttu-id="fda89-152">Můžete nastavit zásady aplikace pro ochranu souborů na zařízeních s Androidem a iPhone a Windows 10 a můžete nastavit zásady konfigurace zařízení pro zařízení vlastněná Windows 10 zařízeními.</span><span class="sxs-lookup"><span data-stu-id="fda89-152">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="fda89-153">Podrobnosti najdete v následujících odkazech:</span><span class="sxs-lookup"><span data-stu-id="fda89-153">See the following links for details:</span></span>

    - [<span data-ttu-id="fda89-154">Nastavení ochrany aplikací pro zařízení s Androidem nebo iOSem</span><span class="sxs-lookup"><span data-stu-id="fda89-154">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

    - [<span data-ttu-id="fda89-155">Nastavení ochrany aplikací pro zařízení s Windows 10</span><span class="sxs-lookup"><span data-stu-id="fda89-155">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

    - [<span data-ttu-id="fda89-156">Nastavení ochrany zařízení pro Windows 10 počítače</span><span class="sxs-lookup"><span data-stu-id="fda89-156">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

4. <span data-ttu-id="fda89-157">Po nastavení zásad můžete vy i vaši zaměstnanci nastavit zařízení:</span><span class="sxs-lookup"><span data-stu-id="fda89-157">After you set up policies, you and your employees can set up devices:</span></span>

    - <span data-ttu-id="fda89-158">Pokud vaše Windows zařízení ještě aktualizaci Windows Pro Creator, budete je muset upgradovat na Windows Pro [Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="fda89-158">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

    - <span data-ttu-id="fda89-159">Postup [pro Windows najdete v Windows](set-up-windows-devices.md) Windows zařízení pro Microsoft 365 Business Premium uživatele.</span><span class="sxs-lookup"><span data-stu-id="fda89-159">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span>

    - <span data-ttu-id="fda89-160">Postup pro telefony s [Androidem a iPhony najdete v tématu](set-up-mobile-devices.md) Microsoft 365 Business Premium mobilních zařízení pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="fda89-160">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span>