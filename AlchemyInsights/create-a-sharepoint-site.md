---
title: "\"SharePoint\" svetainės kūrimas"
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770863"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="bc75f-102">"SharePoint" svetainės kūrimas</span><span class="sxs-lookup"><span data-stu-id="bc75f-102">Create a SharePoint site</span></span>

<span data-ttu-id="bc75f-103">Kurkite arba tvarkykite svetaines iš [aktyvių svetainių](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) "SharePoint" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="bc75f-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="bc75f-104">Daugiau informacijos ieškokite [svetainių valdymas naujajame "SharePoint" administravimo centre](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bc75f-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="bc75f-105">Patarimai:</span><span class="sxs-lookup"><span data-stu-id="bc75f-105">Tips:</span></span>

- <span data-ttu-id="bc75f-106">**Negalima** sukurti svetainės su tuo pačiu esamos svetainės URL.</span><span class="sxs-lookup"><span data-stu-id="bc75f-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="bc75f-107">Jei panaikinote svetainę ir norite iš naujo naudoti URL, gali būti, kad ištrinta svetainė vis dar egzistuoja [naikinvietėse](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="bc75f-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="bc75f-108">Svetainė turės būti visam laikui ištrinta, kad pakartotinai naudotų URL.</span><span class="sxs-lookup"><span data-stu-id="bc75f-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="bc75f-109">Norėdami visiškai pašalinti svetainę su "PowerShell", peržiūrėkite [pašalinti-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="bc75f-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="bc75f-110">Kai kuriems vartotojams gali nepavykti sukurti svetainės.</span><span class="sxs-lookup"><span data-stu-id="bc75f-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="bc75f-111">[Ieškokite svetainės kūrimo valdymas "SharePoint Online"](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bc75f-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="bc75f-112">Gali būti, kad svetainė užstrigo **kurdami** ilgiau nei tikėtasi.</span><span class="sxs-lookup"><span data-stu-id="bc75f-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="bc75f-113">Jei praėjo daugiau nei 24 valandos nuo tada, kai pirmą kartą pamatėte šią problemą, prašome prisijungti prie palaikymo bilieto.</span><span class="sxs-lookup"><span data-stu-id="bc75f-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bc75f-114">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="bc75f-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bc75f-115">Prašome pateikti mums bent 24 valandas, kad užbaigtumėte sprendimą.</span><span class="sxs-lookup"><span data-stu-id="bc75f-115">Please give us at least 24 hours to complete a solution.</span></span>
