---
title: Trikčių diagnostika prieiga uždrausta pranešimai
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751284"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="6cc4b-102">"SharePoint"/"OneDrive" administravimo centro pranešimų prieiga uždrausta trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="6cc4b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="6cc4b-103">Jei gaunate pranešimą prieiga uždrausta bandant naršyti SharePoint/OneDrive administravimo centras, įsitikinkite, kad jums [Priskirti licenciją vartotojui](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="6cc4b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="6cc4b-104">Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jiems [priskirtas administratoriaus vaidmuo](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , kuris gali pasiekti administravimo centrus.</span><span class="sxs-lookup"><span data-stu-id="6cc4b-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="6cc4b-105">Ši problema taip pat gali kilti, kai vartotojas panaikinamas ir iš naujo sukurtas naudojant tą patį vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="6cc4b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="6cc4b-106">Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="6cc4b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="6cc4b-107">Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="6cc4b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="6cc4b-108">Antrasis scenarijus apima katalogų sinchronizavimas su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="6cc4b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="6cc4b-109">Jei vartotojai jau prisijungė prie "SharePoint", ir tada perkeliami į kitą OU ir resynced su "SharePoint", jie gali kilti ši problema.</span><span class="sxs-lookup"><span data-stu-id="6cc4b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="6cc4b-110">Norėdami išspręsti šią problemą, turite atkurti pradinį UPN su straipsnyje nurodytus veiksmus, [atkurti vartotojo Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6cc4b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="6cc4b-111">Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras yra neprieinama keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikinas tarnybos problema.</span><span class="sxs-lookup"><span data-stu-id="6cc4b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="6cc4b-112">[Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6cc4b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


