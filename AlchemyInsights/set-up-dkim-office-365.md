---
title: Nustatyti DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645680"
---
# <a name="setup-dkim"></a>Nustatyti DKIM

Išsami instrukcija konfigūruoti DKIM pasirinktinių domenų Microsoft 365 yra [čia](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Kiekvienam** pasirinktiniam domenui turite sukurti **du** DKIM CNAME įrašus domeno DNS išteklių nuomos tarnyboje (paprastai domenų registratoriuje). Pavyzdžiui, contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įrašų: du contoso.com ir du fourthcoffee.com.

   DKIM CNAME įrašai **kiekvienam** pasirinktiniam domenui naudoja šiuos formatus:

   - **Pagrindinio kompiuterio vardas**:`selector1._domainkey.<CustomDomain>`

     **Nukreipia adresu arba reikšmė:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Pagrindinio kompiuterio vardas**:`selector2._domainkey.<CustomDomain>`

     **Nukreipia adresu arba reikšmė:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> yra pasirinktinio domeno `.mail.protection.outlook.com` tinkinto MX įrašo tekstas į kairę (pvz., `contoso-com` domeno contoso.com). \<InitialDomain\> yra domenas, kurį naudojote prisiregistruodami naudoti "Microsoft 365" (pvz., contoso.onmicrosoft.com).

2. Sukūrę pasirinktinių domenų CNAME įrašus, atlikite toliau nurodytas instrukcijas:

   A. [prisijunkite prie "Microsoft 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) naudodami savo darbo arba mokymo įstaigos paskyrą.

   B. Viršutiniame kairiajame kampe pasirinkite taikomųjų programų vykdyklės piktogramą ir pasirinkite **Administravimas**.

   C. Apatinėje kairiojoje naršymo srityje išplėskite **Administravimas** ir pasirinkite **Exchange**.

   D. Eikite į **Apsauga** > **DKIM**.

   E. Pasirinkite domeną, tada pasirinkite **Įgalinti** **šio domeno pranešimams pasirašyti su DKIM parašais**. Pakartokite šį veiksmą su kiekvienu pasirinktiniu domenu.
