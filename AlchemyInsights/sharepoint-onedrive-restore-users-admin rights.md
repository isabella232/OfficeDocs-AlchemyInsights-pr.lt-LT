---
title: "\"Access\" nesuteiktų pranešimų trikčių šalinimas \"OneDrive\" verslui svetainėse"
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957801"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>"Access" nesuteiktų pranešimų trikčių šalinimas "OneDrive" verslui svetainėse

Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukuriamas tuo pačiu vartotojo vardu (UPN). Nauja paskyra sukuriama naudojant kitą PUID (Paso unikalus ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinį arba jo "OneDrive", vartotojas turi netinkamą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU). Jei vartotojai jau yra prisijungę prie SharePoint, tada perkeliami į kitą OU ir iš naujo sinchronizuojami su SharePoint, jiems gali kilti ši problema.

1. Norėdami išspręsti šią problemą, turite atkurti pradinį UPN, kaip nurodyta straipsnyje, [Atkurti vartotoją](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365 .
2. Jei negalite atkurti pradinio vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" naudodami šiuos veiksmus, [Pašalinkite]()vartotoją iš vartotojo informacijos sąrašo . 
3. Tai atlikę, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikę veiksmus, nurodytus Administratoriaus įtraukimas į [vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Daugiau informacijos apie teisių rinkinius žr. straipsnyje Apie teisių [rinkinius](https://docs.microsoft.com/sharepoint/understanding-permission-levels)SharePoint .
