---
title: Dynamics 365 - negerai prietaisų skydelyje rodo Dynamics 365 vieningą sąsają
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528559"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="b393f-102">Neteisingas prietaisų skydelyje rodo Dynamics 365 vieningą sąsają</span><span class="sxs-lookup"><span data-stu-id="b393f-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="b393f-103">Yra kelios priežastys, kodėl galite matyti skirtingas ataskaitų srities nei tikitės:</span><span class="sxs-lookup"><span data-stu-id="b393f-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="b393f-104">Vartotojas turi nustatyti vartotojo numatytąją įrankių juostos</span><span class="sxs-lookup"><span data-stu-id="b393f-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="b393f-105">Paprastai, galite nustatyti vartotojo numatytąją įrankių juostos yra nustatytas jei mygtuką **Nustatyti kaip numatytąjį** nerodo skydelis komandų juostą.</span><span class="sxs-lookup"><span data-stu-id="b393f-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="b393f-106">Vartotojo numatytąją įrankių juostos bus perrašyti visi kitų numatytąjį skelbimų lentos, net jei vartotojo numatytąją įrankių juostos nėra esamos programos.</span><span class="sxs-lookup"><span data-stu-id="b393f-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="b393f-107">Naudokite šiuos problemos Norėdami išjungti savo numatytąją įrankių juostos.</span><span class="sxs-lookup"><span data-stu-id="b393f-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="b393f-108">Sukurti naują asmens ataskaitų sritis.</span><span class="sxs-lookup"><span data-stu-id="b393f-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="b393f-109">Skirti, naujas Panel numatytuoju vartotojo.</span><span class="sxs-lookup"><span data-stu-id="b393f-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="b393f-110">Panaikinti kad prietaisų skydelio.</span><span class="sxs-lookup"><span data-stu-id="b393f-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="b393f-111">Prietaisų skydelyje yra įsikūrę sitemap</span><span class="sxs-lookup"><span data-stu-id="b393f-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="b393f-112">Kuriuos galite būti nustatę organizacijos numatytąją įrankių juostos pasirinkdami skydelyje ir pasirinkti "Nustatyti kaip numatytąjį" pagal "Tinkinti sistema".</span><span class="sxs-lookup"><span data-stu-id="b393f-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="b393f-113">Tačiau apibrėžta svetainės dizaineris prietaisų skydelyje bus pirmenybė per šią ataskaitų sritį, jei vartotojas turi prieigą prie jo.</span><span class="sxs-lookup"><span data-stu-id="b393f-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="b393f-114">Norėdami peržiūrėti nustatėte kaip numatytąjį organizacijos prietaisų skydelio, galite:</span><span class="sxs-lookup"><span data-stu-id="b393f-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="b393f-115">Nustatyti kad prietaisų skydelio struktūra</span><span class="sxs-lookup"><span data-stu-id="b393f-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="b393f-116">Panaikinti prieigą prie svetainės struktūra, apibrėžti skydelio tiems vartotojams</span><span class="sxs-lookup"><span data-stu-id="b393f-116">Remove access to the sitemap defined dashboard for those users</span></span>
