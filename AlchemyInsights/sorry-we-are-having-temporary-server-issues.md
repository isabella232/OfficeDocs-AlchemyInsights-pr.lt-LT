---
title: "\"Microsoft 365\" programų taisymas Atsiprašome, kyla laikinų serverio problemų pranešimas"
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582711"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="25bfa-102">"Microsoft 365" programėlių taisymas "Atsiprašome, kyla laikinų serverio problemų" pranešimas</span><span class="sxs-lookup"><span data-stu-id="25bfa-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="25bfa-103">Jei gaunate šį pranešimą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="25bfa-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="25bfa-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Microsoft 365" programėlių.</span><span class="sxs-lookup"><span data-stu-id="25bfa-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="25bfa-105">Peržiūrėkite [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="25bfa-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="25bfa-106">Eikite į **Pradėti**  >  **vykdyti**, tada įveskite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="25bfa-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="25bfa-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="25bfa-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="25bfa-108">Tinklo prijungtų įrenginių automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="25bfa-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="25bfa-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="25bfa-109">Network List Service</span></span>
    - <span data-ttu-id="25bfa-110">Tinklo vietos žinomumas</span><span class="sxs-lookup"><span data-stu-id="25bfa-110">Network Location Awareness</span></span>
    - <span data-ttu-id="25bfa-111">Windows įvykių žurnalas</span><span class="sxs-lookup"><span data-stu-id="25bfa-111">Windows Event Log</span></span>

<span data-ttu-id="25bfa-112">Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="25bfa-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="25bfa-113">Jei kyla problemų paleidžiant tarnybą, atidarę komandinę eilutę su didesnių teisių komanda vykdykite šią komandą:</span><span class="sxs-lookup"><span data-stu-id="25bfa-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="25bfa-114">**SFC /scannow SFC /scannow SFC / scannow SFC**</span><span class="sxs-lookup"><span data-stu-id="25bfa-114">**sfc /scannow**</span></span>

<span data-ttu-id="25bfa-115">Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.</span><span class="sxs-lookup"><span data-stu-id="25bfa-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="25bfa-116">Išsamesnės informacijos [ieškokite "Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai įjungiate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="25bfa-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>