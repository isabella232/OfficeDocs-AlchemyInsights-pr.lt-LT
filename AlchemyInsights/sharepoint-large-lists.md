---
title: "\"SharePoint\" didieji sąrašai"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720141"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="634c2-102">Darbas su dideliais sąrašais ir bibliotekomis programoje "SharePoint"</span><span class="sxs-lookup"><span data-stu-id="634c2-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="634c2-103">"SharePoint" sąrašuose ir bibliotekose gali būti iki "30 000 000" elementų, tačiau kai jie turi daugiau nei 5 000 elementų, galite matyti sąrašo rodinio ribinės klaidą, kai bandysite dirbti su jais.</span><span class="sxs-lookup"><span data-stu-id="634c2-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="634c2-104">Ši riba yra įdiegta norint užtikrinti tinkamą paslaugos teikimą.</span><span class="sxs-lookup"><span data-stu-id="634c2-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="634c2-105">Jos keisti negalima.</span><span class="sxs-lookup"><span data-stu-id="634c2-105">It can't be changed.</span></span> <span data-ttu-id="634c2-106">Norėdami išvengti šio slenksčio:</span><span class="sxs-lookup"><span data-stu-id="634c2-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="634c2-107">**Naudokite šiuolaikines**</span><span class="sxs-lookup"><span data-stu-id="634c2-107">**Use modern**</span></span>

<span data-ttu-id="634c2-108">Rodiniai, rodantys, kad daug elementų geriausiai tinka šiuolaikinėje naudojimo srityje.</span><span class="sxs-lookup"><span data-stu-id="634c2-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="634c2-109">[Naudokite šiuolaikinę patirtį](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , kad išvengtumėte klaidų, kurias galite matyti naudodami klasikinę patirtį.</span><span class="sxs-lookup"><span data-stu-id="634c2-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="634c2-110">**Įtraukti indeksus**</span><span class="sxs-lookup"><span data-stu-id="634c2-110">**Add indexes**</span></span>

<span data-ttu-id="634c2-111">Kai filtruojate arba rikiuojate pagal stulpelį, kuris neturi indekso, galite matyti klaidos pranešimą.</span><span class="sxs-lookup"><span data-stu-id="634c2-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="634c2-112">[Įtraukite indeksą](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) neautomatiškai iš **sąrašo parametrų** meniu parametrai, tada **indeksuotus stulpelius**.</span><span class="sxs-lookup"><span data-stu-id="634c2-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="634c2-113">**Sąrašo rodinio redagavimas**</span><span class="sxs-lookup"><span data-stu-id="634c2-113">**Edit the list view**</span></span>

<span data-ttu-id="634c2-114">Jei įvyksta klaida dirbant su dideliu sąrašu, [redaguokite savo sąrašo rodinį](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="634c2-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="634c2-115">Šie keturi pokyčiai pašalins sąrašo rodinio ribinių klaidų.</span><span class="sxs-lookup"><span data-stu-id="634c2-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="634c2-116">Atlikite visus keturis visų klaidų šalinimo pakitimus.</span><span class="sxs-lookup"><span data-stu-id="634c2-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="634c2-117">Jei vis dar gaunate klaidų, pažymėkite [valdyti dideles sąrašus ir bibliotekas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="634c2-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="634c2-118">Pasirinkite **nėra** iš **pirmo rūšiavimo pagal stulpelį** ir **tada Rikiuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="634c2-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="634c2-119">Pažymėkite **nėra** iš **pirmos grupės pagal stulpelį** ir **tada Grupuoti pagal stulpelį**.</span><span class="sxs-lookup"><span data-stu-id="634c2-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="634c2-120">Dalyje **sumos** pasirinkite **nėra** visiems stulpeliams.</span><span class="sxs-lookup"><span data-stu-id="634c2-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="634c2-121">Atžymėti visus, išskyrus vieną stulpelį, kuris rodomas sekcijoje **stulpeliai** .</span><span class="sxs-lookup"><span data-stu-id="634c2-121">Deselect all but one column for display from the **Columns** section.</span></span>

