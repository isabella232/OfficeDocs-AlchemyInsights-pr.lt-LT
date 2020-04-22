---
title: Prieigos uždraustų pranešimų trikčių diagnostika
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758477"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Prieigos uždraustų pranešimų trikčių šalinimas "Sharepoint" / "OneDrive" administravimo centre

Jei bandydami naršyti "Sharepoint" / "OneDrive" administravimo centre gaunate pranešimą apie prieigą, kuriai uždrausta, įsitikinkite, kad [vartotojui suteikėte licenciją](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jam [priskirtas administratoriaus vaidmuo,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) galintis pasiekti administravimo centrus.

Ši problema taip pat gali kilti, kai vartotojas yra panaikintas ir iš naujo sukurtas su tuo pačiu vartotojo vardą (UPN). Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.

Norėdami išspręsti šią problemą, turite atkurti pradinį UPN su straipsnyje , [atkurti vartotojo "Microsoft 365".](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)

Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras nepasiekiamas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.  [Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).


