---
title: Trikčių diagnostikos prieiga uždrausta pranešimus į "OneDrive" verslui svetainės
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051613"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="8fe50-102">Trikčių diagnostikos prieiga uždrausta pranešimus į "OneDrive" verslui svetainės</span><span class="sxs-lookup"><span data-stu-id="8fe50-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="8fe50-103">Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukurtas naudojant tą patį vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="8fe50-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8fe50-104">Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="8fe50-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8fe50-105">Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="8fe50-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8fe50-106">Antrasis scenarijus apima katalogų sinchronizavimas su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="8fe50-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8fe50-107">Jei vartotojai jau prisijungė prie "SharePoint", ir tada perkeliami į kitą OU ir resynced su "SharePoint", jie gali kilti ši problema.</span><span class="sxs-lookup"><span data-stu-id="8fe50-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="8fe50-108">Norėdami išspręsti šią problemą, reikia atkurti pradinį UPN su straipsnyje nurodytus veiksmus, [atkurti vartotojo Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8fe50-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="8fe50-109">Jei negalite atkurti originalaus vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" svetainės atlikdami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo]().</span><span class="sxs-lookup"><span data-stu-id="8fe50-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="8fe50-110">Kai tai padarysite, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę atlikdami veiksmus, Norėdami [pridėti administratoriaus vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="8fe50-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="8fe50-111">Daugiau informacijos apie teisių lygius rasite straipsnyje " [SharePoint" teisių lygių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="8fe50-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
