---
title: "\"SharePoint\" svetainės kūrimas"
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049885"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="8023b-102">"SharePoint" svetainės kūrimas</span><span class="sxs-lookup"><span data-stu-id="8023b-102">Create a SharePoint site</span></span>

<span data-ttu-id="8023b-103">Informaciją apie "SharePoint" svetainių kūrimą galite peržiūrėti toliau:</span><span class="sxs-lookup"><span data-stu-id="8023b-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="8023b-104">[Svetainių tvarkymas naujajame "SharePoint" administravimo centre](https://docs.microsoft.com/sharepoint/manage-site-creation): Sužinokite apie svetainių kūrimo parinktis, įskaitant tai, kaip sukurti klasikinę svetainę arba komandų svetainę, kurioje nėra "Office 365" grupės.</span><span class="sxs-lookup"><span data-stu-id="8023b-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="8023b-105">[Sukurti komandos svetainę "SharePoint"](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Sužinokite, kaip sukurti komandos svetainę.</span><span class="sxs-lookup"><span data-stu-id="8023b-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="8023b-106">[Sukurti ryšio svetainėje SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Sužinokite, kaip sukurti ryšių svetainę.</span><span class="sxs-lookup"><span data-stu-id="8023b-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="8023b-107">[Svetainių tvarkymas naujajame "SharePoint" administravimo centre](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Sužinokite, kaip sukurti klasikinę svetainę arba komandos svetainę, kurioje nėra "Office 365" grupės.</span><span class="sxs-lookup"><span data-stu-id="8023b-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="8023b-108">**Patarimai:**</span><span class="sxs-lookup"><span data-stu-id="8023b-108">**Tips:**</span></span>
- <span data-ttu-id="8023b-109">Negalima sukurti svetainės su tuo pačiu esamos svetainės URL.</span><span class="sxs-lookup"><span data-stu-id="8023b-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="8023b-110">Jei panaikinote svetainę ir norite iš naujo naudoti URL, gali būti, kad ištrinta svetainė vis dar egzistuoja **naikinvietėse**.</span><span class="sxs-lookup"><span data-stu-id="8023b-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="8023b-111">Norėdami valdyti ištrintas svetaines, [panaikinkite svetainę](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="8023b-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="8023b-112">Norėdami visiškai pašalinti svetainę su "PowerShell", peržiūrėkite [pašalinti-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="8023b-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="8023b-113">Kai kuriems vartotojams gali nepavykti sukurti svetainės.</span><span class="sxs-lookup"><span data-stu-id="8023b-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="8023b-114">Žr [valdyti svetainių kūrimas SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="8023b-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="8023b-115">Gali būti, kad svetainė užstrigo **kurdami** ilgiau nei tikėtasi.</span><span class="sxs-lookup"><span data-stu-id="8023b-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="8023b-116">Jei praėjo daugiau nei 24 valandos nuo tada, kai pirmą kartą pamatėte šią problemą, prašome prisijungti prie palaikymo bilieto.</span><span class="sxs-lookup"><span data-stu-id="8023b-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8023b-117">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="8023b-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8023b-118">Prašome pateikti mums bent 24 valandas, kad užbaigtumėte sprendimą.</span><span class="sxs-lookup"><span data-stu-id="8023b-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="8023b-119">Jei reikia sukurti naują komandos svetainę, kuri neapima "Office 365" grupės,</span><span class="sxs-lookup"><span data-stu-id="8023b-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


