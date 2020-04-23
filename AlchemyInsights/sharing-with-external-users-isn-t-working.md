---
title: Bendrinimas su išoriniais vartotojais neveikia
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767257"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="d6445-102">"SharePoint" turinio bendrinimo su išoriniais vartotojais problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="d6445-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="d6445-103">Įsitikinkite, kad jūsų organizacijai įjungtas išorinis bendrinimas:</span><span class="sxs-lookup"><span data-stu-id="d6445-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="d6445-104">Eikite į [ &amp; "Microsoft 365" administravimo centro puslapį Tarnybos priedai](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ir spustelėkite **Svetainės**.</span><span class="sxs-lookup"><span data-stu-id="d6445-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="d6445-105">Įsitikinkite, kad parametras įjungtas į "Įjungta".</span><span class="sxs-lookup"><span data-stu-id="d6445-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="d6445-106">Jei pasirinkta "Tik esami išoriniai vartotojai", įsitikinkite, kad išorinis vartotojas yra nurodytas "Microsoft 365" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="d6445-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="d6445-107">Įsitikinkite, kad svetainės išorinis bendrinimas įjungtas.</span><span class="sxs-lookup"><span data-stu-id="d6445-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="d6445-108">Klasikiniam svetainių rinkiniui:</span><span class="sxs-lookup"><span data-stu-id="d6445-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="d6445-109">Naujo "SharePoint" administravimo centro kairiojoje srityje spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="d6445-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="d6445-110">Pažymėkite svetainę arba svetaines ir juostelėje spustelėkite **Bendrinimas**.</span><span class="sxs-lookup"><span data-stu-id="d6445-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="d6445-111">Komandos svetainei, priklausančiai "Office 365" grupei arba ryšių svetainei:</span><span class="sxs-lookup"><span data-stu-id="d6445-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="d6445-112">Šie nauji svetainių tipai turi tą patį bendrinimo parametrą kaip ir visos organizacijos parametras, nebent visos organizacijos parametras leidžia bendrinti failus naudojant saitus, kuriems nereikia prisijungimo.</span><span class="sxs-lookup"><span data-stu-id="d6445-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="d6445-113">Tokiu atveju svetainės leidžia bendrinti su naujais ir esamais išoriniais vartotojais, kurie prisijungia.</span><span class="sxs-lookup"><span data-stu-id="d6445-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="d6445-114">Norėdami pakeisti konkrečių svetainių parametrą, naudokite naują "SharePoint" administravimo centrą arba "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="d6445-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="d6445-115">[Sužinokite daugiau](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="d6445-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="d6445-116">Bet kurios svetainės išorinio bendrinimo parametras gali būti labiau ribojantis nei visos organizacijos parametras, bet ne labiau leistinus nei visos organizacijos parametras.</span><span class="sxs-lookup"><span data-stu-id="d6445-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

