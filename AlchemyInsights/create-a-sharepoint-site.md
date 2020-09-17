---
title: "\"SharePoint\" svetainės kūrimas"
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806947"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="51738-102">"SharePoint" svetainės kūrimas</span><span class="sxs-lookup"><span data-stu-id="51738-102">Create a SharePoint site</span></span>

<span data-ttu-id="51738-103">Kurkite arba valdykite svetaines iš [aktyvių svetainių](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) "SharePoint" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="51738-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="51738-104">Daugiau informacijos rasite [svetainės valdymas naujame "SharePoint" administravimo centre](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="51738-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="51738-105">Patarimai</span><span class="sxs-lookup"><span data-stu-id="51738-105">Tips:</span></span>

- <span data-ttu-id="51738-106">**Negalite** sukurti svetainės su tuo pačiu esamos svetainės URL.</span><span class="sxs-lookup"><span data-stu-id="51738-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="51738-107">Jei panaikinote svetainę ir norite iš naujo naudoti URL, panaikinama svetainė vis dar yra dalyje [panaikintos svetainės](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="51738-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="51738-108">Svetainė turi būti panaikinta visam laikui, kad iš naujo naudotų URL.</span><span class="sxs-lookup"><span data-stu-id="51738-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="51738-109">Norėdami visiškai pašalinti svetainę naudodami "PowerShell", peržiūrėkite cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="51738-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="51738-110">Kai kuriems vartotojams gali nepavykti sukurti svetainės.</span><span class="sxs-lookup"><span data-stu-id="51738-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="51738-111">[Peržiūrėkite "SharePoint Online" svetainės kūrimo valdymas](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="51738-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="51738-112">Gali būti, kad svetainė bus **rodoma ilgiau nei** tikėtasi.</span><span class="sxs-lookup"><span data-stu-id="51738-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="51738-113">Jei praėjo daugiau nei 24 valandos po to, kai pirmą kartą matėte šią problemą, prisijunkite prie palaikymo bilieto.</span><span class="sxs-lookup"><span data-stu-id="51738-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="51738-114">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="51738-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="51738-115">Pateikite mums bent 24 valandas, kad užbaigtumėte sprendimą.</span><span class="sxs-lookup"><span data-stu-id="51738-115">Please give us at least 24 hours to complete a solution.</span></span>
