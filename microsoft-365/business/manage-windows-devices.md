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
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Povolení správy zařízení s Windows 10 s doménou pomocí Microsoft 365 Business Premium

Pokud vaše organizace používá windows server Active Directory místně, můžete nastavit Microsoft 365 Business Premium na ochranu vašich zařízení s Windows 10 a přitom zachovat přístup k místním prostředkům, které vyžadují místní ověřování.
Chcete-li nastavit tuto ochranu, můžete implementovat **hybridní zařízení spojené Azure AD**. Tato zařízení jsou připojena k místnímu službě Active Directory i k vašemu službě Azure Active Directory.

Toto video popisuje postup, jak nastavit tento scénář pro nejběžnější scénář, který je také podrobně popsán v následujících krocích.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Než začnete, ujistěte se, že provedete tyto kroky:
- Synchronizujte uživatele s Azure AD pomocí služby Azure AD Connect.
- Dokončete synchronizaci organizační jednotky Azure AD Connect (OU).
- Ujistěte se, že všichni uživatelé domény, které synchronizujete, mají licence k Microsoft 365 Business Premium.

Postup naleznete v tématu [Synchronizace uživatelů domény](manage-domain-users.md) společnosti Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Ověření autority MDM v Intune

Přejděte na portal.azure.com a v horní části stránky vyhledejte Intune.
Na stránce Microsoft Intune vyberte **Registrace zařízení** a na stránce **Přehled** se ujistěte, že **autorita MDM** je **Intune**.

- Pokud **autorita MDM** není **žádná**, klepněte na **autoritu MDM a** nastavte ji na **Intune**.
- Pokud je **autorita MDM** **Microsoft Office 365**, přejděte na **Zařízení**  >  **pro registraci zařízení** a použijte dialogové okno Přidat **autoritu MDM** vpravo k přidání autority **Intune MDM** (dialogové okno **Přidat autoritu MDM je** k dispozici jenom v případě, že je **autorita MDM** nastavená na Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Ověření, že azure ad je povolena pro připojení k počítačům

- Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte **Azure Active Directory** (v seznamu **Centra pro správu** vyberte Zobrazit vše, pokud azure active directory není viditelná). 
- V **Centru pro správu Služby Active Directory Azure**přejděte na **Azure Active Directory** , zvolte **Zařízení** a potom **nastavení zařízení**.
- Ověřit, že**uživatelé mohou připojit zařízení k Azure AD** je povolena 
    1. Chcete-li povolit všechny uživatele, nastavte hodnotu **Vše**.
    2. Chcete-li povolit konkrétní uživatele, nastavte na **Hodnotu Vybrané,** která povolí určitou skupinu uživatelů.
        - Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).
        - Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Ověření, že azure ad je povolena pro MDM

- Přejděte do Centra pro správu na <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> adrese a vyberte možnost **Endpoint Managemen**t (vyberte **Zobrazit vše,** pokud **endpoint Manager** není viditelný)
- V **Centru pro správu Správce koncových bodů společnosti Microsoft**přejděte na **Položku**Automatické  >  **Windows**  >  registrace**systému**Windows  >  **Automatic Enrollment**zařízení .
- Ověřte, zda je povolen obor uživatele MDM.

    1. Chcete-li zaregistrovat všechny počítače, nastavte na **Vše,** abyste automaticky zaregistrovali všechny uživatelské počítače, které jsou připojeny k Azure AD a novým počítačům, když uživatelé přidají pracovní účet do Windows.
    2. Chcete-li zaregistrovat počítače určité skupiny uživatelů, nastavte hodnotu **Některé.**
        -  Přidejte uživatele požadované domény synchronizované ve službě Azure AD do [skupiny zabezpečení](../admin/create-groups/create-groups.md).
        -  Zvolte **Vybrat skupiny,** chcete-li povolit uživatelský obor MDM pro tuto skupinu zabezpečení.

## <a name="4-set-up-service-connection-point-scp"></a>4. Nastavení spojovacího bodu služby (SCP)

Tyto kroky jsou zjednodušeny [z konfigurace hybridního spojení Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Chcete-li provést kroky, které potřebujete k použití Azure AD Connect a vašich globálních administrátorů Microsoft 365 Business Premium a hesel pro správce služby Active Directory.

1.  Spusťte Azure AD Connect a pak vyberte **Konfigurovat**.
2.  Na stránce **Další úkoly** vyberte **Konfigurovat možnosti zařízení**a pak vyberte **Další**.
3.  Na stránce **Přehled** vyberte **Další**.
4.  Na stránce **Připojení k Azure AD** zadejte přihlašovací údaje globálního správce pro Microsoft 365 Business Premium.
5.  Na stránce **Možnosti zařízení** vyberte **Konfigurovat hybridní spojení Azure AD**a pak vyberte **Další**.
6.  Na stránce **SCP** pro každou doménovou strukturu, ve které chcete azure ad connect nakonfigurovat SCP, proveďte následující kroky a pak vyberte **Další**:
    - Zaškrtněte políčko vedle názvu doménové struktury. Doménová struktura by měla být název domény služby AD.
    - Ve sloupci **Ověřovací služba** otevřete rozevírací seznam a vyberte odpovídající název domény (měla by existovat pouze jedna možnost).
    - Vyberte **Přidat** a zadejte pověření správce domény.  
7.  Na stránce **Operační systémy Zařízení** vyberte jenom zařízení připojená k Windows 10 nebo novějším doménovým systémům.
8.  Na stránce **Připraveno ke konfiguraci** vyberte **Konfigurovat**.
9.  Na stránce **Konfigurace dokončení** vyberte **Exit**.


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Vytvoření objektu zásad skupiny pro registraci Intune – metoda ADMX

Použít. soubor šablony ADMX.

1.  Přihlaste se k serveru AD, vyhledejte a otevřete **Server Manager**  >  **Tools**  >  **správu zásad skupiny**Nástroje správce serveru .
2.  Vyberte název domény v části **Domény** a vyberte položku **Nový**klepnutím pravým tlačítkem myši na **položku Objekty zásad skupiny** .
3.  Pojmenujte nový objekt zásad skupiny, například "*Cloud_Enrollment*" a pak vyberte **OK**.
4.  Klepněte pravým tlačítkem myši na nový objekt zásad skupiny v části **Objekty zásad skupiny** a vyberte příkaz **Upravit**.
5.  V **Editoru správy zásad skupiny** **přejděte**na  >  **položku Šablony správy zásad**konfigurace  >  **Administrative Templates**  >  **počítače, součásti systému Windows**  >  **MDM**.
6. Klikněte pravým tlačítkem myši na **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD** a pak vyberte **povoleno**  >  **OK**. Zavřete okno editoru.

> [!IMPORTANT]
> Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , přečtěte [si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si přečtěte si nejnovější šablony pro správu](#get-the-latest-administrative-templates).

## <a name="6-deploy-the-group-policy"></a>6. Nasazení zásad skupiny

1.  Ve Správci serveru v části **Domains** > Group Policy objects vyberte objekt zásad skupiny z výše uvedeného kroku 3, například "Cloud_Enrollment".
2.  Vyberte kartu **Obor** pro objekt zásad skupiny.
3.  Na kartě Obor objektu zásad skupiny klikněte pravým tlačítkem myši na odkaz na doménu v části **Odkazy**.
4.  Chcete-li na obrazovce potvrzení nasadit objekt zásad skupiny, vyberte možnost **Vynuceno** a potom **OK.**

## <a name="get-the-latest-administrative-templates"></a>Získejte nejnovější šablony pro správu

Pokud zásady **Povolit automatickou registraci MDM pomocí výchozích přihlašovacích údajů služby Azure AD**nevidíte , může to být způsobeno tím, že nemáte nainstalované kódY ADMX pro Systém Windows 10 verze 1803, verze 1809 nebo verze 1903. Chcete-li tento problém vyřešit, postupujte takto (Poznámka: nejnovější MDM.admx je zpětně kompatibilní):

1.  Ke stažení: [Šablony pro správu (.admx) pro Windows 10 Květen 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Nainstalujte balíček do primárního řadiče domény (PDC).
3.  Navigace v závislosti na verzi složky: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.
4.  Přejmenujte složku **Definice zásad** ve výše uvedené cestě k **policydefinition .**
5.  Zkopírujte složku **PolicyDefinitions** do **souboru C:\Windows\SYSVOL\domain\Policies**. 
    -   Pokud máte v plánu použít centrální úložiště zásad pro celou doménu, přidejte obsah PolicyDefinitions tam.
6.  Chcete-li, aby byla tato zásada k dispozici, restartujte primární řadič domény. Tento postup bude fungovat i pro všechny budoucí verze.

V tomto okamžiku byste měli vidět zásady **Povolit automatické registrace MDM pomocí výchozích přihlašovacích údajů Azure AD** k dispozici.

