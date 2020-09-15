---
title: Neveikia bendras naudojimas su išoriniais vartotojais
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691583"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="42f53-102">"SharePoint" turinio naudojimo su išoriniais vartotojais problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="42f53-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="42f53-103">Įsitikinkite, kad jūsų organizacijai įjungtas Išorinis bendrinimas:</span><span class="sxs-lookup"><span data-stu-id="42f53-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="42f53-104">Eikite į [ &amp; "Microsoft 365" administravimo centro puslapį tarnybų papildiniai](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), tada spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="42f53-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="42f53-105">Įsitikinkite, kad parametras įjungtas į "įjungta".</span><span class="sxs-lookup"><span data-stu-id="42f53-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="42f53-106">Jei pasirinkta "tik esami Išoriniai vartotojai", įsitikinkite, kad išorinis vartotojas yra nurodytas "Microsoft" 365 administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="42f53-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="42f53-107">Įsitikinkite, kad svetainėje įjungtas išorinis bendras naudojimasis.</span><span class="sxs-lookup"><span data-stu-id="42f53-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="42f53-108">Klasikinis svetainių rinkinys:</span><span class="sxs-lookup"><span data-stu-id="42f53-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="42f53-109">Naujame "SharePoint" administravimo centre, kairiojoje srityje spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="42f53-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="42f53-110">Pažymėkite svetainę arba svetaines ir juostelėje spustelėkite **bendras naudojimasis**.</span><span class="sxs-lookup"><span data-stu-id="42f53-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="42f53-111">Komandos svetainėje, priklausančiai "Microsoft 365" grupei, arba bendravimo svetainei:</span><span class="sxs-lookup"><span data-stu-id="42f53-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="42f53-112">Šie nauji svetainių tipai turi tokį patį bendro naudojimo parametrą kaip ir visos organizacijos parametrai, nebent visos organizacijos parametras leidžia failų bendrinimas naudojant saitus, kuriems nereikia prisijungimo.</span><span class="sxs-lookup"><span data-stu-id="42f53-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="42f53-113">Šiuo atveju svetainės leidžia dalytis su naujais ir esamais išoriniais vartotojais, kurie užsiregistruosite.</span><span class="sxs-lookup"><span data-stu-id="42f53-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="42f53-114">Norėdami pakeisti konkrečių svetainių parametrą, naudokite naują "SharePoint" administravimo centrą arba "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="42f53-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="42f53-115">[Sužinokite daugiau](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="42f53-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="42f53-116">Išorinio bendro naudojimo parametrai bet kurioje svetainėje gali būti labiau ribojami nei visos organizacijos parametrai, bet ne daugiau nei visos organizacijos parametrai.</span><span class="sxs-lookup"><span data-stu-id="42f53-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

