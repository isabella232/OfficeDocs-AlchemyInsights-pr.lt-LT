---
title: Modernus svetainės kaip šakninė svetainė
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232723"
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
