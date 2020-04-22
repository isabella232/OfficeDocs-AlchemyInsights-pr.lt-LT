---
title: tas pats, kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676541"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Reikalinga Alchemija Antraštė H1, H2 neveikia.
Geriausia praktika ir gairės Alchemija kūrimo:

1. **Neįkandykite Alchemijos įžvalgų aplankuose**- tai sulaužys URL struktūrą. Mes ieškome tai sutaisydami.
1. **Aplanke AlchemyInsights** esantys failai turi turėti mažąsias failų pavadinimus su brūkšneliais tarpams ex. ***"how-to-enable-litigation-hold".***
    1. Įtraukite taisyklės ID arba segmento ID iš [alchemijos partnerių portalo](https://alchemyportal.azurewebsites.net) į ms.custom lauką. Ex. ***ms.custom: 100021 ms.custom: 100021 ms.custom: 100021 ms.***
1. Kaip šabloną naudokite likusius metaduomenis šio failo viršuje.
1. ["Alchemy" partnerių portale](https://alchemyportal.azurewebsites.net)eikite į skyrių **"Kliento įžvalgos pavadinimas"** ir naudokite jį kaip "H1" pavadinimo pradžios tašką įžvalgoms. 
    > [!NOTE]
    > Alchemija Įžvalgos turi turėti tik vieną H1 viršuje arba jie bus pertrauka gamybos. H2s nepateikia nei **paryškintų,** nei kitų konvencijų, kad būtų galima nurodyti atskiras sekcijas.
1. Tada užpildykite pagrindinį tekstą naudodami medžiagos juodraštį puslapio "Alchemy Rule" sekcijoje Klientų įžvalgos
    1. Sąrašai su ženkleliais yra puikūs
    1. Numeruoti sąrašai taip pat
    1. **Paryškintas** ir *pasvirasis* yra ok
    1. Nuorodos visada turėtų būti **arba "nuorodos į interneto" / išorės** arba giliai nuorodos į ui **elementus,** o ne vidaus nuorodos.
    1. Šiuo metu nuotraukos oficialiai nepalaikomos, bet jos yra veiksmų plane.

Ir tai tikrai jau šiek tiek per ilgai. Geriausia praktika yra apie 400 simbolių ---------------------------------

Kai jūsų turinys bus paruoštas, traukite jį į tiesioginę šaką. Tada eikite į [Alchemija partnerių portalas](https://alchemyportal.azurewebsites.net) ir įveskite failo vardą į URL lauką. 