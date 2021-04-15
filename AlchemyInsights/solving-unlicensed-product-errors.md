---
title: Nelicenti klaid ų sprendimas
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786857"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="9a5c8-102">Pasiūlymai, kaip spręsti klaidas "Nelicentikuotas produktas"</span><span class="sxs-lookup"><span data-stu-id="9a5c8-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="9a5c8-103">Norėdami išspręsti nelicegeninio produkto klaidas, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9a5c8-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="9a5c8-104">Patikrinkite, ar baigėsi prenumeratos būsenos galiojimas.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="9a5c8-105">Įsitikinkite, kad turite prenumeratą, kuri leidžia kliento licencijas, pvz., "Microsoft 365" programėles verslui arba "Business Premium", ir įsitikinkite, kad [vartotojas turi priskirtą licenciją.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="9a5c8-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="9a5c8-106">Įsitikinkite, kad vartotojas prisijungia prie "Office" tuo pačiu abonementu, kuriam priskirta licencija.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="9a5c8-107">Patikrinkite puslapį [Tarnybos sveikata,](https://docs.microsoft.com/office365/enterprise/view-service-health) kad pamatytumėte, ar yra žinomų tarnybos problemų.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="9a5c8-108">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja "Microsoft 365" programų prieigos prie interneto.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="9a5c8-109">Žr. [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9a5c8-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="9a5c8-110">Taip pat galite išbandyti šiuos trikčių šalinimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9a5c8-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="9a5c8-111">Atidarykite "Office" programą [ir atsijungti](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo esamų vartotojų paskyrų.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="9a5c8-112">[Pašalinkite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [ir iš naujo priskirkite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) "Office" licenciją, tada [prisijunkite prie "Office"](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) naudodami paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="9a5c8-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="9a5c8-113">Paleiskite [aktyvinimo trikčių diagnostikos priemonę](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="9a5c8-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="9a5c8-114">[Iš naujo nustatykite "Office" aktyvinimo būseną](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="9a5c8-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="9a5c8-115">[Atlikite "Office" taisymo internete veiksmą.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="9a5c8-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="9a5c8-116">Jei reikia papildomų problemų sprendimo patarimų, žr.:</span><span class="sxs-lookup"><span data-stu-id="9a5c8-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="9a5c8-117">Nelicencijuoto produkto ir aktyvinimo klaidos „Office“</span><span class="sxs-lookup"><span data-stu-id="9a5c8-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="9a5c8-118">„Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau“ klaida, pasirodanti jums aktyvinus „Office“</span><span class="sxs-lookup"><span data-stu-id="9a5c8-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)