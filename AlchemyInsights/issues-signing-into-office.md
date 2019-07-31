---
title: Problemos prisijungiant prie "Office" programos
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938278"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="e8441-102">Problemos prisijungiant prie "Office" programos</span><span class="sxs-lookup"><span data-stu-id="e8441-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="e8441-103">Norėdami išspręsti prisijungimo problemas su "Office" programos, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="e8441-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="e8441-104">Pašalinti visas darbo sąskaitas, išskyrus paveiktą paskyrą, naudodami "Windows" parametrus > **prieigos darbe ar mokykloje**.</span><span class="sxs-lookup"><span data-stu-id="e8441-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e8441-105">[Aišku Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvas.</span><span class="sxs-lookup"><span data-stu-id="e8441-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e8441-106">**Pastaba:** 16,0 pasikeitė registro maršrutai Office 2016.</span><span class="sxs-lookup"><span data-stu-id="e8441-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e8441-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e8441-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e8441-108">Atidaryti Office programą, pasirinkite **failą** > **į** > **Atsijungti**. Tada prisijunkite naudodami vartotojo abonementą, turintis galiojančią licenciją.</span><span class="sxs-lookup"><span data-stu-id="e8441-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e8441-109">Išsamios informacijos, peržiūrėkite [sąskaitas savo pareigas](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e8441-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e8441-110">Skirta "Mac", žr. [negaliu prisijungti prie Office 2016 Mac App](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e8441-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="e8441-111">Jei klaidos atsiranda, o jungiantis prie Office 2013 naudojant "Office 365", leidžia šiuolaikinės autentifikavimas Office kliento.</span><span class="sxs-lookup"><span data-stu-id="e8441-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="e8441-112">Daugiau informacijos žr.</span><span class="sxs-lookup"><span data-stu-id="e8441-112">For more information, see:</span></span>
- [<span data-ttu-id="e8441-113">Jūs negalite prisijungti prie "Office 365", Azure arba Intune</span><span class="sxs-lookup"><span data-stu-id="e8441-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="e8441-114">Ryšį klausimai programoje prisijungdami po atnaujinimo į Office 2016, kurti 16.0.7967 "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="e8441-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="e8441-115">"Deja, kitą sąskaitą iš jūsų organizacija jau pasirašė šiame kompiuteryje" biure</span><span class="sxs-lookup"><span data-stu-id="e8441-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="e8441-116">Spręsti prisijungimo problemas su Office šiuolaikinės autentifikavimas naudojant ADFS</span><span class="sxs-lookup"><span data-stu-id="e8441-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)