---
title: Moderni svetainė kaip šakninė svetainė
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327610"
---
# <a name="modern-site-as-root-site"></a>Moderni svetainė kaip šakninė svetainė

Pradėjome įdiegti naują funkciją, kuri leis jums pakeisti klasikinę svetainės šakninį puslapį [modernia svetaine.](https://docs.microsoft.com/sharepoint/modern-root-site) Naudokite [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kad sukeisti svetainės vietą su kita svetaine archyvavimo metu pradinėje svetainėje. Galima naudoti tiek komandos svetainėje (neprijungtoje prie grupės), tiek ryšių svetainėje.

**Svarbu:** nepanaikykite klasikinės šakninės svetainės, kad sukurtumėte šiuolaikišką ryšių svetainę. "Microsoft" to nepalaiko. Panaikinus šakninį puslapį, visos jūsų SharePoint svetainės taps nepasiekiamos visiems vartotojams, kol atkursite svetainę arba sukursite naują svetainę tuo pačiu URL. Šią funkciją pereisime per pranešimų centrą. Turėtumėte tikėtis, kad netrukus jūsų nuomotojo funkcija bus įjungta.

## <a name="known-issues-with-swapping-sites"></a>Žinomos svetainių apsikeitimo problemos
- Paskirties svetainė trumpą laiką gali pateikti klaidą "nerasta" (HTTP 404).
- Norint atnaujinti ieškos indeksą, turi būti atirašytas turinys. Čia nėra reikalingų rankinių veiksmų, tai bus atliekama automatiškai.
- Viską, kas priklauso nuo "statinių" saitų (pvz., Failų sinchronizavimas ir OneNote failų), reikės pataisyti rankiniu būdu.
- Project Serverio svetaines gali tekti patikrinti, kad jos būtų tinkamai susietos. 
