---
title: "\"SharePoint Online\" užklausų buferizavimas"
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931234"
---
# <a name="sharepoint-online-throttling"></a>"SharePoint Online" užklausų buferizavimas

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**503 serveris užimtas klaida**

Vartotojai gali gauti 503 serveris yra užimtas klaida bandant pereiti į SharePoint "arba" OneDrive svetainėse. 

Šią klaidą gali sukelti buferizavimas SharePoint tarnyboje. "SharePoint Online" naudoja buferizavimas, kad išlaikytų optimalų "SharePoint Online" paslaugos našumą ir patikimumą. Buferizavimas riboja vartotojo veiksmų arba vienu metu skambučių skaičių (pagal scenarijų arba kodą), kad būtų išvengta per daug išteklių. 

Jei norite gauti daugiau informacijos apie buferizavimas [pamatyti, Išvengti gauti throttled arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Jei manote, kad ši klaida nėra susijusi su buferizavimas, galite patikrinti, ar yra aktyvi priežiūra vyksta jūsų nuomotojo keliaudami į [pranešimų centrą](https://portal.office.com/adminportal/home#/MessageCenter).

 Galiausiai įsitikinkite, kad lankotės [puslapyje Tarnybos sveikata](https://portal.office.com/adminportal/home#/servicehealth) ir patikrinkite, ar nėra patarimų / incidentų, kurie gali įvykti.

