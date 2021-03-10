---
title: Geriausios išplėstinės medžioklės užklausų praktikos taikymas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696077"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="6b5be-102">Geriausios išplėstinės medžioklės užklausų praktikos taikymas</span><span class="sxs-lookup"><span data-stu-id="6b5be-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="6b5be-103">Norėdami greičiau gauti rezultatus ir išvengti skirtojo laiko vykdydami sudėtingas užklausas, taikykite šias geriausias praktikas:</span><span class="sxs-lookup"><span data-stu-id="6b5be-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="6b5be-104">Bandant naujas užklausas, visada naudokite apribojimą, kad būtų išvengta itin didelės rezultatų rinkinių.</span><span class="sxs-lookup"><span data-stu-id="6b5be-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="6b5be-105">Taip pat naudokite `count` Norėdami atlikti pradinį rezultatų rinkinio dydžio vertinimą.</span><span class="sxs-lookup"><span data-stu-id="6b5be-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="6b5be-106">Pirmiausia naudokite laiko filtrus.</span><span class="sxs-lookup"><span data-stu-id="6b5be-106">Use time filters first.</span></span> <span data-ttu-id="6b5be-107">Idealiu atveju Apribokite savo užklausas iki septynių dienų.</span><span class="sxs-lookup"><span data-stu-id="6b5be-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="6b5be-108">Užklausos pradžioje, iškart po laiko filtro, įtraukite filtrus, kuriuos tikimasi pašalinti didžiąją dalį duomenų.</span><span class="sxs-lookup"><span data-stu-id="6b5be-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="6b5be-109">Ieškodami visiškai žetonų naudokite `has` operatorių, o ne `contains` .</span><span class="sxs-lookup"><span data-stu-id="6b5be-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="6b5be-110">Vykdykite iešką konkrečiame stulpelyje, o ne visuose stulpeliuose.</span><span class="sxs-lookup"><span data-stu-id="6b5be-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="6b5be-111">Kai sujungiame lenteles, pirmiausia apibrėžkite lentelę, kurioje yra mažiau eilučių.</span><span class="sxs-lookup"><span data-stu-id="6b5be-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="6b5be-112">`project` tik reikiamus stulpelius iš lentelių, kurias sujungėte.</span><span class="sxs-lookup"><span data-stu-id="6b5be-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="6b5be-113">Norėdami sužinoti daugiau, peržiūrėkite [pažangiausių medžioklės užklausų geriausios praktikos](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="6b5be-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
