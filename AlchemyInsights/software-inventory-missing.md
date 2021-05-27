---
title: Trūksta programinės įrangos atsargų arba jos nėra netikslios
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676508"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="2b86b-102">Trūksta programinės įrangos atsargų arba jos nėra netikslios</span><span class="sxs-lookup"><span data-stu-id="2b86b-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="2b86b-103">Programinės įrangos atsargos grėsmių ir pažeidžiamumų valdymas (TVM) yra žinomos programinės įrangos jūsų organizacijoje su oficialiais bendrosios platformos skaičiavimais (CPE) sąrašas.</span><span class="sxs-lookup"><span data-stu-id="2b86b-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="2b86b-104">Programinės įrangos produktai be oficialaus CPE neturi publikuotų pažeidžiamumų.</span><span class="sxs-lookup"><span data-stu-id="2b86b-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="2b86b-105">Atsargose taip pat yra išsami informacija, pvz., tiekėjo pavadinimas, silpnųjų vietų skaičius, grėsmės ir rodomų įrenginių skaičius.</span><span class="sxs-lookup"><span data-stu-id="2b86b-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="2b86b-106">Programinės įrangos pakeitimai įrenginiuose paprastai atsispindi saugos portaluose per dvi valandas.</span><span class="sxs-lookup"><span data-stu-id="2b86b-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="2b86b-107">Tačiau kartais gali užtrukti ilgiau.</span><span class="sxs-lookup"><span data-stu-id="2b86b-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="2b86b-108">Šiuo metu negalima priversti sinchronizuoti; tai nuolatinis nuolatinis įvertinimas.</span><span class="sxs-lookup"><span data-stu-id="2b86b-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="2b86b-109">Jei atlikote programinės įrangos keitimą ir pakeitimas TVM tiksliai neatspindi po 5 valandų, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="2b86b-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="2b86b-110">Patikrinkite programinės įrangos įrodymų skyrių, kad suprastumėte, kaip aptikta programinė įranga.</span><span class="sxs-lookup"><span data-stu-id="2b86b-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="2b86b-111">Įsitikinkite, kad programinė įranga palaikoma.</span><span class="sxs-lookup"><span data-stu-id="2b86b-111">Make sure that the software is supported.</span></span> <span data-ttu-id="2b86b-112">Programinė įranga gali būti matoma tik įrenginio lygiu, net jei šiuo metu jos nepalaiko grėsmių ir pažeidžiamumų valdymas.</span><span class="sxs-lookup"><span data-stu-id="2b86b-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="2b86b-113">Tačiau galimi tik riboti duomenys.</span><span class="sxs-lookup"><span data-stu-id="2b86b-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="2b86b-114">Veiksmus, kaip pranešti apie netikslumą iš portalo, žr. [Ataskaitos netikslumas](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="2b86b-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="2b86b-115">**Pastaba:** pranešimas apie netikslumą iš MDE portalo yra vieningas kanalas į inžineriją.</span><span class="sxs-lookup"><span data-stu-id="2b86b-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="2b86b-116">Jei problema yra skubi, atidarykite palaikymo kvitą.</span><span class="sxs-lookup"><span data-stu-id="2b86b-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="2b86b-117">Daugiau informacijos žr. Programinės [įrangos atsargos – grėsmių ir pažeidžiamumų valdymas](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="2b86b-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>