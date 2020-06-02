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
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505387"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Prieigos uždraustų pranešimų trikčių šalinimas "Sharepoint" / "OneDrive" administravimo centre

Jei bandydami naršyti "Sharepoint" / "OneDrive" administravimo centre gaunate pranešimą apie prieigą, kuriai uždrausta, įsitikinkite, kad [vartotojui suteikėte licenciją](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jam [priskirtas administratoriaus vaidmuo,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) galintis pasiekti administravimo centrus.

Ši problema taip pat gali kilti, kai vartotojas yra panaikintas ir iš naujo sukurtas su tuo pačiu vartotojo vardą (UPN). Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.

Norėdami išspręsti šią problemą, turite atkurti pradinį UPN su straipsnyje , [atkurti vartotojo "Microsoft 365".](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras nepasiekiamas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.  [Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).


