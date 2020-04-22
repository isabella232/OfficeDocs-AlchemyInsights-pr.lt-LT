---
title: Aktyvinimo problema - Mes negalime prisijungti dabar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716180"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="296dd-102">"Office" programų "Šiuo metu nepavyksta prisijungti" nustatymas</span><span class="sxs-lookup"><span data-stu-id="296dd-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="296dd-103">Jei gaunate šį pranešimą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="296dd-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="296dd-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Office" programų.</span><span class="sxs-lookup"><span data-stu-id="296dd-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="296dd-105">Peržiūrėkite ["Microsoft" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="296dd-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="296dd-106">Eikite į **Pradėti** > **vykdyti**, tada įveskite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="296dd-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="296dd-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="296dd-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="296dd-108">Tinklo prijungtų įrenginių automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="296dd-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="296dd-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="296dd-109">Network List Service</span></span>
    - <span data-ttu-id="296dd-110">Tinklo vietos žinomumas</span><span class="sxs-lookup"><span data-stu-id="296dd-110">Network Location Awareness</span></span>
    - <span data-ttu-id="296dd-111">Windows įvykių žurnalas</span><span class="sxs-lookup"><span data-stu-id="296dd-111">Windows Event Log</span></span>

<span data-ttu-id="296dd-112">Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="296dd-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="296dd-113">Jei kyla problemų paleidžiant tarnybą, atidarę komandinę eilutę su didesnių teisių komanda vykdykite šią komandą:</span><span class="sxs-lookup"><span data-stu-id="296dd-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="296dd-114">**SFC /scannow SFC /scannow SFC / scannow SFC**</span><span class="sxs-lookup"><span data-stu-id="296dd-114">**sfc /scannow**</span></span>

<span data-ttu-id="296dd-115">Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.</span><span class="sxs-lookup"><span data-stu-id="296dd-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="296dd-116">Išsamesnės informacijos [ieškokite "Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai aktyvinate "Office" iš "Microsoft 365".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="296dd-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>