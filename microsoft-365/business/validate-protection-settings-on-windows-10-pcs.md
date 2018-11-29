---
title: Ověření nastavení ochrany aplikací na počítačích s Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Zjistěte, jak ověřit nastavení ochrany Microsoft 365 Business aplikace v zařízení Windows 10.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983291"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="4d88e-103">Ověření nastavení ochrany aplikací na počítačích s Windows 10</span><span class="sxs-lookup"><span data-stu-id="4d88e-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="4d88e-104">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na firemních zařízeních</span><span class="sxs-lookup"><span data-stu-id="4d88e-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="4d88e-p101">Jakmile [nastavíte zásady ochrany aplikací](protection-settings-for-windows-10-devices.md), může to trvat několik hodin, než se tyto zásady projeví na zařízeních uživatelů. Pokud jste na zařízeních patřících firmě **zapnuli** nastavení **Brání uživatelům v kopírování dat společnosti do osobních souborů a vynucuje, aby ukládali pracovní soubory na OneDrive pro firmy**, můžete ho zkontrolovat na zařízeních uživatelů, kteří se připojí a přihlásí ke službě Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d88e-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="4d88e-107">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="4d88e-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="4d88e-p102">Až se přihlásíte pomocí přihlašovacích údajů Microsoft 365 Business a připojíte se k Azure AD, jak je popsáno v části [Nastavení zařízení s Windows pro uživatele služby Microsoft 365 Business](set-up-windows-devices.md), přejděte na **Nastavení systému Windows** \> **Účty** \> **Přístup do práce nebo do školy**. Zvolte **Připojeno k \<název tenanta\> Azure AD** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="4d88e-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="4d88e-111">Na stránce **Spravuje** \<název tenanta\> najdete **informace o připojení** s **adresou serveru pro správu**, jak je vidět na následujícím obrázku.</span><span class="sxs-lookup"><span data-stu-id="4d88e-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="4d88e-113">**Ověření, že není možné vkládat firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="4d88e-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="4d88e-114">Otevřete Outlook 2016 nainstalovaný přes Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4d88e-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="4d88e-115">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="4d88e-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="4d88e-116">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="4d88e-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="4d88e-117">Zobrazí se chybová zpráva s informacemi o tom, že aplikace nemá k tomuto obsahu přístup.</span><span class="sxs-lookup"><span data-stu-id="4d88e-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="4d88e-119">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="4d88e-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="4d88e-120">Ověření, že uživatelé nemůžou kopírovat firemní data do osobních souborů na osobních zařízeních</span><span class="sxs-lookup"><span data-stu-id="4d88e-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="4d88e-121">**Ověření nastavení připojení**</span><span class="sxs-lookup"><span data-stu-id="4d88e-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="4d88e-122">Na osobním zařízení s Windows 10, kde jste přihlášení jako místní uživatel, přejděte na **Nastavení systému Windows** a klikněte nebo klepněte na **Účty** \> **Přístup do práce nebo do školy**.</span><span class="sxs-lookup"><span data-stu-id="4d88e-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="4d88e-123">V části **Přístup do práce nebo do školy** zvolte **Připojit**.</span><span class="sxs-lookup"><span data-stu-id="4d88e-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="4d88e-124">Zadejte přihlašovací údaje Microsoft 365 Business do dialogu **Nastavení pracovního nebo školního účtu** \> **Přihlásit se**.</span><span class="sxs-lookup"><span data-stu-id="4d88e-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="4d88e-125">Na stránce **Přístup do práce nebo do školy** zvolte **Pracovní nebo školní účet** a pak zvolte **Informace**.</span><span class="sxs-lookup"><span data-stu-id="4d88e-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="4d88e-127">Na stránce **Přístup do práce nebo do školy** najdete **informace o připojení** s **adresou serveru pro správu** (jak je vidět na následujícím obrázku), které budou obsahovat slova  *wip*  a  *mam*  .</span><span class="sxs-lookup"><span data-stu-id="4d88e-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="4d88e-129">**Ověření, že není možné vkládat firemní data do nespravované aplikace**</span><span class="sxs-lookup"><span data-stu-id="4d88e-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="4d88e-130">Otevřete Outlook 2016 a přidejte svůj účet Microsoft 365 Business (pokud je to potřeba) a přihlaste se přihlašovacími údaji Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4d88e-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="4d88e-131">Otevřete e-mail a zkopírujte z něj nějaký obsah.</span><span class="sxs-lookup"><span data-stu-id="4d88e-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="4d88e-132">Otevřete Poznámkový blok a pokuste se do něho obsah vložit.</span><span class="sxs-lookup"><span data-stu-id="4d88e-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="4d88e-133">Zobrazí se chybová zpráva s informacemi o tom, že aplikace nemá k tomuto obsahu přístup.</span><span class="sxs-lookup"><span data-stu-id="4d88e-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="4d88e-135">Stejný obsah ale můžete vložit do Wordu 2016.</span><span class="sxs-lookup"><span data-stu-id="4d88e-135">You can, however, paste the same content into Word 2016.</span></span>
    

