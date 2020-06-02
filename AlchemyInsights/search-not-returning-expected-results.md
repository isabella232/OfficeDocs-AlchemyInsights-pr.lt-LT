---
title: 1491-paieškos ne grįžtant laukiami rezultatai
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510580"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="4cc21-102">Turinio ieška nepateikia numatomų rezultatų</span><span class="sxs-lookup"><span data-stu-id="4cc21-102">Content Search not returning expected results</span></span>

<span data-ttu-id="4cc21-103">Kai vykdote turinio ieškas iš "Microsoft 365" saugos & atitikties centro, galite gauti netikėtų ieškos rezultatų.</span><span class="sxs-lookup"><span data-stu-id="4cc21-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="4cc21-104">Apsvarstykite šiuos dalykus, kurie gali turėti įtakos ieškos rezultatams:</span><span class="sxs-lookup"><span data-stu-id="4cc21-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="4cc21-105">**Turinio vietos ir paieškos sąlygos**: įsitikinkite, kad pasirinkote tinkamas turinio vietas ir paieškos sąlygas.</span><span class="sxs-lookup"><span data-stu-id="4cc21-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="4cc21-106">Jei vykdėte didelę paiešką (su daugeliu vietų), apsvarstykite galimybę ją skaidyti į kelias paieškas.</span><span class="sxs-lookup"><span data-stu-id="4cc21-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="4cc21-107">**Iš dalies indeksuoti elementai:** [iš dalies indeksuoti pašto](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dėžučių elementai įtraukiami į įvertintus ieškos rezultatus.</span><span class="sxs-lookup"><span data-stu-id="4cc21-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="4cc21-108">Tačiau iš dalies indeksuoti elementai iš "SharePoint" ir "OneDrive" svetainių neįtraukiami į ieškos įvertinimą.</span><span class="sxs-lookup"><span data-stu-id="4cc21-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="4cc21-109">**Ieškos triktys**: ieškodami daug pašto dėžučių (daugiau nei 100 000 pašto dėžučių), galite gauti ieškos klaidų, naudodami klaidų kodus, pvz., CS008-009 ir CS012-002).</span><span class="sxs-lookup"><span data-stu-id="4cc21-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="4cc21-110">Tokiu atveju bandykite ieškoti tik nepavyko turinio vietose.</span><span class="sxs-lookup"><span data-stu-id="4cc21-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="4cc21-111">Daugiau informacijos rasite [šiame straipsnyje.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)</span><span class="sxs-lookup"><span data-stu-id="4cc21-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
