---
title: Profilio sinchronizavimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801777"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="80e43-102">Kada mano profilis pakeis sinchronizavimą su "SharePoint" vartotojo profilio taikomąja programa?</span><span class="sxs-lookup"><span data-stu-id="80e43-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="80e43-103">"SharePoint Online" naudoja "Active Directory" importavimo laikmačio užduotį (skelbimų importavimą), kad importuotumėte vartotojus ir grupes į vartotojo profilio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="80e43-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="80e43-104">SKELBIMŲ importavimas sinchronizuoja duomenis iš "SharePoint Online" katalogų parduotuvės į vartotojo profilio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="80e43-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="80e43-105">Šie pokyčiai apdorojami paketais.</span><span class="sxs-lookup"><span data-stu-id="80e43-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="80e43-106">Laikmačio užduotis vykdoma tol, kol bus sinchronizuoti pasikeitimai.</span><span class="sxs-lookup"><span data-stu-id="80e43-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="80e43-107">Darbo vykdymo laikas priklauso nuo proceso keitimo skaičiaus.</span><span class="sxs-lookup"><span data-stu-id="80e43-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="80e43-108">Daug pasikeitimų trunka ilgiau.</span><span class="sxs-lookup"><span data-stu-id="80e43-108">A large number of changes takes longer.</span></span> <span data-ttu-id="80e43-109">Paslaugų lygio sutartyje (SLA) nurodoma, kad "SharePoint Online" kataloge vartotojas pakeis vartotoją per 24 valandas.</span><span class="sxs-lookup"><span data-stu-id="80e43-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="80e43-110">Daugiau informacijos apie vartotojo profilio sinchronizavimą "SharePoint Online"</span><span class="sxs-lookup"><span data-stu-id="80e43-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

