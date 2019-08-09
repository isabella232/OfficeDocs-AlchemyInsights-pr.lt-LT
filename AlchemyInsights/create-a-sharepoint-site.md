---
title: SharePoint svetainės kūrimas
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269924"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="b433c-102">SharePoint svetainės kūrimas</span><span class="sxs-lookup"><span data-stu-id="b433c-102">Create a SharePoint site</span></span>

<span data-ttu-id="b433c-103">Jūs galite pamatyti šių informacijos apie SharePoint svetainių kūrimas:</span><span class="sxs-lookup"><span data-stu-id="b433c-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="b433c-104">[Valdyti svetainės naują SharePoint administravimo centro](https://docs.microsoft.com/sharepoint/manage-site-creation): Sužinokite daugiau apie svetainės kūrimo parinktys, įskaitant tai, kaip sukurti classic svetainę arba komandos svetainę, kuri neapima "Office 365" grupė.</span><span class="sxs-lookup"><span data-stu-id="b433c-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="b433c-105">[Sukurti komandos svetainę programoje "SharePoint"](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Sužinokite, kaip sukurti komandos svetainę.</span><span class="sxs-lookup"><span data-stu-id="b433c-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="b433c-106">[Kurti internetinio bendravimo svetainę, SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Sužinokite, kaip sukurti svetainę, ryšių.</span><span class="sxs-lookup"><span data-stu-id="b433c-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="b433c-107">[Valdyti svetainės naują SharePoint administravimo centro](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Sužinokite, kaip sukurti classic svetainę arba komandos svetainę, kuri neapima "Office 365" grupė.</span><span class="sxs-lookup"><span data-stu-id="b433c-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Patarimai]
> - <span data-ttu-id="b433c-109">Negalite sukurti svetainę su tuo pačiu esamos svetainės URL.</span><span class="sxs-lookup"><span data-stu-id="b433c-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="b433c-110">Jei panaikinote svetainę ir norintys pakartotinai naudoti URL, tai galima panaikinti svetainės vis dar egzistuoja pagal **panaikinti svetaines**.</span><span class="sxs-lookup"><span data-stu-id="b433c-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="b433c-111">Valdyti panaikinti svetaines žr. [Naikinti svetainės](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="b433c-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="b433c-112">Visiškai pašalinti svetainę su "PowerShell", peržiūrėkite [Šalinti-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="b433c-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="b433c-113">Kai kuriems vartotojams gali nepavykti sukurti svetainę.</span><span class="sxs-lookup"><span data-stu-id="b433c-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="b433c-114">Peržiūrėkite [tvarkyti svetainių kūrimą SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="b433c-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="b433c-115">Galima vietoje atsiranda įstrigo ne **kūrimas** ilgiau nei tikėtasi.</span><span class="sxs-lookup"><span data-stu-id="b433c-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="b433c-116">Jei daugiau nei 24 valandų praėjo nuo pirmą kartą pamačiau šią problemą, prašome prisijungti support ticket.</span><span class="sxs-lookup"><span data-stu-id="b433c-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b433c-117">Daugeliu atvejų, mes jau dirbame išeitį.</span><span class="sxs-lookup"><span data-stu-id="b433c-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b433c-118">Nurodykite bent 24 valandas atlikti sprendimą.</span><span class="sxs-lookup"><span data-stu-id="b433c-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="b433c-119">Jei jums reikia sukurti naują komandos svetainę, kuri neapima "Office 365" grupė,</span><span class="sxs-lookup"><span data-stu-id="b433c-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


