---
title: Prisijungimo prie "Office" taikomųjų programų problemos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763009"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="3359e-102">Prisijungimo prie "Office" taikomųjų programų problemos</span><span class="sxs-lookup"><span data-stu-id="3359e-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="3359e-103">Norėdami išspręsti prisijungimo problemas, susijusias su "Office" programomis, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="3359e-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="3359e-104">Pašalinkite visus darbo abonementus, išskyrus paveiktą abonementą, naudodami "Windows" parametrus > **"Access" darbą arba mokyklą**.</span><span class="sxs-lookup"><span data-stu-id="3359e-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="3359e-105">[Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="3359e-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3359e-106">**Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0.</span><span class="sxs-lookup"><span data-stu-id="3359e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3359e-107">(Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3359e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3359e-108">Atidarykite "Office" programą, pasirinkite > **Atsijungti prie** **failų** > **abonemento**. Tada prisijunkite naudodami vartotojo abonementą su galiojančia licencija.</span><span class="sxs-lookup"><span data-stu-id="3359e-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="3359e-109">Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3359e-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3359e-110">Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="3359e-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="3359e-111">Jei klaidos įvyksta jungiantis prie "Microsoft 365" naudojant "Office 2013", įgalinkite šiuolaikinės autentifikavimas Office kliento.</span><span class="sxs-lookup"><span data-stu-id="3359e-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="3359e-112">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="3359e-112">For more information, see:</span></span>
- [<span data-ttu-id="3359e-113">Negalite prisijungti prie "Microsoft 365", "Azure" arba "Intune"</span><span class="sxs-lookup"><span data-stu-id="3359e-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="3359e-114">Ryšio problemos, kai atnaujinate į "Office 2016" komponavimo versijos 16.0.7967 "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="3359e-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="3359e-115">"Atsiprašome, kitas jūsų organizacijos abonementas jau prisijungęs šiame kompiuteryje" "Office"</span><span class="sxs-lookup"><span data-stu-id="3359e-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="3359e-116">Prisijungimo trikčių šalinimas naudojant "Office" šiuolaikinės autentifikavimas naudojant ADFS</span><span class="sxs-lookup"><span data-stu-id="3359e-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)