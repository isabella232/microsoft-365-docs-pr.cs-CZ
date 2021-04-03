---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Ověřte nastavení ochrany aplikací Microsoft 365 Business Premium na zařízeních s Windows 10 a ověřte, že uživatelé nemohou kopírovat data společnosti do osobních souborů nebo nespravovaných aplikací.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579856"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="a03fb-103">Ověření nastavení ochrany aplikací na počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="a03fb-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="a03fb-104">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních</span><span class="sxs-lookup"><span data-stu-id="a03fb-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="a03fb-105">Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="a03fb-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="a03fb-106">Pokud jste  zapnuli nastavení Zabránit uživatelům v kopírování firemních dat do osobních souborů a přinutili je ukládat pracovní soubory na **OneDrive pro** firmy pro zařízení vlastněná společností, můžete to zkontrolovat na zařízení uživatele po připojení k Azure AD a přihlášení.</span><span class="sxs-lookup"><span data-stu-id="a03fb-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="a03fb-107">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="a03fb-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="a03fb-108">Po přihlášení pomocí přihlašovacích údajů Microsoftu 365 Business Premium a připojení k Azure AD, jak je popsáno v článku Nastavení zařízení s Windows pro uživatele [Microsoft 365 Business Premium,](set-up-windows-devices.md)přejděte na **Účty Nastavení Windows** Přístup do práce nebo do \>  \> **školy**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="a03fb-109">Zvolte **Připojeno \<tenant name\> k Azure AD** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="a03fb-111">Na stránce **Spravovaný** podle se zobrazí informace o připojení, které obsahují adresu serveru pro správu, jak je \<tenant name\> znázorněno na následujícím obrázku.  </span><span class="sxs-lookup"><span data-stu-id="a03fb-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="a03fb-113">**Ověřte, že nemůžete vložit data společnosti do nespravovaná aplikace.**</span><span class="sxs-lookup"><span data-stu-id="a03fb-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="a03fb-114">Otevřete Outlook 2016, který nainstaloval Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a03fb-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="a03fb-115">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="a03fb-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="a03fb-116">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="a03fb-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="a03fb-117">Zobrazí se chybová zpráva, že aplikace nemůže získat přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="a03fb-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="a03fb-119">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="a03fb-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="a03fb-120">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních</span><span class="sxs-lookup"><span data-stu-id="a03fb-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="a03fb-121">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="a03fb-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="a03fb-122">Na osobním zařízení s Windows 10, kde jste přihlášení jako místní uživatel, přejděte na **Nastavení Windows** a klikněte nebo klepněte na **Účty** Access v práci nebo \> **ve škole**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="a03fb-123">V části **Přístup do práce nebo do školy** zvolte **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="a03fb-124">Zadejte přihlašovací údaje Microsoft 365 Business Premium do **dialogového** okna Nastavení pracovního nebo školního \> **účtu Přihlásit se**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="a03fb-125">Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="a03fb-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![V dialogovém okně Pracovní nebo školní účet klikněte nebo klepněte na Informace.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="a03fb-127">Na pracovní nebo školní stránce **Accessu** uvidíte informace o připojení, které obsahují adresu serveru pro správu, jako je adresa uvedená na následujícím obrázku, **a** obsahuje slova *wip* a *mam* uvnitř. </span><span class="sxs-lookup"><span data-stu-id="a03fb-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="a03fb-129">**Ověřte, že nemůžete vložit data společnosti do nespravovaná aplikace.**</span><span class="sxs-lookup"><span data-stu-id="a03fb-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="a03fb-130">Otevřete Outlook 2016 a v případě potřeby přidejte svůj účet Microsoft 365 Business Premium a přihlaste se pomocí přihlašovacích údajů microsoftu 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="a03fb-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="a03fb-131">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="a03fb-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="a03fb-132">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="a03fb-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="a03fb-133">Zobrazí se chybová zpráva, že aplikace nemůže získat přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="a03fb-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="a03fb-135">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="a03fb-135">You can, however, paste the same content into Word 2016.</span></span>
    

