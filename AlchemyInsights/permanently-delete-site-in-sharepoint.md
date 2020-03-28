---
title: Panaikinti svetainę visam laikui programoje „SharePoint“
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955163"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="af02f-102">Panaikinti svetainę visam laikui programoje „SharePoint“</span><span class="sxs-lookup"><span data-stu-id="af02f-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="af02f-103">Jei norite pakartotinai naudoti URL iš panaikintos svetainės (norėdami iš naujo sukurti svetainę) arba visam laikui panaikinti svetainę, nes ji daugiau nebėra naudojama, galite naujajame „SharePoint“ administravimo centre naudoti funkciją **Panaikinti visam laikui**.</span><span class="sxs-lookup"><span data-stu-id="af02f-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="af02f-104">Eikite į [Naujajame „SharePoint“ administravimo centre panaikinti svetainės puslapiai](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) ir prisijunkite naudodami paskyrą, kuriai suteiktos jūsų organizacijos administratoriaus teisės.</span><span class="sxs-lookup"><span data-stu-id="af02f-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="af02f-105">Kairiajame stulpelyje pasirinkite svetainę.</span><span class="sxs-lookup"><span data-stu-id="af02f-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="af02f-106">Spustelėkite **Panaikinti visam laikui**.</span><span class="sxs-lookup"><span data-stu-id="af02f-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="af02f-107">**Pastaba**: naudojant naująjį „SharePoint“ administravimo centrą negalima visam laikui panaikinti grupės prijungtų svetainių.</span><span class="sxs-lookup"><span data-stu-id="af02f-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="af02f-108">Vietoj to turite naudoti [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="af02f-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="af02f-109">Jei norite gauti daugiau informacijos, žr. [Panaikinti svetainę visam laikui](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="af02f-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
