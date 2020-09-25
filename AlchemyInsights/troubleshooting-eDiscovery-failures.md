---
title: 1490 – trikčių diagnostika – "Udiscovery" – gedimai
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277832"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="12d82-102">Turinio ieškos klaidų šalinimas</span><span class="sxs-lookup"><span data-stu-id="12d82-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="12d82-103">Ar susiduriate su problemomis dėl turinio ieškos arba gaunate gedimus, kai eksportuojate ieškos rezultatus?</span><span class="sxs-lookup"><span data-stu-id="12d82-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="12d82-104">Pavyzdžiui, ar vykdydami iešką gaunate šiuos veiksmus?</span><span class="sxs-lookup"><span data-stu-id="12d82-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="12d82-105">CS008 arba CS012 klaidos</span><span class="sxs-lookup"><span data-stu-id="12d82-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="12d82-106">Serverio užimtas/skirtojo laiko klaidos</span><span class="sxs-lookup"><span data-stu-id="12d82-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="12d82-107">Įvyko taikomosios programos klaida</span><span class="sxs-lookup"><span data-stu-id="12d82-107">Application error occurred</span></span>

<span data-ttu-id="12d82-108">Arba, kai ieškote ar eksportuojate rezultatus iš daugybės pašto dėžučių (virš "100 000" pašto dėžučių), ar gaunate eksportavimo klaidų?</span><span class="sxs-lookup"><span data-stu-id="12d82-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="12d82-109">Šio tipo klaidoms bandykite dar kartą ieškoti nepavykusių turinio vietų.</span><span class="sxs-lookup"><span data-stu-id="12d82-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="12d82-110">Daugiau informacijos rasite  [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="12d82-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="12d82-111">Jei eksportuojate daugiau nei 100 k pašto dėžučių, turite naudoti šį "PowerShell", kad atsisiųstumėte eksportavimo rezultatus:  [rezultatų eksportavimas iš daugiau nei 100 k pašto dėžučių](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="12d82-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
