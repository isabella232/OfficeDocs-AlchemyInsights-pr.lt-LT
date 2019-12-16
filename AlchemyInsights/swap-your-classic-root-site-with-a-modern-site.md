---
title: Sukeisti savo Classic šaknų svetainę su šiuolaikinės svetainės
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042935"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Sukeisti savo Classic šaknų svetainę su šiuolaikinės svetainės

Jei jūsų aplinka buvo nustatyta iki balandžio 2019 d., galite pakeisti savo šakninę svetainę į modernią svetainę naudodami "Microsoft PowerShell":

- Jei turite kitą svetainę, kurią norite naudoti kaip savo šakninę svetainę, galite pakeisti [(keisti) šakninę svetainę](https://docs.microsoft.com/sharepoint/modern-root-site) su ja. 
    - Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo vietą su kita svetaine, o archyvuojama originali svetainės vieta. Pasiekiama tiek komandos svetainei (neprisijungtoms prie grupės), tiek bendravimo svetainei. 

- Netrukus bus įvesta papildomų galimybių, kurios leis jums išlaikyti naudojant svetainės turinį, bet konvertuoti esamą svetainę į komunikacijos svetainę. 
>[!Important]
>Šios galimybės bus diegiamos palaipsniui. Toliau tikrinkite "Office 365" pranešimų centro naujinimus. 

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos su svetainių keitimu

- Paskirties svetainė gali grąžinti "nerastas" (HTTP 404) klaidos trumpą laiką.
- Turinys turi būti aptinkama atnaujinti paieškos indeksą. Nėra rankinio žingsnio reikia-tai bus daroma automatiškai.
- Viskas priklauso nuo "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) reikės rankiniu būdu ištaisyti.
- Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.Gaukite visų organizacinių naujienų svetainių sąrašą.
- "Project Server" svetaines gali reikėti patvirtinti, siekiant užtikrinti, kad jos vis dar tinkamai susietos.





