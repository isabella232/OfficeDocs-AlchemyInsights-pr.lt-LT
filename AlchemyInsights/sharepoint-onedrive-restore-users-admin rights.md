---
title: Prieigos uždraustų pranešimų į "OneDrive" verslui svetaines trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692809"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="94405-102">Prieigos uždraustų pranešimų į "OneDrive" verslui svetaines trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="94405-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="94405-103">Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukuriamas su tuo pačiu vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="94405-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="94405-104">Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="94405-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="94405-105">Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID.</span><span class="sxs-lookup"><span data-stu-id="94405-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="94405-106">Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="94405-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="94405-107">Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.</span><span class="sxs-lookup"><span data-stu-id="94405-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="94405-108">Norėdami išspręsti šią problemą, turėtumėte atkurti pradinį UPN su straipsnyje nurodytais veiksmais, [atkurti "Microsoft 365" vartotoją](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="94405-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="94405-109">Jei negalite atkurti pradinio vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" svetainės atlikdami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo]().</span><span class="sxs-lookup"><span data-stu-id="94405-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="94405-110">Atlikę tai, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikdami [veiksmus, norėdami įtraukti administratoriaus vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="94405-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="94405-111">Daugiau informacijos apie teisių rinkinius ieškokite straipsnyje [Teisių lygių supratimas "SharePoint".](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="94405-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
