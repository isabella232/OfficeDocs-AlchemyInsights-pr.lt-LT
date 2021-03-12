---
title: "\"Access\" uždraustų žinučių trikčių diagnostika"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707962"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="1bb17-102">Prieigos prie "SharePoint"/"OneDrive" administravimo centre trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="1bb17-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="1bb17-103">Jei bandydami naršyti "SharePoint"/"OneDrive" administravimo centre gaunate pranešimą "prieiga uždrausta", įsitikinkite, kad [vartotojui priskiriate licenciją](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="1bb17-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="1bb17-104">Jei vartotojas turi licenciją, taip pat įsitikinkite, kad jiems [priskirtas administratoriaus vaidmuo](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , kuris gali pasiekti administravimo centrus.</span><span class="sxs-lookup"><span data-stu-id="1bb17-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="1bb17-105">Ši problema taip pat gali įvykti, kai vartotojas panaikinamas ir sukuriamas iš naujo su tuo pačiu vartotojo pagrindiniu pavadinimu (UPN).</span><span class="sxs-lookup"><span data-stu-id="1bb17-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="1bb17-106">Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1bb17-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="1bb17-107">Kai vartotojas bandys pasiekti svetainių rinkinį arba savo "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="1bb17-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="1bb17-108">Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU).</span><span class="sxs-lookup"><span data-stu-id="1bb17-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="1bb17-109">Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą "SharePoint", jie gali susidurti su šia problema.</span><span class="sxs-lookup"><span data-stu-id="1bb17-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="1bb17-110">Norėdami išspręsti šią problemą, atkurkite pradinę UPN su straipsnyje veiksmais, [atkurkite vartotoją "Microsoft 365"](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="1bb17-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="1bb17-111">Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras nepasiekiamas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.</span><span class="sxs-lookup"><span data-stu-id="1bb17-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="1bb17-112">[Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1bb17-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


