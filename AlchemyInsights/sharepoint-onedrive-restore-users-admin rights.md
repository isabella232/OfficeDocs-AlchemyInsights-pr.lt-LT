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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Prieigos prie "OneDrive" verslui svetainių trikčių diagnostika

Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir sukuriamas iš naujo su tuo pačiu vartotojo pagrindiniu pavadinimu (UPN). Naujas abonementas sukuriamas naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bandys pasiekti svetainių rinkinį arba savo "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su "Active Directory" organizacijos vienetu (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą "SharePoint", jie gali susidurti su šia problema.

1. Norėdami išspręsti šią problemą, atkurkite pradinę UPN su straipsnyje veiksmais, [atkurkite vartotoją "Microsoft 365"](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jei negalite atkurti pirminio vartotojo, turite pašalinti senąjį vartotoją iš "OneDrive" svetainės, naudodami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo](). 
3. Tai atlikę, galite patvirtinti, kad vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikdami veiksmus, kaip [įtraukti administratoriaus vartotojo "OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) "

Daugiau informacijos apie teisių rinkinius ieškokite straipsnyje " [SharePoint" teisių rinkinių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
