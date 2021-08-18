---
title: Klasikinės šakninės svetainės sukeitimas naudojant modernią svetainę
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316148"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasikinės šakninės svetainės sukeitimas naudojant modernią svetainę

Jei jūsų aplinka buvo nustatyta iki 2019 m. balandžio mėn., galite pakeisti šakninį puslapį į šiuolaikišką svetainę naudodami "Microsoft PowerShell":

- Jei turite kitą svetainę, kurią norite naudoti kaip šakninį puslapį, galite ją pakeisti [(sukeisti).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Naudokite [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kad sukeisti svetainės vietą su kita svetaine archyvavimo metu pradinėje svetainėje. Galima naudoti tiek komandos svetainėje (neprijungtoje prie grupės), tiek ryšių svetainėje. 

- Netrukus bus įvestos papildomos galimybės, kurios leis toliau naudoti svetainės turinį, bet konvertuoti esamą svetainę į ryšių svetainę. 

**Svarbu:** šios galimybės bus išsiųstos palaipsniui. Toliau patikrinkite, ar pranešimų centre yra naujinimų. 

## <a name="known-issues-with-swapping-sites"></a>Žinomos svetainių apsikeitimo problemos

- Paskirties svetainė trumpą laiką gali pateikti klaidą "nerasta" (HTTP 404).
- Norint atnaujinti ieškos indeksą, turi būti atirašytas turinys. Nereikia atlikti rankinio veiksmo – tai bus atliekama automatiškai.
- Viską, kas priklauso nuo "statinių" saitų (pvz., Failų sinchronizavimas ir OneNote failų), reikės pataisyti rankiniu būdu.
- Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL. Gaukite visų organizacijos naujienų svetainių sąrašą.
- Project Serverio svetaines gali tekti patikrinti, kad jos būtų tinkamai susietos.
