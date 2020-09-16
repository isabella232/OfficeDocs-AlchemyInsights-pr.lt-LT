---
title: "\"Microsoft 365\" taikomųjų programų taisymas Atsiprašome, yra laikino serverio problemų pranešimas"
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758253"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="8d8e4-102">"Microsoft 365" taikomųjų programų taisymas pranešimas "Atsiprašome, iškilo laikinų serverio problemų"</span><span class="sxs-lookup"><span data-stu-id="8d8e4-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="8d8e4-103">Gavę šį pranešimą, išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8d8e4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="8d8e4-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Microsoft" 365 taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="8d8e4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="8d8e4-105">Peržiūrėkite [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="8d8e4-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="8d8e4-106">Eikite į **pradėti**  >  **vykdyti**ir įveskite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="8d8e4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="8d8e4-107">Įsitikinkite, kad visos toliau nurodytos tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="8d8e4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="8d8e4-108">Tinklo prijungtų įrenginių Automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="8d8e4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="8d8e4-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="8d8e4-109">Network List Service</span></span>
    - <span data-ttu-id="8d8e4-110">Tinklo vietos informacijos suvokimas</span><span class="sxs-lookup"><span data-stu-id="8d8e4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="8d8e4-111">"Windows" įvykių registras</span><span class="sxs-lookup"><span data-stu-id="8d8e4-111">Windows Event Log</span></span>

<span data-ttu-id="8d8e4-112">Jei viena iš šių tarnybų nepaleista, bandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="8d8e4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="8d8e4-113">Jei kilo problemų paleidžiant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę naudodami didesnes teises:</span><span class="sxs-lookup"><span data-stu-id="8d8e4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="8d8e4-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="8d8e4-114">**sfc /scannow**</span></span>

<span data-ttu-id="8d8e4-115">Baigę šią komandą, iš naujo paleiskite kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="8d8e4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="8d8e4-116">Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų abonemento. Bandykite dar kartą vėliau "klaida, kai suaktyvinate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="8d8e4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>