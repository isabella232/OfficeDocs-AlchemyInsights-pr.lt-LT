---
title: Diagramoje rodomas skirtingas įrašų skaičius tinklelyje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439351"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="3cf2f-102">Diagramoje rodomas skirtingas įrašų skaičius tinklelyje</span><span class="sxs-lookup"><span data-stu-id="3cf2f-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="3cf2f-103">**Simptomas**</span><span class="sxs-lookup"><span data-stu-id="3cf2f-103">**Symptom**</span></span>

<span data-ttu-id="3cf2f-104">Diagramos ataskaitų srities puslapyje, kai paspausite ant diagramos "..." ir spustelėkite "Peržiūrėti įrašus", pereikite į tinklelio puslapį, kad pamatytumėte visus įrašus. Kartais keičiasi įrašų skaičius.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="3cf2f-105">**Sukelti**</span><span class="sxs-lookup"><span data-stu-id="3cf2f-105">**Cause**</span></span>

<span data-ttu-id="3cf2f-106">Taip yra dėl to, kad pradiniame ataskaitų srities puslapyje esanti diagrama skiriasi nuo tinklelio pagrindinio puslapio diagramos.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="3cf2f-107">**Tirpalas**</span><span class="sxs-lookup"><span data-stu-id="3cf2f-107">**Solution**</span></span>

1. <span data-ttu-id="3cf2f-108">Patikrinkite rodinį iš pradinio puslapio ir tinklelio rodinio, kad sužinotumėte, ar jie skiriasi.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="3cf2f-109">Pakeiskite rodinį tinklelyje, kad jis atitiktų pradinio puslapio rodinį.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="3cf2f-110">Jei tinkamo rodinio rasti nepavyksta, paprastai tai reiškia, kad rodinys neįgalintas programų dizaino įrankyje.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="3cf2f-111">Eikite į konkrečios programos programų dizaino įrankį, pasirinkite objektą ir jo rodinius, patikrinkite rodinį, kurį norite įgalinti, įrašyti, publikuoti ir uždaryti.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="3cf2f-112">Atnaujinkite puslapį.</span><span class="sxs-lookup"><span data-stu-id="3cf2f-112">Refresh the page.</span></span>