---
title: Aktyvinimas problema-mes negalime prisijungti dabar
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628250"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="0d67a-102">"Office" programų taisymas "mes negalime prisijungti dabar" pranešimas</span><span class="sxs-lookup"><span data-stu-id="0d67a-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="0d67a-103">Jei gavote šį pranešimą, išbandykite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="0d67a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0d67a-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Office" programėlių.</span><span class="sxs-lookup"><span data-stu-id="0d67a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="0d67a-105">Peržiūrėkite " [Office 365" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="0d67a-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0d67a-106">Eikite į **pradėti** > **vykdyti**, tada įveskite **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="0d67a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0d67a-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="0d67a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0d67a-108">Tinklo prijungtų įrenginių Automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="0d67a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0d67a-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="0d67a-109">Network List Service</span></span>
    - <span data-ttu-id="0d67a-110">Tinklo vieta sąmoningumo</span><span class="sxs-lookup"><span data-stu-id="0d67a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0d67a-111">"Windows" įvykių žurnale</span><span class="sxs-lookup"><span data-stu-id="0d67a-111">Windows Event Log</span></span>

<span data-ttu-id="0d67a-112">Jei viena iš šių paslaugų nepaleista, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="0d67a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0d67a-113">Jei turite problemų pradedant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę su didesnių teisių:</span><span class="sxs-lookup"><span data-stu-id="0d67a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0d67a-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="0d67a-114">**sfc /scannow**</span></span>

<span data-ttu-id="0d67a-115">Po to, kai ši komanda baigia darbą, iš naujo paleiskite kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="0d67a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0d67a-116">Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau "klaida suaktyvinus Office iš Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="0d67a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>