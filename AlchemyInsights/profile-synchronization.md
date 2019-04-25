---
title: Profilio sinchronizavimo
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371992"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="55d3a-102">Kada mano profilio pakeitimus sinchronizuoti su SharePoint vartotojo profilio taikomosios programos?</span><span class="sxs-lookup"><span data-stu-id="55d3a-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="55d3a-103">SharePoint Online naudoja Active Directory importavimo laikmačio užduotis (AD importo) importuoti vartotojus ir grupes į vartotojo profilio taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="55d3a-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="55d3a-104">AD importo sinchronizuoja pakeitimus iš SharePoint Online katalogas parduotuvės vartotojo profilio taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="55d3a-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="55d3a-105">Šie pokyčiai gali būti perdirbama partijų.</span><span class="sxs-lookup"><span data-stu-id="55d3a-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="55d3a-106">Laikmačio užduotis bus vykdoma tol, kol keitimai bus sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="55d3a-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="55d3a-107">Užduotį, kurią norite paleisti laiko priklauso keičiant proceso skaičiaus.</span><span class="sxs-lookup"><span data-stu-id="55d3a-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="55d3a-108">Didelio skaičiaus pokyčiai užtrunka ilgiau.</span><span class="sxs-lookup"><span data-stu-id="55d3a-108">A large number of changes takes longer.</span></span> <span data-ttu-id="55d3a-109">Service Level AGREMENT (SLA) nurodo, kad SharePoint Online kataloge vartotojo pakeitimas atsispindės vartotojo profilio taikomosios programos per 24 valandas.</span><span class="sxs-lookup"><span data-stu-id="55d3a-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="55d3a-110">Daugiau informacijos apie vartotojo profilio sinchronizavimo SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="55d3a-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

