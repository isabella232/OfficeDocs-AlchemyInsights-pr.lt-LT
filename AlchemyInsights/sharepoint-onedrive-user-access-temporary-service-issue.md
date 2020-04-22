---
title: Efektyvumo problemos – "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692701"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ff0ed-102">"SharePoint" arba "OneDrive Slow", "Unaccessible" arba nepasiekiama keliems vartotojams</span><span class="sxs-lookup"><span data-stu-id="ff0ed-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ff0ed-103">Jei "OneDrive" arba "SharePoint" svetainė nepasiekiama keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.</span><span class="sxs-lookup"><span data-stu-id="ff0ed-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ff0ed-104">[Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ff0ed-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ff0ed-105">**Vartotojo įtraukimas ir licencijavimas**</span><span class="sxs-lookup"><span data-stu-id="ff0ed-105">**Add and license the user**</span></span>

<span data-ttu-id="ff0ed-106">Įsitikinkite, kad [priskiriate licencijas vartotojams "Microsoft 365" verslui](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="ff0ed-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="ff0ed-107">**Priskirti teises**</span><span class="sxs-lookup"><span data-stu-id="ff0ed-107">**Assign Permissions**</span></span>

<span data-ttu-id="ff0ed-108">Jei vartotojui buvo priskirta "SharePoint" licencija ir vis dar gaunamas pranešimas apie prieigą, kuriai uždrausta, įsitikinkite, kad jis turi [atitinkamą teisių lygį.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="ff0ed-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ff0ed-109">**Apsvarstykite galimybę naudoti prieigos užklausos funkciją**</span><span class="sxs-lookup"><span data-stu-id="ff0ed-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ff0ed-110">[Prieigos užklausos funkcija](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) leidžia žmonėms prašyti prieigos prie turinio, kurio jie šiuo metu neturi teisės matyti.</span><span class="sxs-lookup"><span data-stu-id="ff0ed-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ff0ed-111">**Leisti pasirinktinį scenarijų gali sukelti prieigos uždrausta problemos**</span><span class="sxs-lookup"><span data-stu-id="ff0ed-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ff0ed-112">Yra tam tikrų scenarijų, kai *leisti pasirinktinio scenarijaus* funkcija gali būti pateikti prieiga uždrausta.</span><span class="sxs-lookup"><span data-stu-id="ff0ed-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ff0ed-113">Dėl funkcijų, susijusių su paveiktų funkcijų sąrašą, saugos sumetimais ir galimybę išjungti funkciją.</span><span class="sxs-lookup"><span data-stu-id="ff0ed-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ff0ed-114">Apsilankykite [Leisti arba užkirsti kelią pasirinktiniam scenarijui](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ff0ed-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

