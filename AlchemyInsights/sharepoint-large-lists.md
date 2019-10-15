---
title: Dideli SharePoint sąrašai
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488525"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="ea0ea-102">Dirbkite su dideliais "SharePoint" sąrašais ir bibliotekomis</span><span class="sxs-lookup"><span data-stu-id="ea0ea-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="ea0ea-103">SharePoint sąrašuose ir bibliotekose gali būti iki 30 000 000 elementų, bet kai juose yra daugiau nei 5 000 elementų, bandant dirbti su jais, gali būti rodoma sąrašo rodinio slenksčio klaida.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="ea0ea-104">Ši ribinė vertė yra skirta paslaugos veikimui užtikrinti.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="ea0ea-105">Jo keisti negalima.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-105">It can't be changed.</span></span> <span data-ttu-id="ea0ea-106">Norėdami išvengti pataikyti šią ribą:</span><span class="sxs-lookup"><span data-stu-id="ea0ea-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="ea0ea-107">**Naudokitės modernia**</span><span class="sxs-lookup"><span data-stu-id="ea0ea-107">**Use modern**</span></span>

<span data-ttu-id="ea0ea-108">Rodiniai, rodantys daug daiktų, geriausiai veikia modernioje patirčiai.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="ea0ea-109">[Pasinaudokite modernia patirtimi](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , kad išvengtumėte klaidų, kurias galite matyti klasikinėje patirčiai.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="ea0ea-110">**Indeksų pridėjimas**</span><span class="sxs-lookup"><span data-stu-id="ea0ea-110">**Add indexes**</span></span>

<span data-ttu-id="ea0ea-111">Kai filtruojate arba rikiuojate stulpelį, kuriame nėra rodyklės, gali būti rodomas klaidos pranešimas.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="ea0ea-112">[Įtraukite indeksą](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) neautomatiniu būdu iš **sąrašo parametrai** nustatymų meniu, tada **indeksuojami stulpeliai**.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="ea0ea-113">**Sąrašo rodinio redagavimas**</span><span class="sxs-lookup"><span data-stu-id="ea0ea-113">**Edit the list view**</span></span>

<span data-ttu-id="ea0ea-114">Jei klaida įvyksta dirbant su dideliu sąrašu, [redaguokite savo sąrašo rodinį](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="ea0ea-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="ea0ea-115">Šie keturi pakeitimai bus pašalinti sąrašo rodinio slenksčio klaidas.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="ea0ea-116">Atlikite visus keturis pakeitimus, kad pašalintumėte visas klaidas.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="ea0ea-117">Jei vis dar gaunate klaidų, patikrinkite [valdyti didelius sąrašus ir bibliotekas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="ea0ea-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="ea0ea-118">Pasirinkite **nė vienas** iš **pirma rūšiuoti pagal stulpelį** ir **tada Rūšiuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="ea0ea-119">Pasirinkite **nė vienas** iš **pirmosios grupės stulpelyje** ir **tada Grupuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="ea0ea-120">Pasirinkite **nėra** visiems stulpelių **sumos** sekcijoje.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="ea0ea-121">Panaikinkite žymėjimą visiems, išskyrus vieną stulpelį, skirtą Rodyti iš **stulpelių** sekcijos.</span><span class="sxs-lookup"><span data-stu-id="ea0ea-121">Deselect all but one column for display from the **Columns** section.</span></span>

