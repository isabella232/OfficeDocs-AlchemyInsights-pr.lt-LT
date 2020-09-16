---
title: Efektyvumo problemos – "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771252"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5d154-102">"SharePoint" arba "OneDrive" lėtas, nepasiekiamas arba neprieinamas keliems vartotojams</span><span class="sxs-lookup"><span data-stu-id="5d154-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="5d154-103">Jei "OneDrive" arba "SharePoint" svetainė neprieinama keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.</span><span class="sxs-lookup"><span data-stu-id="5d154-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="5d154-104">[Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5d154-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="5d154-105">**Vartotojo įtraukimas ir licencijuoti**</span><span class="sxs-lookup"><span data-stu-id="5d154-105">**Add and license the user**</span></span>

<span data-ttu-id="5d154-106">Įsitikinkite, kad [vartotojams priskiriate licencijas "Microsoft 365" verslui](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="5d154-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="5d154-107">**Teisių priskyrimas**</span><span class="sxs-lookup"><span data-stu-id="5d154-107">**Assign Permissions**</span></span>

<span data-ttu-id="5d154-108">Jei vartotojui priskirta "SharePoint" licencija ir vis tiek gaunamas pranešimas "prieiga uždrausta", įsitikinkite, kad jiems priskirtas [reikiamas teisių lygis](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="5d154-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="5d154-109">**Naudokite "Access" užklausos funkciją**</span><span class="sxs-lookup"><span data-stu-id="5d154-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="5d154-110">" [Access" užklausos funkcija](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) leidžia žmonėms prašyti prieigos prie turinio, kurio jie šiuo metu neturi teisės matyti.</span><span class="sxs-lookup"><span data-stu-id="5d154-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="5d154-111">**Leisti pasirinktiniam scenarijui gali sukelti "Access" uždraustas problemas**</span><span class="sxs-lookup"><span data-stu-id="5d154-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="5d154-112">Yra tam tikrų scenarijų, kai *leisti pasirinktinę scenarijaus* funkciją gali pateikti "Access" nesuteikta.</span><span class="sxs-lookup"><span data-stu-id="5d154-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="5d154-113">Dėl paveiktų funkcijų sąrašo, saugos sumetimais ir galimybės išjungti funkciją.</span><span class="sxs-lookup"><span data-stu-id="5d154-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="5d154-114">Apsilankykite [leisti arba neleiskite pasirinktiniam scenarijui](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="5d154-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

