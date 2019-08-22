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
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503541"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive administravimo centro pranešimus Prieiga uždrausta trikčių diagnostika

Jei gaunate kad prieiga uždrausta bandant naršyti į Sharepoint/OneDrive administravimo centrą pranešimą, prašome įsitikinti, kad turite [Priskirti licenciją vartotojui](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jei vartotojas turi licenciją, taip pat būtinai yra [priskirtas administratoriaus vaidmenį](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , galite pasiekti admin centrai.

Ši problema gali atsirasti, kai vartotojo panaikinti ir iš naujo sukurti patį vartotojo vardą (UPN). Sukūrus abonementą sukuriamas naudojant skirtingus PUID (paso unikalų ID) reikšmę. Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai turi jau prisijungę prie SharePoint, tada persikėlė į skirtingas OU ir resynced su "SharePoint", jie gali kilti ši problema.

Norėdami išspręsti šią problemą, turite atkurti originalų UPN su straipsnyje, [atkurti vartotojo "Office 365"](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)nurodytus veiksmus.

Pastaba: Jei "OneDrive" arba SharePoint administravimo centro nėra keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikinai skundams.  [Patikrinkite tarnybų sveikatos stebėjimo skydas](https://portal.office.com/adminportal/home#/servicehealth).


