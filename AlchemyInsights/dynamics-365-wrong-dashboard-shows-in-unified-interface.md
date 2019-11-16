---
title: Dynamics 365-neteisingas ataskaitų srities rodo Dynamics 365 vieningosios sąsajos
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528559"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="1b7eb-102">Neteisinga ataskaitų srities rodo Dynamics 365 vieningosios sąsajos</span><span class="sxs-lookup"><span data-stu-id="1b7eb-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="1b7eb-103">Yra kelios priežastys, kodėl galite matyti kitą ataskaitų sritį nei tikitės:</span><span class="sxs-lookup"><span data-stu-id="1b7eb-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="1b7eb-104">Vartotojas nustatė vartotojo numatytąjį ataskaitų sritį</span><span class="sxs-lookup"><span data-stu-id="1b7eb-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="1b7eb-105">Paprastai galite nustatyti vartotojo numatytąją ataskaitų sritį, jei mygtukas **nustatyti kaip numatytąjį** nerodomas ataskaitų srities komandų juostoje.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="1b7eb-106">Vartotojo numatytoji ataskaitų sritis pakeis visas kitas numatytąsias ataskaitų sritis, net jei vartotojo numatytoji ataskaitų sritis nėra dabartinėje programėlėje.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="1b7eb-107">Norėdami nustatyti numatytąją ataskaitų sritį, naudokite toliau nurodytą problemos sprendimą.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="1b7eb-108">Sukurkite naują asmeninę ataskaitų sritį.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="1b7eb-109">Nustatykite naują ataskaitų sritį kaip numatytąją vartotojo.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="1b7eb-110">Panaikinkite tą ataskaitų sritį.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="1b7eb-111">Informacijos suvestinė nustatyta svetainės struktūroje</span><span class="sxs-lookup"><span data-stu-id="1b7eb-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="1b7eb-112">Galite nustatyti organizacijos numatytąjį ataskaitų sritį pasirinkdami ataskaitų sritį ir pasirinkę "nustatyti kaip numatytąjį" dalyje "tinkinti sistemą".</span><span class="sxs-lookup"><span data-stu-id="1b7eb-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="1b7eb-113">Bet informacijos suvestinė, nurodyta svetainės struktūros konstruktoriuje, bus viršesnė už šią ataskaitų sritį, jei vartotojas turi prieigą prie jos.</span><span class="sxs-lookup"><span data-stu-id="1b7eb-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="1b7eb-114">Jei norite, kad vartotojai matytų ataskaitų sritį, kurią nustatėte kaip numatytąją organizaciją, galite:</span><span class="sxs-lookup"><span data-stu-id="1b7eb-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="1b7eb-115">Nustatykite ataskaitų sritį svetainės struktūroje</span><span class="sxs-lookup"><span data-stu-id="1b7eb-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="1b7eb-116">Pašalinti prieigą prie svetainės struktūra nustatyta ataskaitų srities tiems vartotojams</span><span class="sxs-lookup"><span data-stu-id="1b7eb-116">Remove access to the sitemap defined dashboard for those users</span></span>
