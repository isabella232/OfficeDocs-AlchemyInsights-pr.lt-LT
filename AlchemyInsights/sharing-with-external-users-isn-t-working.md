---
title: Dalintis su išoriniais vartotojais neveikia
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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753434"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="3276f-102">Spręsti problemas, dalytis SharePoint turinio su išoriniais vartotojais</span><span class="sxs-lookup"><span data-stu-id="3276f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="3276f-103">Įsitikinkite, kad išorinis bendrinimas yra įjungtas, jūsų organizacija:</span><span class="sxs-lookup"><span data-stu-id="3276f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="3276f-104">Eikite į į [paslaugos &amp; priedai "Microsoft 365" administravimo centro puslapį](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="3276f-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="3276f-105">Įsitikinkite, kad parametras yra įjungta "Įjungtas."</span><span class="sxs-lookup"><span data-stu-id="3276f-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="3276f-106">Jei pažymėtas "Tik esamos išoriniams vartotojams", įsitikinkite, kad išorinis vartotojas yra įtraukta į "Microsoft" 365 administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="3276f-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="3276f-107">Įsitikinkite, kad svetainės įjungta išorės dalintis ja.</span><span class="sxs-lookup"><span data-stu-id="3276f-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="3276f-108">Klasikiniai svetainės rinkinio:</span><span class="sxs-lookup"><span data-stu-id="3276f-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="3276f-109">Klasikinis SharePoint administravimo centro kairiojoje srityje, spustelėkite **svetainių rinkinius**.</span><span class="sxs-lookup"><span data-stu-id="3276f-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="3276f-110">Pasirinkite svetainę ar svetaines, ir juostelėje, spustelėkite **bendrinimas**.</span><span class="sxs-lookup"><span data-stu-id="3276f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="3276f-111">Komandos svetainę, kuri priklauso "Office 365" grupei, arba bendravimo svetainės:</span><span class="sxs-lookup"><span data-stu-id="3276f-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="3276f-112">Šioms naujoms svetainės turi pačios bendrinimo nustatymas, kaip jūsų visos organizacijos aplinkoje, jei visos organizacijos parametras leidžia bendrinti failus naudodami nuorodas, kurios nereikalauja prisijungimo.</span><span class="sxs-lookup"><span data-stu-id="3276f-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="3276f-113">Tokiu atveju svetainėse leidžia dalintis su naujų ir esamų išoriniams vartotojams, kurie prisijungti.</span><span class="sxs-lookup"><span data-stu-id="3276f-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="3276f-114">Norėdami pakeisti parametrą konkrečių svetainių, naudokite naują SharePoint administravimo centro (beta versijos) arba "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="3276f-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="3276f-115">[Sužinokite daugiau](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="3276f-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="3276f-116">Išorinio bendrinimo parametrą dėl bet kurios svetainės gali būti griežtesnės negu visos organizacijos aplinkoje, bet ne griežtomis nei visos organizacijos parametrus.</span><span class="sxs-lookup"><span data-stu-id="3276f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

