---
title: Dynamics 365 – neteisinga ataskaitų srities rodoma "Dynamics 365" bendroji sąsaja
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711283"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="0bf05-102">Neteisinga ataskaitų srities rodoma Dynamics 365 bendroji sąsaja</span><span class="sxs-lookup"><span data-stu-id="0bf05-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="0bf05-103">Yra kelios priežastys, kodėl galite matyti kitokią ataskaitų sritį nei tikitės:</span><span class="sxs-lookup"><span data-stu-id="0bf05-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="0bf05-104">Vartotojas nustatė vartotojo numatytąjį ataskaitų sritį</span><span class="sxs-lookup"><span data-stu-id="0bf05-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="0bf05-105">Paprastai galite nustatyti vartotojo numatytąjį ataskaitų sritį, jei mygtukas **nustatyti kaip numatytąjį** nerodomas ataskaitų srities komandų juostoje.</span><span class="sxs-lookup"><span data-stu-id="0bf05-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="0bf05-106">Vartotojo numatytoji ataskaitų sritis pakeis visas kitas numatytąsias ataskaitų sritis, net jei vartotojo numatytosios ataskaitų srities nėra dabartinėje taikomojoje programoje.</span><span class="sxs-lookup"><span data-stu-id="0bf05-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="0bf05-107">Norėdami panaikinti numatytąjį ataskaitų sritį, naudokite šį sprendimo būdą.</span><span class="sxs-lookup"><span data-stu-id="0bf05-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="0bf05-108">Kurti naują asmeninį ataskaitų sritį.</span><span class="sxs-lookup"><span data-stu-id="0bf05-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="0bf05-109">Nustatyti naują ataskaitų sritį kaip numatytąjį vartotojo.</span><span class="sxs-lookup"><span data-stu-id="0bf05-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="0bf05-110">Naikinti tą ataskaitų sritį.</span><span class="sxs-lookup"><span data-stu-id="0bf05-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="0bf05-111">Ataskaitų sritis nustatyta struktūra</span><span class="sxs-lookup"><span data-stu-id="0bf05-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="0bf05-112">Galbūt nustatėte organizacijos numatytąją ataskaitų sritį pasirinkdami ataskaitų sritį ir pasirinkę "nustatyti kaip numatytąjį" dalyje "tinkinti sistemą".</span><span class="sxs-lookup"><span data-stu-id="0bf05-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="0bf05-113">Tačiau, jei vartotojas turi prieigą prie šio ataskaitų srities, pagal šią ataskaitų sritį bus teikiama pirmenybė schemos dizaino įrankyje.</span><span class="sxs-lookup"><span data-stu-id="0bf05-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="0bf05-114">Jei norite, kad vartotojai matytų ataskaitų sritį, kurią nustatėte kaip numatytąjį organizacijos, galite:</span><span class="sxs-lookup"><span data-stu-id="0bf05-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="0bf05-115">Nustatyti, kad ataskaitų sritis būtų "Sitemap"</span><span class="sxs-lookup"><span data-stu-id="0bf05-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="0bf05-116">Prieigos prie "Sitemap" apibrėžtosios ataskaitų srities pašalinimas tiems vartotojams</span><span class="sxs-lookup"><span data-stu-id="0bf05-116">Remove access to the sitemap defined dashboard for those users</span></span>
