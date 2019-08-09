---
title: Modernus svetainės kaip šakninė svetainė
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269384"
---
# <a name="modern-site-as-root-site"></a>Modernus svetainės kaip šakninė svetainė

Mes pradėjome įdiegiant naują funkciją, kuri leis jums apsikeitimo jūsų classic svetainę šakninė svetainė su šiuolaikinės svetainės. Naudokite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo su kita svetaine svetainės vietą, o archyvavimo originalų puslapį. Galima komandos svetainėje (nėra prijungtas prie grupės) bei bendravimo svetainės. 

>[!Important]
> Ne ištrinti savo "classic" šaknų svetainę sukurti šiuolaikinės komunikacijos svetainę. Tai nėra palaikoma "Microsoft". Panaikinus šakninė svetainė leis visus "SharePoint" svetainių organizacijoje neprieinama visiems naudotojams, tol, kol galite atkurti į svetainės arba sukurti naują svetainę tuo pačiu URL. Mes bus perduoti šią funkciją per pranešimų centras. Reikia tikėtis funkciją galima įjungti į savo nuomotojo artimiausiu metu.

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos su apsikeitimo svetaines
- Tikslinės svetainės gali grįžti su "nerasta" klaida (HTTP 404) per trumpą laiką.
- Medžiaga turi būti recrawled į paieškos indeksą atnaujinti. Nėra jokių rankiniu būdu pirmiausia reikia čia, tai bus padaryta automatiškai.
- Nieko priklauso "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) turės rankiniu būdu ištaisyti.
- Projekto serverio svetainėse gali tekti būti patikrintas siekiant užtikrinti, kad jie dar siejama teisingai. 
