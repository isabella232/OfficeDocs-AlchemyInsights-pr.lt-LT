---
title: Šiuolaikinė svetainė kaip šakninė svetainė
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713799"
---
# <a name="modern-site-as-root-site"></a>Šiuolaikinė svetainė kaip šakninė svetainė

Mes pradėjome diegti naują funkciją, kuri leis jums [apsikeitimo savo klasikinę svetainę šaknies svetainę su modernia svetaine.](https://docs.microsoft.com/sharepoint/modern-root-site) Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pakeisti svetainės vietą su kita svetaine, o archyvuoti pradinę svetainę. Galima naudoti ir komandos svetainėje (neprijungtoje prie grupės), ir ryšių svetainėje.

>[!Important]
> Neištrinkite savo klasikinės šaknies svetainės, kad sukurtumėte modernią komunikacijos svetainę. "Microsoft" to nepalaiko. Panaikinus šakninę svetainę visos jūsų organizacijos "SharePoint" svetainės taps nepasiekiamos visiems vartotojams, kol atkursite svetainę arba sukursite naują svetainę tuo pačiu URL. Mes bendrauti šią funkciją per pranešimų centrą. Turėtumėte tikėtis, kad funkcija bus įjungta jūsų nuomotojo netrukus.

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos, susijusios su svetainių swapping
- Paskirties svetainė gali pateikti klaidos "nerasta" (HTTP 404) trumpą laiką.
- Norint atnaujinti ieškos indeksą, turinį reikės nuskaityti iš naujo. Čia nereikia rankinio žingsnio, tai bus daroma automatiškai.
- Viskas, kas priklauso nuo "statinių" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti ištaisyta rankiniu būdu.
- Project Server svetainėse gali tekti patikrinti, siekiant užtikrinti, kad jie vis dar tinkamai susiję. 
