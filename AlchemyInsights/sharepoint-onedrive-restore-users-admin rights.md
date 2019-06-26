---
title: Prieiga uždrausta pranešimų į "OneDrive" verslo svetainėms
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223432"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="df37d-102">Prieiga uždrausta pranešimų į "OneDrive" verslo svetainėms</span><span class="sxs-lookup"><span data-stu-id="df37d-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="df37d-103">Ši problema dažniausiai kyla, kai vartotojas yra panaikinti ir iš naujo sukurti patį vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="df37d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="df37d-104">Sukūrus abonementą sukuriamas naudojant skirtingus PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="df37d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="df37d-105">Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="df37d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="df37d-106">Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="df37d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="df37d-107">Jei vartotojai turi jau prisijungę prie SharePoint, tada persikėlė į skirtingas OU ir resynced su "SharePoint", jie gali kilti ši problema.</span><span class="sxs-lookup"><span data-stu-id="df37d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="df37d-108">Norėdami išspręsti šią problemą turite atkurti originalų UPN su straipsnyje,[atkurti vartotojo "Office 365"](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="df37d-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="df37d-109">Po to, kai tai bus padaryta, galite patikrinti turi administratoriaus teises į "OneDrive" svetainę atlikdami nurodytus veiksmus norėdami [pridėti admin's vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="df37d-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="df37d-110">Daugiau informacijos apie teisių lygius, ieškokite straipsnyje, [suprasti teisių lygius programoje "SharePoint"](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="df37d-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
