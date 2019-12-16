---
title: Šiuolaikinė svetainė kaip šakninė svetainė
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054710"
---
# <a name="modern-site-as-root-site"></a>Šiuolaikinė svetainė kaip šakninė svetainė

Mes pradėjome rida naują funkciją, kuri leis jums [apsikeitimo savo Classic svetainę šaknų svetainę su modernia svetaine](https://docs.microsoft.com/sharepoint/modern-root-site). Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo vietą su kita svetaine, o archyvuojama originali svetainės vieta. Pasiekiama tiek komandos svetainei (neprisijungtoms prie grupės), tiek bendravimo svetainei.

>[!Important]
> Nenaikinkite savo klasikinės Šakninės svetainės, kad sukurtumėte modernią bendravimo svetainę. Tai nepalaiko Microsoft. Panaikinus šakninę svetainę visos organizacijos SharePoint svetainės bus neprieinamos visiems vartotojams, kol neatkursite svetainės arba nesukursite naujos svetainės tuo pačiu URL. Mes susisieksime su šia funkcija per pranešimų centrą. Turėtumėte tikėtis, kad funkcija turi būti įjungtas jūsų nuomininkas netrukus.

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos su svetainių keitimu
- Paskirties svetainė gali grąžinti "nerastas" (HTTP 404) klaidos trumpą laiką.
- Turinys turi būti aptinkama atnaujinti paieškos indeksą. Nėra rankinio žingsnio reikia čia, tai bus daroma automatiškai.
- Viskas priklauso nuo "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) reikės rankiniu būdu ištaisyti.
- "Project Server" svetaines gali reikėti patvirtinti, siekiant užtikrinti, kad jos vis dar tinkamai susietos. 
