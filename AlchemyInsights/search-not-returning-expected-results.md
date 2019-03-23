---
title: 1491-Search-not-Returning-Expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776089"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="8d5a0-102">Turinio paieška negrįžta laukiami rezultatai</span><span class="sxs-lookup"><span data-stu-id="8d5a0-102">Content Search not returning expected results</span></span>

<span data-ttu-id="8d5a0-103">Kai veikia turinio paieškų iš "Office 365" sauga & atitikties užtikrinimo centre, gaunate netikėtas paieškos rezultatus.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="8d5a0-104">Apsvarstyti šiuos dalykus, kurie gali turėti įtakos jūsų paieškos rezultatai:</span><span class="sxs-lookup"><span data-stu-id="8d5a0-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="8d5a0-105">**Turinio vietos ir ieškos sąlygų**: įsitikinkite, kad pasirinkote tinkamą turinio vietas ir paieškos sąlygas.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="8d5a0-106">Jei jūs paleidote didelis paieškos (daugelyje vietų) su, mano padalijant ją į keletą paieškų.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="8d5a0-107">**Iš dalies indeksuoti elementus**: [iš dalies indeksuoti elementus](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iš pašto dėžutės yra įtrauktos į numatomą paieškos rezultatus.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="8d5a0-108">Vis dėlto iš dalies indeksuoti elementus iš SharePoint ir "OneDrive" neįtraukiami į ieškos įvertinimą.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="8d5a0-109">**Paieška gedimai**: ieškant daug pašto dėžučių (daugiau nei 100 000 pašto dėžučių), galite gauti paieškos klaidas, klaidų kodai, pvz., CS008-009 ir CS012-002).</span><span class="sxs-lookup"><span data-stu-id="8d5a0-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="8d5a0-110">Šiuo atveju, bandykite dar kartą ieškoti tik nepavyko turinio vietas.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="8d5a0-111">Skaitykite [šį straipsnį](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="8d5a0-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
