---
title: "\"Office\" programėlių taisymas Atsiprašome, mes turime laikiną serverio problemos pranešimą"
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627998"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="e66e7-102">"Office" programėlių taisymas "Atsiprašome, mes turime laikiną serverio problemos" pranešimas</span><span class="sxs-lookup"><span data-stu-id="e66e7-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="e66e7-103">Jei gavote šį pranešimą, išbandykite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="e66e7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e66e7-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Office" programėlių.</span><span class="sxs-lookup"><span data-stu-id="e66e7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e66e7-105">Peržiūrėkite " [Office 365" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e66e7-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e66e7-106">Eikite į **pradėti** > **vykdyti**, tada įveskite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="e66e7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e66e7-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="e66e7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e66e7-108">Tinklo prijungtų įrenginių Automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="e66e7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e66e7-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="e66e7-109">Network List Service</span></span>
    - <span data-ttu-id="e66e7-110">Tinklo vieta sąmoningumo</span><span class="sxs-lookup"><span data-stu-id="e66e7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e66e7-111">"Windows" įvykių žurnale</span><span class="sxs-lookup"><span data-stu-id="e66e7-111">Windows Event Log</span></span>

<span data-ttu-id="e66e7-112">Jei viena iš šių paslaugų nepaleista, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="e66e7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e66e7-113">Jei turite problemų pradedant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę su didesnių teisių:</span><span class="sxs-lookup"><span data-stu-id="e66e7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e66e7-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="e66e7-114">**sfc /scannow**</span></span>

<span data-ttu-id="e66e7-115">Po to, kai ši komanda baigia darbą, iš naujo paleiskite kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="e66e7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e66e7-116">Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau "klaida suaktyvinus Office iš Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e66e7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>