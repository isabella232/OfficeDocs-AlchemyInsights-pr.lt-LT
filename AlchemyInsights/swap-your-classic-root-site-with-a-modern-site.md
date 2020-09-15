---
title: Klasikinės šaknies svetainės keitimas naudojant šiuolaikinę svetainę
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691187"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasikinės šaknies svetainės keitimas naudojant šiuolaikinę svetainę

Jei jūsų aplinka buvo nustatyta iki balandžio 2019, galite pakeisti savo šaknies svetainę į šiuolaikinę svetainę naudodami "Microsoft PowerShell":

- Jei turite kitą svetainę, kurią norite naudoti kaip savo šaknies svetainę, galite pakeisti [(sukeisti) šaknies svetainę](https://docs.microsoft.com/sharepoint/modern-root-site) su ja. 
    - Naudokite funkciją [Invoke – SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Norėdami sukeisti svetainės vietą su kita svetaine archyvuodami pradinę svetainę. Galima naudoti ir komandos svetainėje (nėra prijungta prie grupės) ir bendravimo svetainėje. 

- Netrukus bus įdiegtos papildomos galimybės, leidžiančios toliau naudoti svetainės turinį, bet konvertuoti esamą svetainę į ryšių svetainę. 
>[!Important]
>Šie pajėgumai bus palaipsniui išskleidžiami. Toliau tikrinkite naujinimų centro naujinimus. 

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos keičiant svetaines

- Paskirties svetainė trumpą laiką gali pateikti klaidą "nerastas" (HTTP 404).
- Turiniui atnaujinti reikia atnaujinti ieškos indeksą. Nėra reikalingo rankinio veiksmo – tai bus atlikta automatiškai.
- Viskas, kas priklauso nuo "statinio" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti rankiniu būdu pataisyta.
- Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.Gaukite visų organizacijos naujienų svetainių sąrašą.
- "Project Server" svetaines gali reikėti patvirtinti, kad jos būtų tinkamai susietos.
