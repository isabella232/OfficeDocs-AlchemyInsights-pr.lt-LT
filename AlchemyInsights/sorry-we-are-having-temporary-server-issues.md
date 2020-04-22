---
title: "\"Office\" programų taisymas Atsiprašome, kyla laikinų serverio problemų pranešimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764125"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="bad3d-102">"Office" programų taisymas "Atsiprašome, kyla laikinų serverio problemų" pranešimas</span><span class="sxs-lookup"><span data-stu-id="bad3d-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="bad3d-103">Jei gaunate šį pranešimą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="bad3d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bad3d-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Office" programų.</span><span class="sxs-lookup"><span data-stu-id="bad3d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="bad3d-105">Peržiūrėkite [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bad3d-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bad3d-106">Eikite į **Pradėti** > **vykdyti**, tada įveskite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="bad3d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bad3d-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="bad3d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bad3d-108">Tinklo prijungtų įrenginių automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="bad3d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bad3d-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="bad3d-109">Network List Service</span></span>
    - <span data-ttu-id="bad3d-110">Tinklo vietos žinomumas</span><span class="sxs-lookup"><span data-stu-id="bad3d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bad3d-111">Windows įvykių žurnalas</span><span class="sxs-lookup"><span data-stu-id="bad3d-111">Windows Event Log</span></span>

<span data-ttu-id="bad3d-112">Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="bad3d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bad3d-113">Jei kyla problemų paleidžiant tarnybą, atidarę komandinę eilutę su didesnių teisių komanda vykdykite šią komandą:</span><span class="sxs-lookup"><span data-stu-id="bad3d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bad3d-114">**SFC /scannow SFC /scannow SFC / scannow SFC**</span><span class="sxs-lookup"><span data-stu-id="bad3d-114">**sfc /scannow**</span></span>

<span data-ttu-id="bad3d-115">Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.</span><span class="sxs-lookup"><span data-stu-id="bad3d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bad3d-116">Išsamesnės informacijos [ieškokite "Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai įjungiate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bad3d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>