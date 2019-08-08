---
title: Apsikeitimo savo klasikinis šakninė svetainė su moderni svetainė
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246029"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Apsikeitimo savo klasikinis šakninė svetainė su moderni svetainė

Jei jūsų aplinkoje buvo nustatytas iki 2019 m. balandžio, galite pakeisti savo šakninėje svetainėje prie šiuolaikinės svetainės naudodami Microsoft PowerShell:

- Jei turite kitą svetainę, kurią norite naudoti kaip šakninę svetainę, galite pakeisti (apsikeitimo) šaknis svetainę su juo. 
    - Naudokite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo su kita svetaine svetainės vietą, o archyvavimo originalų puslapį. Galima komandos svetainėje (nėra prijungtas prie grupės) bei bendravimo svetainės. 

- Papildomus pajėgumus pradės veikti greitai, leis jums išlaikyti naudojant turinio svetainėje, bet ir konvertuoti esamą svetainę pranešimas svetainė. 
>[!Important]
>Šie pajėgumai bus diegiamos palaipsniui. Ir toliau tikrins, ar yra naujinimų Office 365 pranešimų centras. 

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos su apsikeitimo svetaines

- Tikslinės svetainės gali grįžti su "nerasta" klaida (HTTP 404) per trumpą laiką.
- Medžiaga turi būti recrawled į paieškos indeksą atnaujinti. Nėra jokių rankiniu būdu pirmiausia reikia - tai bus padaryta automatiškai.
- Nieko priklauso "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) turės rankiniu būdu ištaisyti.
- Jei šaltinio svetainė buvo organizacijos naujienų svetainę, atnaujinti URL.Gauti visus organizacinius naujienų svetainių sąrašą.
- Projekto serverio svetainėse gali tekti būti patikrintas siekiant užtikrinti, kad jie dar siejama teisingai.





