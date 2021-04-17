---
title: MC210173 – „SharePoint Designer“ naujos pasirinktinės formos funkcijos atsisakymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831814"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="73193-102">MC210173 – „SharePoint Designer“ naujos pasirinktinės formos funkcijos atsisakymas</span><span class="sxs-lookup"><span data-stu-id="73193-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="73193-103">Nustatėme problemą, kuri turi įtakos „SharePoint Designer“ veikimui [kuriant pasirinktines formas](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) naudojant „SharePoint Online“.</span><span class="sxs-lookup"><span data-stu-id="73193-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="73193-104">Atlikę kruopštų tikrinimą nustatėme, kad nėra žinomos šios problemos pataisos ir pasirinkote išjungti pasirinktinės formų kūrimo funkciją, 2020 m. balandžio 25 d., šeštadienio, 3:00 val. UTC.</span><span class="sxs-lookup"><span data-stu-id="73193-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="73193-105">Šis pakeitimas nedaro įtakos galimybei redaguoti anksčiau sukurtas formas ar kitas esamas „SharePoint Online Designer“ funkcijas.</span><span class="sxs-lookup"><span data-stu-id="73193-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="73193-106">Atlikus šį keitimą vartotojai, kurdami naujas formas, gali gauti klaidos pranešimą: „Nepavyko įrašyti sąrašo pakeitimų serveryje“.</span><span class="sxs-lookup"><span data-stu-id="73193-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="73193-107">Vartotojai, kurie anksčiau naudojo „SharePoint Designer“ kurdami pasirinktines formas, gali naudoti [„PowerApps“](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="73193-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="73193-108">„PowerApps“ yra paprastas ir efektyvus įrankis, kuris leidžia „SharePoint Online Modern“ vartotojams kurti bei redaguoti pasirinktines formas, skirtas „SharePoint“ sąrašams ir dokumentų bibliotekoms, tiesiai iš naršyklės lango.</span><span class="sxs-lookup"><span data-stu-id="73193-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="73193-109">„PowerApps“ nereikalauja tradicinių programavimo žinių arba papildomų programų, pvz., „InfoPath“.</span><span class="sxs-lookup"><span data-stu-id="73193-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="73193-110">**Pastaba**: „SharePoint Online Classic“ vartotojams reikės laikinai pereiti prie „Modern“ patirties, kad galėtų pasiekti ir naudoti „PowerApps“; nors visos pasirinktinės formos, sukurtos „PowerApps“, pasiekiamos „SharePoint Online Classic“ vartotojams.</span><span class="sxs-lookup"><span data-stu-id="73193-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
