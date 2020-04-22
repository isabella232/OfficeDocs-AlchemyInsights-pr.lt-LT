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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Prieigos uždraustų pranešimų į "OneDrive" verslui svetaines trikčių diagnostika

Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukuriamas su tuo pačiu vartotojo vardą (UPN). Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.

1. Norėdami išspręsti šią problemą, turėtumėte atkurti pradinį UPN su straipsnyje nurodytais veiksmais, [atkurti "Microsoft 365" vartotoją](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jei negalite atkurti pradinio vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" svetainės atlikdami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo](). 
3. Atlikę tai, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikdami [veiksmus, norėdami įtraukti administratoriaus vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Daugiau informacijos apie teisių rinkinius ieškokite straipsnyje [Teisių lygių supratimas "SharePoint".](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
