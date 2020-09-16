---
title: "\"Microsoft 365\" programų taisymas nepavyko aptikti \"Office\" licencijų susijusio pranešimo"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747703"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="4757f-102">"Microsoft 365" taikomųjų programų taisymas "nepavyko aptikti" Office "licencijų susietųjų"</span><span class="sxs-lookup"><span data-stu-id="4757f-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="4757f-103">Gavę šį pranešimą, išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="4757f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4757f-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Microsoft" 365 taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="4757f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4757f-105">Peržiūrėkite ["Microsoft" 365 URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="4757f-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="4757f-106">Pašalinkite ir iš [naujo priskirkite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) susijusio vartotojo "Office" licenciją.</span><span class="sxs-lookup"><span data-stu-id="4757f-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="4757f-107">Atidarykite "Office" programą ir [atsijunkite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo esamų vartotojų paskyrų.</span><span class="sxs-lookup"><span data-stu-id="4757f-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="4757f-108">Eikite į "Windows" parametrai > **paskyros**  >  **el. paštas & paskyras**ir pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą.</span><span class="sxs-lookup"><span data-stu-id="4757f-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="4757f-109">Eikite į "Windows" parametrai > **paskyrų**  >  **prieiga prie darbo arba mokymo įstaigos**ir atjunkite visas darbo paskyras, išskyrus paveiktą paskyrą.</span><span class="sxs-lookup"><span data-stu-id="4757f-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="4757f-110">Iš naujo nustatykite "Office" aktyvinimo būseną.</span><span class="sxs-lookup"><span data-stu-id="4757f-110">Reset the Office activation state.</span></span> <span data-ttu-id="4757f-111">[Sužinokite, kaip](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="4757f-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="4757f-112">[Prisijunkite](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) naudodami paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="4757f-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="4757f-113">Papildomų trikčių šalinimo sprendimų ieškokite [nelicencijuoto produkto ir aktyvinimo klaidos "Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)".</span><span class="sxs-lookup"><span data-stu-id="4757f-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>