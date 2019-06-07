---
title: Pranešimus Prieiga uždrausta trikčių diagnostika
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760348"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="aaba9-102">Sharepoint/OneDrive administravimo centro pranešimus Prieiga uždrausta trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="aaba9-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="aaba9-103">Jei gaunate kad prieiga uždrausta bandant naršyti į Sharepoint/OneDrive administravimo centrą pranešimą, prašome įsitikinti, kad turite [Priskirti licenciją vartotojui](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="aaba9-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="aaba9-104">Jei vartotojas turi licenciją, taip pat būtinai yra [priskirtas administratoriaus vaidmenį](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , galite pasiekti admin centrai.</span><span class="sxs-lookup"><span data-stu-id="aaba9-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="aaba9-105">Ši problema gali atsirasti, kai vartotojo panaikinti ir iš naujo sukurti patį vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="aaba9-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="aaba9-106">Sukūrus abonementą sukuriamas naudojant skirtingus PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="aaba9-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="aaba9-107">Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="aaba9-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="aaba9-108">Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="aaba9-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="aaba9-109">Jei vartotojai turi jau prisijungę prie SharePoint, tada persikėlė į skirtingas OU ir resynced su "SharePoint", jie gali kilti ši problema.</span><span class="sxs-lookup"><span data-stu-id="aaba9-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="aaba9-110">Norėdami išspręsti šią problemą, turite atkurti originalų UPN su straipsnyje, [atkurti vartotojo "Office 365"](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="aaba9-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="aaba9-111">Pastaba: Jei "OneDrive" arba SharePoint administravimo centro nėra keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikinai skundams.</span><span class="sxs-lookup"><span data-stu-id="aaba9-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="aaba9-112">[Patikrinkite tarnybų sveikatos stebėjimo skydas](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="aaba9-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


