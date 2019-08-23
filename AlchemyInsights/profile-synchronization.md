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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554341"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="7c4ff-102">Kada mano profilio pakeitimus sinchronizuoti su SharePoint vartotojo profilio taikomosios programos?</span><span class="sxs-lookup"><span data-stu-id="7c4ff-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="7c4ff-103">SharePoint Online naudoja Active Directory importavimo laikmačio užduotis (AD importo) importuoti vartotojus ir grupes į vartotojo profilio taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="7c4ff-104">AD importo sinchronizuoja pakeitimus iš SharePoint Online katalogas parduotuvės vartotojo profilio taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="7c4ff-105">Šie pokyčiai gali būti perdirbama partijų.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="7c4ff-106">Laikmačio užduotis bus vykdoma tol, kol keitimai bus sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7c4ff-107">Užduotį, kurią norite paleisti laiko priklauso keičiant proceso skaičiaus.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="7c4ff-108">Didelio skaičiaus pokyčiai užtrunka ilgiau.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-108">A large number of changes takes longer.</span></span> <span data-ttu-id="7c4ff-109">Service Level AGREMENT (SLA) nurodo, kad SharePoint Online kataloge vartotojo pakeitimas atsispindės vartotojo profilio taikomosios programos per 24 valandas.</span><span class="sxs-lookup"><span data-stu-id="7c4ff-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="7c4ff-110">Daugiau informacijos apie vartotojo profilio sinchronizavimo SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7c4ff-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

