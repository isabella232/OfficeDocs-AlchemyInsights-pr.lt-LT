---
title: Prieigos uždraustų pranešimų trikčių diagnostika
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759808"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d775a-102">Prieigos uždraustų pranešimų trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="d775a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d775a-103">Jei kas nors gavo pranešimą "Prieiga uždrausta" į bendrai naudojamą aplanką "SharePoint", svetainių rinkinio administratorius galėjo įgalinti "Ribotos prieigos vartotojo teisių blokavimo režimą".</span><span class="sxs-lookup"><span data-stu-id="d775a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d775a-104">Norėdami tai išjungti:</span><span class="sxs-lookup"><span data-stu-id="d775a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d775a-105">Raskite svetainę, spustelėkite piktogramą Parametrai, tada spustelėkite **Svetainės parametrai**.</span><span class="sxs-lookup"><span data-stu-id="d775a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d775a-106">Dalyje **Svetainių rinkinio administravimas**spustelėkite **Svetainių rinkinio priemonės**.</span><span class="sxs-lookup"><span data-stu-id="d775a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d775a-107">Šalia **Apribotos prieigos vartotojo teisių užrakinimo režimas**spustelėkite **Išjungti**.</span><span class="sxs-lookup"><span data-stu-id="d775a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d775a-108">Prieiga uždrausta pranešimas taip pat gali atsirasti bendrai naudojamų aplankų, jei svetainė yra publikavimo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="d775a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d775a-109">Informacijos ieškokite [Prieiga uždrausta, kai prisijungiate prie bendrai naudojamo aplanko](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="d775a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="d775a-110">Jei bandant peržiūrėti prieigos užklausas kažkas gavo pranešimą "Prieiga uždrausta", vartotojas turi būti įtrauktas kaip svetainės svetainių rinkinio administratorius arba savininkų grupės narys.</span><span class="sxs-lookup"><span data-stu-id="d775a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d775a-111">Daugiau informacijos [ieškokite Prieiga uždrausta prie prieigos užklausų sąrašo](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="d775a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d775a-112">Jei vartotojas gavo pranešimą "Prieiga uždrausta", kai jie buvo pašalinti iš "Active Directory" vietiniame ir tada įtraukti atgal, žr [Prieiga uždrausta, kai vartotojo abonementas sinchronizuojamas su "Microsoft 365".](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="d775a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

