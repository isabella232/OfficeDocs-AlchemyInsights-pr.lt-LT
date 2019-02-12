---
title: Pranešimus Prieiga uždrausta trikčių diagnostika
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916460"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="be040-102">Pranešimus Prieiga uždrausta trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="be040-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="be040-p101">Jei kas nors turite pranešimą "Prieiga uždrausta" į bendrai naudojamą aplanką, svetainių rinkinio administratorius gali įgalinti "riboto naudojimo vartotojas leidimo lockdown režimas." Išjungti šį parametrą:</span><span class="sxs-lookup"><span data-stu-id="be040-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="be040-105">Eikite į svetainę, spustelėkite nustatymų piktogramą ir tada spustelėkite **Svetainės parametrai**.</span><span class="sxs-lookup"><span data-stu-id="be040-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="be040-106">Dalyje **Svetainių rinkinio administravimas**spustelėkite **svetainės rinkinio funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="be040-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="be040-107">Šalia **riboto naudojimo vartotojas leidimo lockdown režimas**, spustelėkite **išjungti aktyvinimą**.</span><span class="sxs-lookup"><span data-stu-id="be040-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="be040-p102">Pranešimą prieiga uždrausta gali atsirasti bendrai naudojamiems aplankams, jei svetainė publikavimo svetainės. Informacijos rasite [Prieiga uždrausta bandant pasiekti bendrinamą aplanką](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="be040-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="be040-p103">Jei yra kas nors turite pranešimą "Prieiga uždrausta" bandant Rodyti prieigos prašymus, vartotojas turi būti įtraukta kaip svetainių rinkinio administratorius arba svetainės savininkų grupės narys. Daugiau informacijos rasite [Nesuteikta prieiga prie prieigos prašymus sąrašą](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="be040-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="be040-112">Jei vartotojas gavo pranešimą "Prieiga uždrausta" po to, kai jie buvo pašalintas iš Active Directory vietinės ir sudedama atgal, peržiūrėkite [Prieiga uždrausta kai vartotojo abonementą yra sinchronizuojami su "Office 365"](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="be040-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

