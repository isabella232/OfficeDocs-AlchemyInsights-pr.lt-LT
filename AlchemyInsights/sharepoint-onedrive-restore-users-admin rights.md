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
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511192"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Prieigos uždraustų pranešimų į "OneDrive" verslui svetaines trikčių diagnostika

Ši problema dažniausiai kyla, kai vartotojas panaikinamas ir iš naujo sukuriamas su tuo pačiu vartotojo vardą (UPN). Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę. Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.

1. Norėdami išspręsti šią problemą, turėtumėte atkurti pradinį UPN su straipsnyje nurodytais veiksmais, [atkurti "Microsoft 365" vartotoją](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jei negalite atkurti pradinio vartotojo, turėtumėte pašalinti seną vartotoją iš "OneDrive" svetainės atlikdami šiuos veiksmus, [pašalinkite vartotoją iš vartotojo informacijos sąrašo](). 
3. Atlikę tai, galite patikrinti, ar vartotojas turi administratoriaus teises į "OneDrive" svetainę, atlikdami [veiksmus, norėdami įtraukti administratoriaus vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Daugiau informacijos apie teisių rinkinius ieškokite straipsnyje [Teisių lygių supratimas "SharePoint".](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
