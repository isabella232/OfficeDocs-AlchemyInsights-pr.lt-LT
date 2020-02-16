---
title: "\"Office Apps\" taisymas jūsų abonementas yra blogos būsenos pranešimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969627"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="96c1e-102">"Office" programėlių taisymas "klaida" jūsų abonementas yra blogos būsenos "</span><span class="sxs-lookup"><span data-stu-id="96c1e-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="96c1e-103">Norėdami išspręsti šią klaidą, Išbandykite šias parinktis paveiktame kompiuteryje:</span><span class="sxs-lookup"><span data-stu-id="96c1e-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="96c1e-104">Atidarykite "Office" programėlę, pasirinkite **failo** > **abonemento** > **Atsijungti nuo visų paskyrų**.</span><span class="sxs-lookup"><span data-stu-id="96c1e-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="96c1e-105">Vėl prisijunkite naudodami vartotojo abonementą su galiojančia licencija.</span><span class="sxs-lookup"><span data-stu-id="96c1e-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="96c1e-106">Išsamesnės informacijos ieškokite [Office aplankuose](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="96c1e-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="96c1e-107">[Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="96c1e-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="96c1e-108">**Pastaba:** Registro keliai Office 2016 pasikeitė į 16,0.</span><span class="sxs-lookup"><span data-stu-id="96c1e-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="96c1e-109">Pvz., \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="96c1e-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="96c1e-110">Susijusio kompiuterio, nustatykite EnableADAL = 0, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="96c1e-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="96c1e-111">Dešiniuoju pelės mygtuku spustelėkite mygtuką "Windows" ir pasirinkite **vykdyti**.</span><span class="sxs-lookup"><span data-stu-id="96c1e-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="96c1e-112">Lauke **atidaryti** įveskite **regedit**, ir tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="96c1e-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="96c1e-113">Pasirinkite **taip** Kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="96c1e-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="96c1e-114">Registro rengyklėje pridėkite EnableADAL DWORD reikšmę su parametr 0 pagal HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="96c1e-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="96c1e-115">Jei klaida įvyksta jungiantis prie "Office 365" naudojant "Office 2013", [įjunkite modernų](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) "Office" kliento autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="96c1e-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="96c1e-116">Jei norite gauti daugiau informacijos, Sužinokite, [kaip spręsti ne naršyklės programas, kurios negali prisijungti prie Office 365, Azure arba Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="96c1e-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

