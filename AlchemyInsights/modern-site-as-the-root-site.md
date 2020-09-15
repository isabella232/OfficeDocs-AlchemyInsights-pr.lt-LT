---
title: Moderni svetainė kaip pagrindinė svetainė
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666878"
---
# <a name="modern-site-as-root-site"></a>Moderni svetainė kaip pagrindinė svetainė

Pradėjome naudoti naują funkciją, kuri leis jums [sukeisti klasikinės svetainės šaknies svetainę su šiuolaikine svetaine](https://docs.microsoft.com/sharepoint/modern-root-site). Naudokite funkciją [Invoke – SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Norėdami sukeisti svetainės vietą su kita svetaine archyvuodami pradinę svetainę. Galima naudoti ir komandos svetainėje (nėra prijungta prie grupės) ir bendravimo svetainėje.

>[!Important]
> Nepanaikinkite klasikinės šaknies svetainės kurdami šiuolaikinę bendravimo svetainę. Tai nepalaiko "Microsoft". Panaikinus svetainę, visos jūsų organizacijos "SharePoint" svetainės bus prieinamos visiems vartotojams, kol neatkursite svetainės arba sukursite naują svetainę tame pačiame URL. Perduodame šią funkciją per pranešimų centrą. Turėtumėte tikėtis, kad funkcija bus įjungta jūsų nuomotojuje artimiausiu metu.

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos keičiant svetaines
- Paskirties svetainė trumpą laiką gali pateikti klaidą "nerastas" (HTTP 404).
- Turiniui atnaujinti reikia atnaujinti ieškos indeksą. Čia nereikia atlikti rankinio veiksmo, tai bus atlikta automatiškai.
- Viskas, kas priklauso nuo "statinio" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti rankiniu būdu pataisyta.
- "Project Server" svetaines gali reikėti patvirtinti, kad jos būtų tinkamai susietos. 
