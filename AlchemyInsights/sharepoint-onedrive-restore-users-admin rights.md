---
title: Prieiga uždrausta pranešimų į "OneDrive" verslo svetainėms
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507819"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Prieiga uždrausta pranešimų į "OneDrive" verslo svetainėms

Ši problema dažniausiai kyla, kai vartotojas yra panaikinti ir iš naujo sukurti patį vartotojo vardą (UPN). Sukūrus abonementą sukuriamas naudojant skirtingus PUID (paso unikalų ID) reikšmę. Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai turi jau prisijungę prie SharePoint, tada persikėlė į skirtingas OU ir resynced su "SharePoint", jie gali kilti ši problema.

1. Norėdami išspręsti šią problemą turite atkurti originalų UPN su straipsnyje,[atkurti vartotojo "Office 365"](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)nurodytus veiksmus.
2. Jei negalėsite atkurti pradinio vartotojo senas vartotojas turėtų pašalinti atlikdami šiuos veiksmus, [pašalinti iš vartotojo informacijos sąraše vartotojo]()"OneDrive" svetainę. 
3. Po to, kai tai bus padaryta, galite patikrinti turi administratoriaus teises į "OneDrive" svetainę atlikdami nurodytus veiksmus norėdami [pridėti admin's vartotojo "OneDrive"](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Daugiau informacijos apie teisių lygius, ieškokite straipsnyje, [suprasti teisių lygius programoje "SharePoint"](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
