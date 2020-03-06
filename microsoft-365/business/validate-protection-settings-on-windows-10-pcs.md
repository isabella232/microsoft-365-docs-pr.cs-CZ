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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Ověřte nastavení ochrany aplikací Microsoft 365 Business na zařízeních s Windows 10 a ověřte, zda uživatelé nemohou kopírovat firemní data do osobních souborů nebo do nespravovaných aplikací.
ms.openlocfilehash: 4d3d7e950311ac32606e700ebb35bf026ae091cc
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/06/2020
ms.locfileid: "42549991"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="c5f90-103">Ověření nastavení ochrany aplikací na počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="c5f90-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="c5f90-104">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních</span><span class="sxs-lookup"><span data-stu-id="c5f90-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="c5f90-105">Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů.</span><span class="sxs-lookup"><span data-stu-id="c5f90-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="c5f90-106">Pokud jste **zapnuli možnost** **Zabránit uživatelům v kopírování firemních dat do osobních souborů a vynutit jim uložení pracovních souborů do nastavení OneDrivu pro firmy** pro zařízení vlastněná společností, můžete to zkontrolovat na zařízení uživatele po připojení k Azure AD a přihlášení.</span><span class="sxs-lookup"><span data-stu-id="c5f90-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="c5f90-107">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="c5f90-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="c5f90-p102">Až se přihlásíte pomocí přihlašovacích údajů Microsoft 365 Business a připojíte se k Azure AD, jak je popsáno v části [Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business](set-up-windows-devices.md), přejděte na **Nastavení systému Windows** \> **Účty** \> **Přístup do práce nebo do školy**. Zvolte **Připojeno k \<název tenanta\> Azure AD** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="c5f90-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="c5f90-111">\> Na stránce Název **klienta** \<Správa podle můžete zobrazit **informace o připojení,** které obsahují adresu serveru pro **správu,** jako je adresa zobrazená na následujícím obrázku.</span><span class="sxs-lookup"><span data-stu-id="c5f90-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="c5f90-113">**Ověření, že nelze vložit firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="c5f90-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="c5f90-114">Otevřete Outlook 2016 nainstalovaný přes Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c5f90-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="c5f90-115">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="c5f90-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="c5f90-116">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="c5f90-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="c5f90-117">Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="c5f90-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="c5f90-119">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="c5f90-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="c5f90-120">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních</span><span class="sxs-lookup"><span data-stu-id="c5f90-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="c5f90-121">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="c5f90-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="c5f90-122">Na osobním zařízení s Windows 10, kde jste přihlášení jako místní uživatel, přejděte do **Nastavení Windows**a klikněte nebo klepněte na Přístup **k účtům** \> **v práci nebo ve škole**.</span><span class="sxs-lookup"><span data-stu-id="c5f90-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="c5f90-123">V části **Přístup do práce nebo do školy** zvolte **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="c5f90-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="c5f90-124">Zadejte přihlašovací údaje Microsoft 365 Business do dialogu **Nastavení pracovního nebo školního účtu** \> **Přihlásit se**.</span><span class="sxs-lookup"><span data-stu-id="c5f90-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="c5f90-125">Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="c5f90-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Klikněte nebo klepněte na Informace v dialogovém okně Pracovní nebo školní účet.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="c5f90-127">Na stránce **Práce nebo škola aplikace Access** se zobrazí informace o **připojení,** které obsahují **adresu serveru pro správu,** jako je adresa zobrazená na následujícím obrázku, a uvnitř obsahuje slova *stírací* a *mam.*</span><span class="sxs-lookup"><span data-stu-id="c5f90-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="c5f90-129">**Ověření, že nelze vložit firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="c5f90-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="c5f90-130">Otevřete Outlook 2016 a přidejte svůj účet Microsoft 365 Business (pokud je to potřeba) a přihlaste se přihlašovacími údaji Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c5f90-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c5f90-131">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="c5f90-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="c5f90-132">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="c5f90-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="c5f90-133">Zobrazí se chyba, která uvádí, že aplikace nemá přístup k obsahu.</span><span class="sxs-lookup"><span data-stu-id="c5f90-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="c5f90-135">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="c5f90-135">You can, however, paste the same content into Word 2016.</span></span>
    

