---
title: Pašto dėžutės gavimo limito vykdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316041"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Pašto dėžutės gavimo limito vykdymas

"Microsoft" neseniai pradėjo vykdyti 3600 laiškų per valandą už pašto dėžutę ribą. Daugiau informacijos žr. [Exchange Online apribojimai](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 pašto dėžutės, kurios per valandą gauna daugiau nei 3 600 laiškų, per 60 min. yra sustos. 

Be to, taikoma siuntėjo ir gavėjo porų (SRP) riba, blokuojanti laiškus, Microsoft 365 iš konkretaus siuntėjo gaunamus laiškus. Jei vienas siuntėjas siunčia daugiau nei 33 % visos ribinės vertės arba 1200 laiškų per slenkamą valandą konkrečiam gavėjui, SRP limitas prasideda, o pašto dėžutė nebetinka laiškų iš to siuntėjo. Atkreipkite dėmesį, kad:

- Šis apribojimas taikomas el. laiškams, gautims iš kitų nuomotojų, vietinį arba interneto siuntėjus.
- El. laiškų pristatymas į pašto dėžutę blokuojamas per kitas 60 minučių. 
- Siuntėjai į šias pašto dėžutes gauna nepristatyto pristatymo ataskaitą (5.2.121 arba 5.2.122), kurioje nurodoma, kad pašto dėžutė viršijo didžiausią pristatymo ribą. Nuomotojo viduje (paštas tame pačiame nuomotoje) ir toliau pristatomas.
- Kai taikomas SRP limitas, gaunančioji pašto dėžutė ir toliau priima kitų siuntėjų laiškus.

Administratoriai gali stebėti dabartinę pašto dėžutės veiklą, pasiekdami naują ataskaitą ir įžvalgas Exchange administravimo centre, vadinamame "Pašto dėžutės, viršijančios gavimo apribojimus". Įžvalga rodoma tik jei nuomotojas turi įžeidžiančių pašto dėžučių, o ataskaita visada rodoma ataskaitų srityje, bet yra tuščia, nebent nuomotojas turi įžeidžiančių pašto dėžučių.

Daugiau informacijos apie įžvalgų gavimo apribojimus žr. Pašto [dėžutės, viršijančios gavimo apribojimų įžvalgas naujojoje EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Daugiau informacijos apie viršijančių gavimo apribojimų ataskaitą žr. Pašto dėžutės, viršijančios gavimo [limitų ataskaitą naujoje EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).