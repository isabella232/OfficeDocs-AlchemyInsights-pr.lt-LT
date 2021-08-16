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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000400"
---
# <a name="modern-site-as-root-site"></a>Moderni svetainė kaip šakninė svetainė

Pradėjome įdiegti naują funkciją, kuri leis jums pakeisti klasikinę svetainės šakninį puslapį [modernia svetaine.](https://docs.microsoft.com/sharepoint/modern-root-site) Naudokite [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kad sukeisti svetainės vietą su kita svetaine archyvavimo metu pradinėje svetainėje. Galima naudoti tiek komandos svetainėje (neprijungtoje prie grupės), tiek ryšių svetainėje.

>[!Important]
> Nepanaikykite klasikinės šakninės svetainės, kad sukurtumėte šiuolaikišką ryšių svetainę. "Microsoft" to nepalaiko. Panaikinus šakninį puslapį, visos jūsų SharePoint svetainės taps nepasiekiamos visiems vartotojams, kol atkursite svetainę arba sukursite naują svetainę tuo pačiu URL. Šią funkciją pereisime per pranešimų centrą. Turėtumėte tikėtis, kad netrukus jūsų nuomotojo funkcija bus įjungta.

## <a name="known-issues-with-swapping-sites"></a>Žinomos svetainių apsikeitimo problemos
- Paskirties svetainė trumpą laiką gali pateikti klaidą "nerasta" (HTTP 404).
- Norint atnaujinti ieškos indeksą, turi būti atirašytas turinys. Čia nėra reikalingų rankinių veiksmų, tai bus atliekama automatiškai.
- Viską, kas priklauso nuo "statinių" saitų (pvz., Failų sinchronizavimas ir OneNote failų), reikės pataisyti rankiniu būdu.
- Project Gali tekti patikrinti serverio svetaines, kad jos būtų tinkamai susietos. 
