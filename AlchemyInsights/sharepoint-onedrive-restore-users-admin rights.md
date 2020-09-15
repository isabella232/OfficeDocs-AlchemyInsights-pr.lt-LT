---
title: Prieigos prie "OneDrive" verslui svetainių trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670624"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="0f31b-102">Prieigos prie "OneDrive" verslui svetainių trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="0f31b-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="0f31b-103">Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir sukuriamas iš naujo su tuo pačiu vartotojo pagrindiniu pavadinimu (UPN).</span><span class="sxs-lookup"><span data-stu-id="0f31b-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="0f31b-104">Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="0f31b-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="0f31b-105">Kai vartotojas bandys pasiekti svetainių rinkinį arba savo "OneDrive", vartotojas turi neteisingą PUID.</span><span class="sxs-lookup"><span data-stu-id="0f31b-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="0f31b-106">Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU).</span><span class="sxs-lookup"><span data-stu-id="0f31b-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="0f31b-107">Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą "SharePoint", jie gali susidurti su šia problema.</span><span class="sxs-lookup"><span data-stu-id="0f31b-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="0f31b-108">Norėdami išspręsti šią problemą, atkurkite pradinę UPN su straipsnyje veiksmais, [atkurkite vartotoją "Microsoft 365"](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="0f31b-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="0f31b-109">Jei negalite atkurti pirminio vartotojo, turite pašalinti senąjį vartotoją iš "OneDrive" svetainės, naudodami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo]().</span><span class="sxs-lookup"><span data-stu-id="0f31b-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="0f31b-110">Tai atlikę, galite patvirtinti, kad vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikdami veiksmus, kaip [įtraukti administratoriaus vartotojo "OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) "</span><span class="sxs-lookup"><span data-stu-id="0f31b-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="0f31b-111">Daugiau informacijos apie teisių rinkinius ieškokite straipsnyje " [SharePoint" teisių rinkinių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0f31b-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
