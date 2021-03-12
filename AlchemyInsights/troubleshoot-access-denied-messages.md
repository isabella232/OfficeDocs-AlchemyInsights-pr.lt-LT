---
title: "\"Access\" uždraustų žinučių trikčių diagnostika"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704902"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="055e8-102">"Access" uždraustų žinučių trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="055e8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="055e8-103">Jei kas nors gavo pranešimą "prieiga uždrausta" "SharePoint" bendrinamame aplanke, svetainių rinkinio administratorius galėjo įgalinti "Riboto priėjimo vartotojo teisių blokavimo režimą".</span><span class="sxs-lookup"><span data-stu-id="055e8-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="055e8-104">Norėdami išjungti:</span><span class="sxs-lookup"><span data-stu-id="055e8-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="055e8-105">Eikite į svetainę, spustelėkite piktogramą parametrai, tada spustelėkite **Svetainės parametrai**.</span><span class="sxs-lookup"><span data-stu-id="055e8-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="055e8-106">Dalyje **svetainių rinkinio administravimas** spustelėkite **svetainių rinkinio funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="055e8-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="055e8-107">Šalia **riboto priėjimo vartotojų teisių blokavimo režimo** spustelėkite **išjungti**.</span><span class="sxs-lookup"><span data-stu-id="055e8-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="055e8-108">"Access Denied" pranešimas taip pat gali įvykti bendrinamuose aplankuose, jei svetainė yra publikavimo svetainė.</span><span class="sxs-lookup"><span data-stu-id="055e8-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="055e8-109">Informacijos ieškokite skyriuje [prieiga uždrausta jungiantis prie bendrinamo aplanko](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="055e8-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="055e8-110">Jei kas nors gavo pranešimą "prieiga uždrausta" bandydami Peržiūrėti prieigos užklausas, vartotojas turi būti įtrauktas kaip svetainių rinkinio administratorius arba svetainės savininkų grupės narys.</span><span class="sxs-lookup"><span data-stu-id="055e8-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="055e8-111">Daugiau informacijos ieškokite " [Access" uždrausta prieigos užklausų sąrašui](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="055e8-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="055e8-112">Jei vartotojas gavo pranešimą "prieiga uždrausta" po to, kai jis buvo pašalintas iš "Active Directory" vietoje ir vėl įtrauktas, peržiūrėkite " [Access" uždraustas, kai vartotojo paskyra sinchronizuojama su "Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)".</span><span class="sxs-lookup"><span data-stu-id="055e8-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

