---
title: Dideli "SharePoint" sąrašai
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767293"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="08046-102">Darbas su dideliais sąrašais ir bibliotekomis "SharePoint"</span><span class="sxs-lookup"><span data-stu-id="08046-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="08046-103">SharePoint sąrašuose ir bibliotekose gali būti iki 30 milijonų elementų, tačiau jei juose yra daugiau nei 5 000 elementų, bandydami dirbti su jais galite matyti sąrašo rodinio slenkstį.</span><span class="sxs-lookup"><span data-stu-id="08046-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="08046-104">Ši riba yra įdiegta norint užtikrinti tinkamą paslaugos teikimą.</span><span class="sxs-lookup"><span data-stu-id="08046-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="08046-105">Jos keisti negalima.</span><span class="sxs-lookup"><span data-stu-id="08046-105">It can't be changed.</span></span> <span data-ttu-id="08046-106">Norėdami išvengti pataikyti šią ribą:</span><span class="sxs-lookup"><span data-stu-id="08046-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="08046-107">**Naudokite modernius**</span><span class="sxs-lookup"><span data-stu-id="08046-107">**Use modern**</span></span>

<span data-ttu-id="08046-108">Rodiniai, rodantys daug elementų, geriausiai veikia šiuolaikinėje patirtyje.</span><span class="sxs-lookup"><span data-stu-id="08046-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="08046-109">[Naudokite šiuolaikinę patirtį,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) kad išvengtumėte klaidų, kurios gali būti matytos klasikinėje patirtį.</span><span class="sxs-lookup"><span data-stu-id="08046-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="08046-110">**Įtraukti rodykles**</span><span class="sxs-lookup"><span data-stu-id="08046-110">**Add indexes**</span></span>

<span data-ttu-id="08046-111">Kai filtruojate arba rūšiuojate pagal stulpelį, kuriame nėra rodyklės, gali būti rodomas klaidos pranešimas.</span><span class="sxs-lookup"><span data-stu-id="08046-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="08046-112">[Įtraukite rodyklę](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) rankiniu būdu iš meniu **Parametrai sąrašo parametrai,** tada **Indeksuoti stulpeliai**.</span><span class="sxs-lookup"><span data-stu-id="08046-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="08046-113">**Sąrašo rodinio redagavimas**</span><span class="sxs-lookup"><span data-stu-id="08046-113">**Edit the list view**</span></span>

<span data-ttu-id="08046-114">Jei dirbant su dideliu sąrašu įvyksta klaida, [redaguokite sąrašo rodinį](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="08046-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="08046-115">Šie keturi pakeitimai pašalins sąrašo rodinio slenkstį.</span><span class="sxs-lookup"><span data-stu-id="08046-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="08046-116">Atlikite visus keturis pakeitimus, kad pašalintumėte visas klaidas.</span><span class="sxs-lookup"><span data-stu-id="08046-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="08046-117">Jei vis dar gaunate klaidų, patikrinkite [Tvarkyti didelius sąrašus ir bibliotekas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="08046-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="08046-118">Pasirinkite **Nėra** iš abiejų **Pirma rūšiuoti pagal stulpelį** ir **Tada rūšiuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="08046-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="08046-119">Pasirinkite **Nėra** iš abiejų **Pirmoji grupė pagal stulpelį** ir **Tada grupuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="08046-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="08046-120">Sekcijoje **Sumos** pasirinkite **Nėra** visiems stulpeliams.</span><span class="sxs-lookup"><span data-stu-id="08046-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="08046-121">Panaikinkite visų, išskyrus vieną, **rodymo** stulpelį žymėjimą iš stulpelių skyriaus.</span><span class="sxs-lookup"><span data-stu-id="08046-121">Deselect all but one column for display from the **Columns** section.</span></span>

