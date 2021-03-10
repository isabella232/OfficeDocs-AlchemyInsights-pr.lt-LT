---
title: Geriausios išplėstinės medžioklės užklausų praktikos taikymas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696077"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Geriausios išplėstinės medžioklės užklausų praktikos taikymas

Norėdami greičiau gauti rezultatus ir išvengti skirtojo laiko vykdydami sudėtingas užklausas, taikykite šias geriausias praktikas:

- Bandant naujas užklausas, visada naudokite apribojimą, kad būtų išvengta itin didelės rezultatų rinkinių. Taip pat naudokite `count` Norėdami atlikti pradinį rezultatų rinkinio dydžio vertinimą.
- Pirmiausia naudokite laiko filtrus. Idealiu atveju Apribokite savo užklausas iki septynių dienų.
- Užklausos pradžioje, iškart po laiko filtro, įtraukite filtrus, kuriuos tikimasi pašalinti didžiąją dalį duomenų.
- Ieškodami visiškai žetonų naudokite `has` operatorių, o ne `contains` .
- Vykdykite iešką konkrečiame stulpelyje, o ne visuose stulpeliuose.
- Kai sujungiame lenteles, pirmiausia apibrėžkite lentelę, kurioje yra mažiau eilučių.
- `project` tik reikiamus stulpelius iš lentelių, kurias sujungėte.

Norėdami sužinoti daugiau, peržiūrėkite [pažangiausių medžioklės užklausų geriausios praktikos](https://go.microsoft.com/fwlink/?linkid=2144812).
