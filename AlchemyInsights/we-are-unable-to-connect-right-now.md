---
title: Aktyvinimo problema – šiuo metu negalime prisijungti
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806450"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="702e4-102">"Microsoft 365" programų "Mes negalime prisijungti dabar" pranešimo taisymo</span><span class="sxs-lookup"><span data-stu-id="702e4-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="702e4-103">Jei gaunate šį pranešimą, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="702e4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="702e4-104">Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Microsoft 365" programų.</span><span class="sxs-lookup"><span data-stu-id="702e4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="702e4-105">Žr. ["Microsoft" URL ir IP adresų diapazonai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="702e4-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="702e4-106">Eikite **į Pradėti**  >  **vykdyti**, tada įveskite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="702e4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="702e4-107">Įsitikinkite, kad visos šios tarnybos veikia:</span><span class="sxs-lookup"><span data-stu-id="702e4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="702e4-108">Tinklo prijungtų įrenginių automatinis nustatymas</span><span class="sxs-lookup"><span data-stu-id="702e4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="702e4-109">Tinklo sąrašo tarnyba</span><span class="sxs-lookup"><span data-stu-id="702e4-109">Network List Service</span></span>
    - <span data-ttu-id="702e4-110">Tinklo vietos žinomumas</span><span class="sxs-lookup"><span data-stu-id="702e4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="702e4-111">"Windows" įvykių žurnalas</span><span class="sxs-lookup"><span data-stu-id="702e4-111">Windows Event Log</span></span>

<span data-ttu-id="702e4-112">Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti.</span><span class="sxs-lookup"><span data-stu-id="702e4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="702e4-113">Jei kyla problemų pradedant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę su didesnėmis teisėmis:</span><span class="sxs-lookup"><span data-stu-id="702e4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="702e4-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="702e4-114">**sfc /scannow**</span></span>

<span data-ttu-id="702e4-115">Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.</span><span class="sxs-lookup"><span data-stu-id="702e4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="702e4-116">Išsamios informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai suaktyvinsite "Office" iš "Microsoft 365".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="702e4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>