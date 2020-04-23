---
title: Profilio sinchronizavimas
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768121"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="43b8b-102">Kada mano profilis pasikeičia į "SharePoint" vartotojo profilio taikomąją programą?</span><span class="sxs-lookup"><span data-stu-id="43b8b-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="43b8b-103">"SharePoint Online" naudoja Active Directory importavimo laikmačio užduotį (AD importavimas) vartotojams ir grupėms į vartotojo profilio taikomąją programą importuoti.</span><span class="sxs-lookup"><span data-stu-id="43b8b-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="43b8b-104">AD importavimas sinchronizuoja pakeitimus iš SharePoint Online Directory store vartotojo profilio programa.</span><span class="sxs-lookup"><span data-stu-id="43b8b-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="43b8b-105">Šie pakeitimai apdorojami paketuose.</span><span class="sxs-lookup"><span data-stu-id="43b8b-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="43b8b-106">Laikmačio užduotis vykdoma tol, kol pakeitimai bus sinchronizuojami.</span><span class="sxs-lookup"><span data-stu-id="43b8b-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="43b8b-107">Užduoties vykdymo laikas priklauso nuo apdorojamų pakeitimų skaičiaus.</span><span class="sxs-lookup"><span data-stu-id="43b8b-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="43b8b-108">Daug pakeitimų trunka ilgiau.</span><span class="sxs-lookup"><span data-stu-id="43b8b-108">A large number of changes takes longer.</span></span> <span data-ttu-id="43b8b-109">Paslaugų lygio sutartyje (SLA) teigiama, kad "SharePoint Online Directory" vartotojo pakeitimas bus atspindėtas vartotojo profilio taikomojoje programoje per 24 valandas.</span><span class="sxs-lookup"><span data-stu-id="43b8b-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="43b8b-110">Daugiau informacijos apie vartotojo profilio sinchronizavimą "SharePoint Online"</span><span class="sxs-lookup"><span data-stu-id="43b8b-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

