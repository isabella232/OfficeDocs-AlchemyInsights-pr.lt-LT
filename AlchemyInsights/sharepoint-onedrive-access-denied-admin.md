---
title: Trikčių diagnostika prieiga uždrausta pranešimai
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051433"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>"SharePoint"/"OneDrive" administravimo centro pranešimų prieiga uždrausta trikčių diagnostika

Jei gaunate pranešimą prieiga uždrausta bandant naršyti SharePoint/OneDrive administravimo centras, įsitikinkite, kad jums [Priskirti licenciją vartotojui](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jiems [priskirtas administratoriaus vaidmuo](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , kuris gali pasiekti administravimo centrus.

Ši problema taip pat gali kilti, kai vartotojas panaikinamas ir iš naujo sukurtas naudojant tą patį vartotojo vardą (UPN). Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimas su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", ir tada perkeliami į kitą OU ir resynced su "SharePoint", jie gali kilti ši problema.

Norėdami išspręsti šią problemą, turite atkurti pradinį UPN su straipsnyje nurodytus veiksmus, [atkurti vartotojo Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras yra neprieinama keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikinas tarnybos problema.  [Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).


