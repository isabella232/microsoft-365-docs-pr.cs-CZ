---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
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
description: Ověřte nastavení ochrany aplikací Microsoft 365 Business Premium na zařízeních s Windows 10 a ověřte, zda uživatelé nemohou kopírovat firemní data do osobních souborů nebo do nespravovaných aplikací.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403384"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="aff4c-103">Ověření nastavení ochrany aplikací na počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="aff4c-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="aff4c-104">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních</span><span class="sxs-lookup"><span data-stu-id="aff4c-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="aff4c-105">Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="aff4c-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="aff4c-106">Pokud jste **zapnuli možnost** **Zabránit uživatelům v kopírování firemních dat do osobních souborů a vynutit jim uložení pracovních souborů do nastavení OneDrivu pro firmy** pro zařízení vlastněná společností, můžete to zkontrolovat na zařízení uživatele po připojení k Azure AD a přihlášení.</span><span class="sxs-lookup"><span data-stu-id="aff4c-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="aff4c-107">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="aff4c-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="aff4c-108">Po přihlášení pomocí přihlašovacích údajů k Microsoft 365 Business Premium a připojení k Azure AD, jak je popsáno v [části Nastavení zařízení s Windows pro uživatele Microsoft 365 Business Premium](set-up-windows-devices.md), přejděte na pracovní nebo školní téma Windows **Settings** \> **Accounts** \> **Access**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="aff4c-109">Zvolte **Připojeno k \<tenant name\> Azure AD**a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="aff4c-111">Na stránce **Správa podle** \<tenant name\> uvidíte informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku.</span><span class="sxs-lookup"><span data-stu-id="aff4c-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="aff4c-113">**Ověření, že nelze vložit firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="aff4c-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="aff4c-114">Otevřete Outlook 2016, který nainstaloval Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="aff4c-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="aff4c-115">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="aff4c-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="aff4c-116">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="aff4c-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="aff4c-117">Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="aff4c-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="aff4c-119">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="aff4c-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="aff4c-120">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních</span><span class="sxs-lookup"><span data-stu-id="aff4c-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="aff4c-121">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="aff4c-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="aff4c-122">Na osobním zařízení s Windows 10, kde jste přihlášení jako místní uživatel, přejděte do **Nastavení Windows**a klikněte nebo klepněte na Přístup **k** \> **účtům v práci nebo ve škole**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="aff4c-123">V části **Přístup do práce nebo do školy** zvolte **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="aff4c-124">Zadejte své přihlašovací údaje microsoft 365 Business Premium do **dialogového okna Nastavit pracovní nebo školní účet** \> **Přihlášení**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="aff4c-125">Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="aff4c-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Klikněte nebo klepněte na Informace v dialogovém okně Pracovní nebo školní účet.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="aff4c-127">Na stránce **Práce nebo škola aplikace Access** se zobrazí informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku, a uvnitř obsahuje slova *stírací* a *mam.*</span><span class="sxs-lookup"><span data-stu-id="aff4c-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="aff4c-129">**Ověření, že nelze vložit firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="aff4c-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="aff4c-130">Otevřete Outlook 2016 a v případě potřeby přidejte svůj účet Microsoft 365 Business Premium a přihlaste se pomocí přihlašovacích údajů microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="aff4c-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="aff4c-131">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="aff4c-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="aff4c-132">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="aff4c-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="aff4c-133">Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="aff4c-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="aff4c-135">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="aff4c-135">You can, however, paste the same content into Word 2016.</span></span>
    

