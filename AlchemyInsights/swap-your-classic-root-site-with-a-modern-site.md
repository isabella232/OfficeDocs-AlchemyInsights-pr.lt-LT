---
title: Sukeiskite savo klasikinę šakninę svetainę su modernia svetaine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741552"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Sukeiskite savo klasikinę šakninę svetainę su modernia svetaine

Jei jūsų aplinka buvo nustatyta iki 2019 m. balandžio mėn., galite pakeisti šakninę svetainę į modernią svetainę naudodami "Microsoft PowerShell":

- Jei turite kitą svetainę, kurią norite naudoti kaip savo šakninę svetainę, galite pakeisti [(apsikeitimo) šakninė svetainė](https://docs.microsoft.com/sharepoint/modern-root-site) su juo. 
    - Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pakeisti svetainės vietą su kita svetaine, o archyvuoti pradinę svetainę. Galima naudoti ir komandos svetainėje (neprijungtoje prie grupės), ir ryšių svetainėje. 

- Netrukus bus įvestos papildomos galimybės, kurios leis jums toliau naudoti svetainės turinį, bet konvertuoti esamą svetainę į ryšio svetainę. 
>[!Important]
>Šios galimybės bus diegiamos palaipsniui. Toliau patikrinkite, ar pranešimų centre nėra naujinimų. 

## <a name="known-issues-with-swapping-sites"></a>Žinomos problemos, susijusios su svetainių swapping

- Paskirties svetainė gali pateikti klaidos "nerasta" (HTTP 404) trumpą laiką.
- Norint atnaujinti ieškos indeksą, turinį reikės nuskaityti iš naujo. Nėra rankinio žingsnio reikia - tai bus daroma automatiškai.
- Viskas, kas priklauso nuo "statinių" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti ištaisyta rankiniu būdu.
- Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.Gaukite visų organizacinių naujienų svetainių sąrašą.
- Project Server svetainėse gali tekti patikrinti, siekiant užtikrinti, kad jie vis dar tinkamai susiję.
