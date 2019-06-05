---
title: Suteikti vartotojams prieigą prie SharePoint ir "OneDrive"
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715219"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Suteikti vartotojams prieigą prie SharePoint ir "OneDrive"

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ši problema dažniausiai kyla, kai vartotojas yra panaikinti ir iš naujo sukurti patį vartotojo vardą (UPN). Sukūrus abonementą sukuriamas naudojant skirtingus PUID (paso unikalų ID) reikšmę. Kai vartotojas bando prieiti prie svetainių rinkinio arba jų "OneDrive", vartotojas turi neteisingą PUID. Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU). Jei vartotojai turi jau prisijungę prie SharePoint, tada persikėlė į skirtingas OU ir resynced su "SharePoint", jie gali kilti ši problema.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Norėdami išspręsti šią problemą, turite atkurti originalų UPN veiksmus šiame straipsnyje, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">atkurti vartotojo "Office 365".</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Po to, kai tai bus padaryta, galite patikrinti turi administratoriaus teises į "OneDrive" svetainę atlikdami veiksmus, nurodytus prie <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">pridėti administratoriaus vartotojo "OneDrive".</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Daugiau informacijos apie teisių lygius, ieškokite straipsnyje, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">suprasti teisių lygius SharePoint.</a>&nbsp;</span></p>
