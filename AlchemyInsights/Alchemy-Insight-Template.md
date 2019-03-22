---
title: pats, kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742430"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Reikia Alchemy antraštės H1, H2, neveikia.
Geriausia praktika ir rengti gaires Alchemija kūrimo:

1. **Neįdėtas Alchemija įžvalgos aplankuose**- tai nutrauks url struktūrą. Mes ieškome į tvirtinimo tai.
1. Failus į aplanką **AlchemyInsights** turėtų būti mažoji raidė failų vardai su brūkšneliais erdves ex. ***pažangiąja-į-įgalinti--sulaikymas***.
    1. Įtraukti taisyklė ID arba kibiras ID [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ms.custom srityje. ex. ***ms.Custom: 100021***
1. Naudoti metaduomenų likusioje šio failo viršuje jūsų šabloną.
1. [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net)naršyti žemyn į skiltį **klientų supratimą pavadinimas:** ir naudoti, kad pradžios taškas H1 pavadinimo už supratimą. 
    > [!NOTE]
    > Alchemija tendencijos turi turėti tik vieną H1 į viršų arba jie bus pertrauka gamybos. H2s ne padaryti tiek naudoti **paryškinti** arba kitomis konvencijomis reiškia atskiruose skyriuose.
1. Be to, užpildykite naudojant projekto medžiagą įžvalgų apie klientą dalyje Alchemija taisyklė puslapio tekste
    1. Sąrašai su ženkleliais yra gerai
    1. Numeruotas sąrašas per
    1. **Drąsiai** ir *kursyvas* yra OK-
    1. Nuorodas visada turi būti arba **"nuorodos ä¯ interneto" / užsienio** arba **giliai nuorodos į vartotojo sąsajos elementai**, ne vidaus ryšius.
    1. Nuotraukos nėra oficialiai palaikoma šiuo metu, bet tai dėl plano.

Ir tai tikrai jau yra šiek tiek per ilgas. Geriausia praktika yra apie 400 simbolių---

Kai jūsų turinys yra pasirengusi, traukti į gyvos apatinės šakos. Tada eikite į [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ir url lauke įveskite failo vardą. M