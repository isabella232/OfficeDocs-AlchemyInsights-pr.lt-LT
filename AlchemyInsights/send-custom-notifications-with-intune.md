---
title: Pasirinktinio pranešimų siuntimas naudojant "Intune"
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720654"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kaip nusiųsti pritaikytus pranešimus valdomoms "iOS" ir "Android" įrenginiams vartotojams

Pasirinktinio naudojimo pranešimus, skirtus "Intune", tvarko įmonės portalo programėlė vartotojo įrenginyje. Tada programa sukuria "Push" pranešimą tame įrenginyje.

Toliau nurodyti įrenginio Būtinosios sąlygos, skirtos palaikyti pasirinktiniams pranešimams gavimą, o tada programėlei sukurti "Push" pranešimą:

- Įrenginyje turi būti įdiegta įmonės portalo taikomoji programa.  

- Įrenginys turi leisti įmonės portalo taikomajai programai išsiųsti "Push" pranešimus. Kai taikomoji programa įdiegiama arba atnaujinama, ji paragins vartotoją leisti pranešimus.

- "Android" įrenginiuose turi būti įdiegtos "Google Play" paslaugos.

- Įrenginys turi būti užregistruotas su Intune.

Daugiau informacijos, įskaitant pranešimo siuntimą, rasite [funkcijų dokumentacijoje](https://docs.microsoft.com/intune/custom-notifications).
