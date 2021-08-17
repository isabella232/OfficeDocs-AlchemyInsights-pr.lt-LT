---
title: "\"Access Denied\" pranešimų trikčių šalinimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085236"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>"Access Denied" pranešimų trikčių šalinimas "Sharepoint" / "OneDrive" administravimo centre

Jei bandydami naršyti "Sharepoint" / ""OneDrive"" administravimo centre gaunate pranešimą, kuriam nesuteikta prieiga, įsitikinkite, kad [vartotojui priskiriate licenciją](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jam [priskirtas administratoriaus vaidmuo,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) kuris gali pasiekti administravimo centrus.

Ši problema taip pat gali kilti, kai vartotojas panaikinamas ir iš naujo sukuriamas tuo pačiu vartotojo vardu (UPN). Nauja paskyra sukuriama naudojant kitą PUID (Paso unikalus ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinį arba jo "OneDrive", vartotojas turi netinkamą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU). Jei vartotojai jau yra prisijungę prie SharePoint, tada perkeliami į kitą OU ir iš naujo sinchronizuojami su SharePoint, jiems gali kilti ši problema.

Norėdami išspręsti šią problemą, turėtumėte atkurti pradinį UPN, atlikite [veiksmus,](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)nurodytus straipsnyje Atkurti vartotoją Microsoft 365 .

Pastaba: jei "OneDrive" arba SharePoint administravimo centras negalimas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.  [Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).


