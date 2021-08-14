---
title: Geriausios praktikos naudojimas išplėstinėms medžioklės užklausoms
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930141"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Geriausios praktikos naudojimas išplėstinėms medžioklės užklausoms

Norėdami greičiau gauti rezultatus ir išvengti skirtasis laikas vykdant sudėtingas užklausas, taikykite šias geriausias praktikas:

- Bandydami naujas užklausas visada naudokite limitą, kad išvengtumėte labai didelių rezultatų rinkinių. Taip pat `count` naudokite norėdami atlikti pradinį rezultatų rinkinio dydžio įvertinimą.
- Pirmiausia naudokite laiko filtrus. Geriausia apriboti užklausas iki septynių dienų.
- Užklausos pradžioje, iš karto po laiko filtro, įtraukite filtrus, kurie turėtų pašalinti daugumą duomenų.
- Ieškodami visų atpažinimo ženklų, naudokite operatorių, `has` o ne `contains` .
- Vykdyti iešką konkrečiame stulpelyje, o ne visuose stulpeliuose.
- Kai jungiate lenteles, pirmiausia nurodykite lentelę su mažiau eilučių.
- `project` tik reikiamus stulpelius iš lentelių, prie kurių prisijungėte.

Norėdami sužinoti daugiau, žr. [Išplėstinės medžioklės užklausų geriausios praktikos](https://go.microsoft.com/fwlink/?linkid=2144812).
