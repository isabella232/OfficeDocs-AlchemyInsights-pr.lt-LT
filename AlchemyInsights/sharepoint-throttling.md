---
title: "\"SharePoint Online\" užklausų buferizavimas"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931450"
---
# <a name="sharepoint-online-throttling"></a>"SharePoint Online" užklausų buferizavimas

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**"SharePoint Online" užklausų buferizavimas**

"SharePoint Online" naudoja buferizavimas, kad išlaikytų optimalų "SharePoint Online" paslaugos našumą ir patikimumą. Buferizavimas riboja vartotojo veiksmų arba vienu metu skambučių skaičių (pagal scenarijų arba kodą), kad būtų išvengta per daug išteklių. Norėdami gauti daugiau informacijos, apsilankykite žemiau pateiktose nuorodose.

- ["SharePoint Online" neužblokavo arba neužblokavo](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Duomenų perkėlimas ir SPO buferizavimas](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- ["SharePoint Online" ir "OneDrive" perkėlimo greitis](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - ["SharePoint Online" užklausų buferizavimas naudojant eksponentinį atgal](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Pajėgumų planavimas ir apkrovos testavimas "SharePoint Online"](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

