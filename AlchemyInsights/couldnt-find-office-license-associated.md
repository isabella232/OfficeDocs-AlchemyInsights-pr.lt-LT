---
title: "\"Microsoft 365\" programų taisymo nepavyko rasti su \"Office\" licencijomis susijusio pranešimo"
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816496"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="3028a-102">"Microsoft 365" programų "Nepavyko rasti susietų "Office" licencijų" taisymo pranešimas</span><span class="sxs-lookup"><span data-stu-id="3028a-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="3028a-103">Jei gaunate šį pranešimą, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="3028a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3028a-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Microsoft 365" programų.</span><span class="sxs-lookup"><span data-stu-id="3028a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3028a-105">Žr. ["Microsoft 365" URL ir IP adresų diapazonai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3028a-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="3028a-106">Pašalinkite [ir iš naujo priskirti susijusio vartotojo "Office"](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenciją.</span><span class="sxs-lookup"><span data-stu-id="3028a-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="3028a-107">Atidarykite "Office" programą [ir atsijungti](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo esamų vartotojų paskyrų.</span><span class="sxs-lookup"><span data-stu-id="3028a-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="3028a-108">Eikite į "Windows" parametrai > **Paskyros**  >  **El. & paskyros** ir pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą.</span><span class="sxs-lookup"><span data-stu-id="3028a-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="3028a-109">Eikite į "Windows" parametrai >  >  **"Accounts Access" darbo arba mokymo** įstaigos ir atjunkite visas darbo paskyras, išskyrus paveiktą paskyrą.</span><span class="sxs-lookup"><span data-stu-id="3028a-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="3028a-110">Iš naujo nustatykite "Office" aktyvinimo būseną.</span><span class="sxs-lookup"><span data-stu-id="3028a-110">Reset the Office activation state.</span></span> <span data-ttu-id="3028a-111">[Sužinokite, kaip](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3028a-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="3028a-112">[Prisijunkite naudodami](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="3028a-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="3028a-113">Daugiau trikčių šalinimo sprendimų žr. [Nelicelicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3028a-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>