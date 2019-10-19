---
title: Neveikia bendrinimas su išoriniais vartotojais
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502239"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="b6e37-102">SharePoint turinio bendrinimo su išoriniais vartotojais problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="b6e37-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="b6e37-103">Įsitikinkite, kad jūsų organizacijoje įjungtas Išorinis bendrinimas:</span><span class="sxs-lookup"><span data-stu-id="b6e37-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="b6e37-104">Eikite į ["Microsoft &amp; " 365 administravimo centro puslapį tarnybos papildiniai](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ir spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="b6e37-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="b6e37-105">Įsitikinkite, kad parametras yra įjungtas į "įjungta".</span><span class="sxs-lookup"><span data-stu-id="b6e37-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="b6e37-106">Jei pasirinkta "tik esami Išoriniai vartotojai", įsitikinkite, kad išorinis vartotojas yra nurodytas "Microsoft" 365 administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="b6e37-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="b6e37-107">Įsitikinkite, kad svetainėje įjungtas Išorinis bendrinimas.</span><span class="sxs-lookup"><span data-stu-id="b6e37-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="b6e37-108">Klasikiniam svetainių rinkiniui:</span><span class="sxs-lookup"><span data-stu-id="b6e37-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="b6e37-109">Naujame SharePoint administravimo centre kairiojoje srityje spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="b6e37-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="b6e37-110">Pasirinkite svetainę ar svetaines ir juostelėje spustelėkite **bendrinimas**.</span><span class="sxs-lookup"><span data-stu-id="b6e37-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="b6e37-111">Komandos svetainei, priklausančiai "Office 365" grupei, arba ryšio svetainei:</span><span class="sxs-lookup"><span data-stu-id="b6e37-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="b6e37-112">Šie nauji svetainių tipai turi tą patį bendrinimo parametrą kaip ir jūsų organizacijos mastu, nebent visos organizacijos parametras leidžia bendrinti failus naudojant saitus, kuriems nereikia prisijungimo.</span><span class="sxs-lookup"><span data-stu-id="b6e37-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="b6e37-113">Tokiu atveju svetainėse leidžiama bendrinti su naujais ir esamais išoriniais vartotojais, kurie užsiregistruosite.</span><span class="sxs-lookup"><span data-stu-id="b6e37-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="b6e37-114">Norėdami pakeisti konkrečių svetainių parametrą, naudokite naują SharePoint administravimo centrą arba "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="b6e37-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="b6e37-115">[Sužinokite daugiau](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="b6e37-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="b6e37-116">Išorinio bendrinimo nustatymas bet kurioje svetainėje gali būti labiau ribojantis nei visos organizacijos nustatymas, bet ne daugiau, negu visos organizacijos parametras.</span><span class="sxs-lookup"><span data-stu-id="b6e37-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

