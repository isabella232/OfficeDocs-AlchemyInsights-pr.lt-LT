---
title: Profilio sinchronizavimas
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554341"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="29414-102">Kada mano profilis keičia sinchronizavimą į "SharePoint" vartotojo profilio programą?</span><span class="sxs-lookup"><span data-stu-id="29414-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="29414-103">"SharePoint Online" naudoja "Active Directory" importavimo laikmačio užduotį (AD Import) vartotojų ir grupių importavimui į vartotojo profilio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="29414-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="29414-104">AD importuoti sinchronizuoja keitimus iš SharePoint Online katalogo parduotuvėje į vartotojo profilio programą.</span><span class="sxs-lookup"><span data-stu-id="29414-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="29414-105">Šie pakeitimai apdorojami partijomis.</span><span class="sxs-lookup"><span data-stu-id="29414-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="29414-106">Laikmačio užduotis vykdoma tol, kol keitimai bus sinchronizuojami.</span><span class="sxs-lookup"><span data-stu-id="29414-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="29414-107">Laikas, kurio reikia užduočiai vykdyti, priklauso nuo proceso keitimų skaičiaus.</span><span class="sxs-lookup"><span data-stu-id="29414-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="29414-108">Daug pakeitimų užtrunka ilgiau.</span><span class="sxs-lookup"><span data-stu-id="29414-108">A large number of changes takes longer.</span></span> <span data-ttu-id="29414-109">Aptarnavimo lygio sutartis (SLA) nurodo, kad pakeisti vartotojo SharePoint Online kataloge bus įtrauktos į vartotojo profilio programa per 24 valandas.</span><span class="sxs-lookup"><span data-stu-id="29414-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="29414-110">Daugiau informacijos apie vartotojo profilio sinchronizavimo SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="29414-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

