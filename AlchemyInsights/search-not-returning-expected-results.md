---
title: 1491 – ieška – ne – grąžinimas – tikėtasi – rezultatai
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740482"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="98044-102">Turinio ieška negrąžina laukiamų rezultatų</span><span class="sxs-lookup"><span data-stu-id="98044-102">Content Search not returning expected results</span></span>

<span data-ttu-id="98044-103">Vykdydami turinio iešką "Microsoft" 365 saugos & atitikties centre, galite gauti netikėtų ieškos rezultatų.</span><span class="sxs-lookup"><span data-stu-id="98044-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="98044-104">Apsvarstykite šiuos dalykus, kurie gali turėti įtakos jūsų ieškos rezultatams:</span><span class="sxs-lookup"><span data-stu-id="98044-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="98044-105">**Turinio vietos ir ieškos sąlygos**: įsitikinkite, kad pažymėjote tinkamas turinio vietas ir ieškos sąlygas.</span><span class="sxs-lookup"><span data-stu-id="98044-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="98044-106">Jei susidūrėte su didele ieška (keliose vietose), apsvarstykite, ar nereikėtų jos suskaidyti į kelias paieškas.</span><span class="sxs-lookup"><span data-stu-id="98044-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="98044-107">**Iš dalies indeksuoti elementai**: iš  [dalies indeksuoti elementai](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iš pašto dėžučių įtraukiami į numatomus ieškos rezultatus.</span><span class="sxs-lookup"><span data-stu-id="98044-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="98044-108">Tačiau iš dalies indeksuoti elementai iš svetainių, esančių "SharePoint" ir "OneDrive", neįtraukiami į ieškos įvertinimą.</span><span class="sxs-lookup"><span data-stu-id="98044-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="98044-109">**Ieškos triktys**: ieškodami daug pašto dėžučių (virš "100 000" pašto dėžučių), galite gauti ieškos klaidų ir klaidų kodus, pvz., CS008 – 009 ir CS012-002).</span><span class="sxs-lookup"><span data-stu-id="98044-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="98044-110">Šiuo atveju bandykite ieškoti tik nepavykusių turinio vietų.</span><span class="sxs-lookup"><span data-stu-id="98044-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="98044-111">Daugiau informacijos rasite  [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="98044-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
