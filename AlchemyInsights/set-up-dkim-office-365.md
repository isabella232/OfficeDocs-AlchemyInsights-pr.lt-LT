---
title: DKIM sąranka
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108564"
---
# <a name="setup-dkim"></a>DKIM sąranka

Čia pateikiamos išsamios vartotojo domenų DKIM konfigūravimo Microsoft 365 [čia.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Kiekvienam **pasirinktiniam** domenui turite sukurti du **DKIM** CNAME įrašus savo domeno DNS išteklių nuomos tarnybos (paprastai domenų registratoriaus) svetainėje. Pvz., contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įrašų: du – contoso.com, o du – fourthcoffee.com.

   Kiekvieno pasirinktinio domeno DKIM CNAME **įrašai** naudoja šiuos formatus:

   - **Pagrindinio kompiuterio vardas**: `selector1._domainkey.<CustomDomain>`

     **Nurodo adresą arba reikšmę:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Pagrindinio kompiuterio vardas**: `selector2._domainkey.<CustomDomain>`

     **Nurodo adresą arba reikšmę:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> yra pasirinktinio domeno tinkinto MX įrašo kairėje esantis tekstas `.mail.protection.outlook.com` (pvz., `contoso-com` domeno contoso.com). \<InitialDomain\>yra domenas, kurį naudojote prisiregistravę naudoti Microsoft 365 (pvz., contoso.onmicrosoft.com).

2. Sukūrę pasirinktinių domenų CNAME įrašus, užpildykite šias instrukcijas:

   a. [prisijunkite prie Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) naudodami savo darbo arba mokymo įstaigos paskyrą.

   b. Pasirinkite taikomųjų programų vykdyklės piktogramą viršutiniame kairiajame kampe ir pasirinkite **Administravimas**.

   c. Apatinėje kairiojoje naršymo srityje išplėskite **Administravimas** ir **pasirinkite Exchange**.

   d. Eikite **į Apsaugos**  >  **DKIM**.

   e. Pasirinkite domeną, tada pasirinkite **Įgalinti,** kad **būtų pasirašyti šio domeno laiškai su DKIM parašais.** Kartokite šį veiksmą su kiekvienu pasirinktiniu domenu.
