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
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Prieigos prie "SharePoint"/"OneDrive" administravimo centre trikčių šalinimas

Jei bandydami naršyti "SharePoint"/"OneDrive" administravimo centre gaunate pranešimą "prieiga uždrausta", įsitikinkite, kad [vartotojui priskiriate licenciją](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jei vartotojas turi licenciją, taip pat įsitikinkite, kad jiems [priskirtas administratoriaus vaidmuo](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , kuris gali pasiekti administravimo centrus.

Ši problema taip pat gali įvykti, kai vartotojas panaikinamas ir sukuriamas iš naujo su tuo pačiu vartotojo pagrindiniu pavadinimu (UPN). Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bandys pasiekti svetainių rinkinį arba savo "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą "SharePoint", jie gali susidurti su šia problema.

Norėdami išspręsti šią problemą, atkurkite pradinę UPN su straipsnyje veiksmais, [atkurkite vartotoją "Microsoft 365"](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras nepasiekiamas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.  [Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).


