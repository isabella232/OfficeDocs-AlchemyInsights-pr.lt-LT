---
title: Prisijungimo prie "Microsoft 365" programų problemos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833083"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="61d01-102">"Microsoft 365" programų "Atsiprašome, kita jūsų organizacijos paskyra jau yra prisijungusi" taisymo pranešimas</span><span class="sxs-lookup"><span data-stu-id="61d01-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="61d01-103">Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="61d01-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="61d01-104">Pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą, naudodami "Windows" > **"Access" darbo arba mokymo įstaigos**.</span><span class="sxs-lookup"><span data-stu-id="61d01-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="61d01-105">[Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="61d01-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="61d01-106">**Pastaba:** "Office 2016" registro keliai pakeisti į 16.0.</span><span class="sxs-lookup"><span data-stu-id="61d01-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="61d01-107">(pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="61d01-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="61d01-108">Atidarykite "Office" programą, **pasirinkite**  >  **Failo paskyra**  >  **Atsijungti**. Tada prisijunkite naudodami vartotojo paskyrą su galiojančia licencija.</span><span class="sxs-lookup"><span data-stu-id="61d01-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="61d01-109">Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="61d01-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="61d01-110">Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="61d01-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="61d01-111">Daugiau informacijos žr. "Atsiprašome, kita jūsų organizacijos paskyra jau [yra prisijungusi šiame kompiuteryje" "Office".](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="61d01-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>