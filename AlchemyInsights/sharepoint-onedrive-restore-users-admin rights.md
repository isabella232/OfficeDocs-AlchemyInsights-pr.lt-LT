---
title: Trikčių diagnostikos prieiga uždrausta pranešimus į "OneDrive" verslui svetainės
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766719"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Trikčių diagnostikos prieiga uždrausta pranešimus į "OneDrive" verslui svetainės

Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukurtas naudojant tą patį vartotojo vardą (UPN). Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimas su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", ir tada perkeliami į kitą OU ir resynced su "SharePoint", jie gali kilti ši problema.

1. Norėdami išspręsti šią problemą, reikia atkurti pradinį UPN su straipsnyje nurodytus veiksmus, [atkurti vartotojo Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jei negalite atkurti originalaus vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" svetainės atlikdami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo](). 
3. Kai tai padarysite, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę atlikdami veiksmus, Norėdami [pridėti administratoriaus vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Daugiau informacijos apie teisių lygius rasite straipsnyje " [SharePoint" teisių lygių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
