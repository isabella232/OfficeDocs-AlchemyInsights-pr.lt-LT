---
title: Dalintis su išoriniais vartotojais neveikia
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480456"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="a2938-102">Spręsti problemas, dalytis SharePoint turinio su išoriniais vartotojais</span><span class="sxs-lookup"><span data-stu-id="a2938-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="a2938-103">Įsitikinkite, kad išorinis bendrinimas yra įjungtas, jūsų organizacija:</span><span class="sxs-lookup"><span data-stu-id="a2938-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="a2938-104">Eikite į į [paslaugos &amp; priedai "Office 365" administravimo centro puslapį](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), spustelėkite **svetainės**.</span><span class="sxs-lookup"><span data-stu-id="a2938-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="a2938-p101">Įsitikinkite, kad parametras yra įjungta "Įjungtas." Jei pažymėtas "Tik esamos išoriniams vartotojams", įsitikinkite, kad išorinis vartotojas yra įtraukta į "Office 365" administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="a2938-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="a2938-p102">Įsitikinkite, kad svetainės įjungta išorės dalintis ja. Klasikiniai svetainės rinkinio:</span><span class="sxs-lookup"><span data-stu-id="a2938-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="a2938-109">Klasikinis SharePoint administravimo centro kairiojoje srityje, spustelėkite **svetainių rinkinius**.</span><span class="sxs-lookup"><span data-stu-id="a2938-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="a2938-110">Pasirinkite svetainę ar svetaines, ir juostelėje, spustelėkite **bendrinimas**.</span><span class="sxs-lookup"><span data-stu-id="a2938-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="a2938-111">Komandos svetainę, kuri priklauso "Office 365" grupei, arba bendravimo svetainės:</span><span class="sxs-lookup"><span data-stu-id="a2938-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="a2938-p103">Šioms naujoms svetainės turi pačios bendrinimo nustatymas, kaip jūsų visos organizacijos aplinkoje, jei visos organizacijos parametras leidžia bendrinti failus naudodami nuorodas, kurios nereikalauja prisijungimo. Tokiu atveju svetainėse leidžia dalintis su naujų ir esamų išoriniams vartotojams, kurie prisijungti. Norėdami pakeisti parametrą konkrečių svetainių, naudokite naują SharePoint administravimo centro (beta versijos) arba "PowerShell". [Sužinokite daugiau](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="a2938-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a2938-116">Išorinio bendrinimo parametrą dėl bet kurios svetainės gali būti griežtesnės negu visos organizacijos aplinkoje, bet ne griežtomis nei visos organizacijos parametrus.</span><span class="sxs-lookup"><span data-stu-id="a2938-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

