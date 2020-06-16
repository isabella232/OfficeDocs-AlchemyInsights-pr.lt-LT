---
title: tas pats kaip failo vardas yra geriausias
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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750978"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Reikalinga Alchemija Antraštė H1, H2's neveikia."
Geriausia praktika ir gairės Alchemija kūrimo:

1. **Negalima įdėti Alchemijos įžvalgos aplankuose**- tai bus pertrauka URL struktūrą. Mes ieškome, kaip tai ištaisyti.
1. Aplanke **AlchemyInsights** esantys failai turi turėti mažąsias failų vardus su brūkšneliais tarpams. ***"how-to-enable-litigation-hold".***
    1. Įtraukite taisyklės ID arba ieškos id iš [Alchemijos partnerių portalo](https://alchemyportal.azurewebsites.net) į lauką ms.custom. Ex. ***ms.custom: 100021 ms.custom: 100021 ms.custom: 100021***
1. Naudokite likusius metaduomenis šio failo viršuje kaip šabloną.
1. ["Alchemy" partnerių portale](https://alchemyportal.azurewebsites.net)eikite į skyrių **Klientų įžvalgos pavadinimas:** ir naudokite tai kaip atspirties tašką savo H1 pavadinimui įžvalgai. 
    > [!NOTE]
    > Alchemija Įžvalgos turi turėti tik vieną H1 viršuje arba jie bus pertrauka gamybos. H2s netampa nei taip naudoti **paryškinti** ar kitų konvencijų reikšti atskiras sekcijas.
1. Tada užpildykite pagrindinį tekstą naudodami medžiagos juodraštį, esantį puslapio Alchemijos taisyklė skyriuje Klientų įžvalgos
    1. Sąrašai su ženkleliais yra gerai
    1. Taip pat sunumeruoti sąrašai
    1. **Paryškintasis** ir *pasvirasis* yra a-ok
    1. Nuorodos visada turėtų būti **arba "nuorodos į interneto" / išorės** arba **gilias nuorodas į UI elementai, o**ne vidaus nuorodos.
    1. Šiuo metu nuotraukos nėra oficialiai palaikomos, tačiau jos yra veiksmų plane.

Ir tai tikrai jau šiek tiek per ilgas. Geriausia praktika yra apie 400 simbolių ---------------------------------

Kai jūsų turinys bus paruoštas, traukite jį į gyvą šaką. Tada eikite į [Alchemijos partnerių portalą](https://alchemyportal.azurewebsites.net) ir įveskite failo vardą į url lauką. 