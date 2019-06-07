---
title: DKIM "Office 365" sąranka
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765253"
---
# <a name="setup-dkim-in-office-365"></a>DKIM "Office 365" sąranka

Visą instrukciją konfigūravimo DKIM pasirinktinius domenus "Office 365" yra [čia](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Kiekvieno** vartotojo domeno, turite sukurti **du** DKIM CNAME įrašus ne savo domeno DNS išteklių nuomos tarnybą (paprastai, domenų registratorius). Pvz., contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įra us: du contoso.com ir du fourthcoffee.com.

   DKIM CNAME įrašus apie **kiekvieno** individualiame domene naudoti šiuos formatus:

   - **Pagrindinio kompiuterio vardas**:`selector1._domainkey.<CustomDomain>`

     **Atkreipia dėmesį į adresą arba vertė**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Pagrindinio kompiuterio vardas**:`selector2._domainkey.<CustomDomain>`

     **Atkreipia dėmesį į adresą arba vertė**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> -tekstas kairėje `.mail.protection.outlook.com` į individualų pasirinktinio domeno MX įrašas (pavyzdžiui, `contoso-com` už domeno contoso.com). \<InitialDomain\> yra domenas, kurį naudojote, kai prisiregistravote prie "Office 365" (pvz., contoso.onmicrosoft.com).

2. Sukūrę CNAME įra us Pasirinktinių domenų, atlikite šiuos nurodymus:

   a. [Prisijunkite prie "Office 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) su savo darbovietės ar mokyklos paskyros.

   b. Pasirinkite programos paleidimo piktograma viršutiniame kairiajame ir **administratorius**.

   c. Apatiniame kairiajame naršymo, išplėskite **Admin** ir pasirinkite **Exchange**.

   d. Eikite į **saugos** > **DKIM**.

   e. Pasirinkite domeno, tada pasirinkite **įjungti** pranešimams **pasirašyti šio domeno su DKIM parašais**. Pakartokite šį veiksmą kiekvienam individualiame domene.
