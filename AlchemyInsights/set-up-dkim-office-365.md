---
title: "\"DKIM\" sąranka"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808715"
---
# <a name="setup-dkim"></a>"DKIM" sąranka

[Čia](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)rasite instrukcijas, kaip sukonfigūruoti "DKIM" tinkintus domenus programoje "Microsoft 365".

1. **Kiekvienam** pasirinktiniam domenui turite sukurti **du** DKIM CNAME įrašus savo domeno DNS išteklių nuomos tarnyboje (paprastai tai yra domenų registratorius). Pvz., contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įra ų: du – contoso.com ir du – fourthcoffee.com.

   DKIM CNAME įrašų **kiekvienam** pasirinktiniam domenui naudokite šiuos formatus:

   - **Pagrindinio kompiuterio vardas**: `selector1._domainkey.<CustomDomain>`

     **Taškai adresu arba reikšmė**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     " **CTL**": 3600

   - **Pagrindinio kompiuterio vardas**: `selector2._domainkey.<CustomDomain>`

     **Taškai adresu arba reikšmė**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     " **CTL**": 3600

   \<DomainGUID\> yra `.mail.protection.outlook.com` pasirinktinio domeno tinkinto MX įrašo tekstas kairėje (pvz `contoso-com` ., domeno contoso.com). \<InitialDomain\> yra domenas, kurį naudojote, kai prisiregistravote naudoti "Microsoft 365" (pvz., contoso.onmicrosoft.com).

2. Sukūrę CNAME įra us savo pasirinktiniams domenams, atlikite toliau nurodytus veiksmus.

   a. [Prisijunkite prie "Microsoft 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) naudodami savo darbo arba mokymo įstaigos paskyrą.

   b. Pasirinkite taikomųjų programų vykdyklės piktogramą viršuje kairėje ir pasirinkite **administravimas**.

   c. Apatinėje kairiojoje naršymo srityje išplėskite **administravimas** ir pasirinkite " **Exchange**".

   d. Eikite į **apsaugos**  >  **DKIM**.

   e. Pasirinkite domeną, tada pasirinkite **įjungti** **šio domeno parašo pranešimą su DKIM parašais**. Pakartokite šį veiksmą su kiekvienu pasirinktiniu domenu.
