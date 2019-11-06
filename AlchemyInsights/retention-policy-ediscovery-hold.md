---
title: 2609 – sulaikymo arba-eDiscovery sulaikymas
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994080"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="eac41-102">Nepavyksta panaikinti elementus "SharePoint Online" arba "OneDrive" verslui</span><span class="sxs-lookup"><span data-stu-id="eac41-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="eac41-103">Jūs arba jūsų vartotojai gali nepavykti panaikinti elementų "SharePoint Online" arba "OneDrive" verslui, nes saugojimo strategija, saugojimo etiketė arba "eDiscovery" sulaikymas taikomas SharePoint "OneDrive" svetainėje arba tam tikrų elementų.</span><span class="sxs-lookup"><span data-stu-id="eac41-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="eac41-104">Tai reiškia, kad negalite panaikinti dokumento, dokumento versijos, aplanko, dokumentų bibliotekos, sąrašo, programėlės, svetainės arba svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="eac41-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="eac41-105">Toliau pateikti keli klaidų pranešimų, kuriuos gavote, jei bandysite panaikinti išsaugomas prekes, pavyzdžiai:</span><span class="sxs-lookup"><span data-stu-id="eac41-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="eac41-106">"Šios svetainės negalima panaikinti, nes ji įtraukta į el. duomenų aptikimo sulaikymo ar saugojimo strategiją"</span><span class="sxs-lookup"><span data-stu-id="eac41-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="eac41-107">"Šios svetainės atitikties strategija nustatyta blokuoti naikinimą"</span><span class="sxs-lookup"><span data-stu-id="eac41-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="eac41-108">"Atitikties strategija šiuo metu blokuoja šios svetainės naikinimas"</span><span class="sxs-lookup"><span data-stu-id="eac41-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="eac41-109">"Šio svetainių rinkinio negalima panaikinti, nes jame yra svetainių, įtrauktų į el. duomenų aptikimo sulaikymo arba saugojimo strategiją"</span><span class="sxs-lookup"><span data-stu-id="eac41-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="eac41-110">"Jūs turite ištrinti visus elementus šiame aplanke prieš ištrynus aplanką"</span><span class="sxs-lookup"><span data-stu-id="eac41-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="eac41-111">"Šio elemento versijų negalima panaikinti, nes ji yra sulaikymas arba saugojimo strategija"</span><span class="sxs-lookup"><span data-stu-id="eac41-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="eac41-112">"Negalima panaikinti elemento laikydami"</span><span class="sxs-lookup"><span data-stu-id="eac41-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="eac41-113">"Etiketės, kuri yra taikoma šiam elementui neleidžia redaguoti arba panaikinti"</span><span class="sxs-lookup"><span data-stu-id="eac41-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="eac41-114">"Negalima panaikinti sąrašo sulaikymo arba saugojimo strategija"</span><span class="sxs-lookup"><span data-stu-id="eac41-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="eac41-115">"Sąrašo panaikinti negalima, jei jis užblokuotas arba jei jam taikoma saugojimo strategija"</span><span class="sxs-lookup"><span data-stu-id="eac41-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="eac41-116">Norint panaikinti elementus viename iš šių scenarijų, turi būti pašalinta saugojimo strategija, saugojimo žymė arba eDiscovery (arba svetainė turi būti pašalinta iš saugojimo strategijos).</span><span class="sxs-lookup"><span data-stu-id="eac41-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="eac41-117">Jums reikia arba išjungti atitinkamą palaikykite tai sukelia šią problemą.</span><span class="sxs-lookup"><span data-stu-id="eac41-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="eac41-118">Pašalinus saugojimo strategiją arba sulaikymą, gali užtrukti iki 24 valandų, kol pakeitimas įsigalios.</span><span class="sxs-lookup"><span data-stu-id="eac41-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="eac41-119">Informacijos apie skirtingas saugojimo ir sulaikymo funkcijas, kurios gali būti pritaikytos SharePoint svetainėms ir "OneDrive" abonementams, ieškokite vienoje iš šių temų.</span><span class="sxs-lookup"><span data-stu-id="eac41-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="eac41-120">Saugojimo strategijos apžvalga</span><span class="sxs-lookup"><span data-stu-id="eac41-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="eac41-121">Saugojimo etikečių apžvalga</span><span class="sxs-lookup"><span data-stu-id="eac41-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="eac41-122">Tvarkyti sulaikymus "Advanced eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="eac41-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="eac41-123">eDiscovery turi</span><span class="sxs-lookup"><span data-stu-id="eac41-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="eac41-124">Senstelėjusios svetainės uždarymo ir naikinimo strategijos</span><span class="sxs-lookup"><span data-stu-id="eac41-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
