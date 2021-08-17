---
title: tas pats, kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312833"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Būtinas "Alchemy Header H1", H2 neveikia."
"Alchemy" kūrimo geriausios praktikos ir gairės:

1. **Nedėskite "Alchemy Įžvalgos aplankuose**– tai sulaužys URL struktūrą. Norime išspręsti šią problemą.
1. Failų aplanke **AlchemyInsights** turi būti mažųjų failų pavadinimų su tarpų brūkšneliais ex. **_how-to-enable-litigation-hold_**.
    1. Įtraukite taisyklės ID arba talpyklos ID iš ["Alchemy" partnerių portalo](https://alchemyportal.azurewebsites.net) į lauką ms.custom. ex. ***ms.custom: 100021***
1. Kaip šabloną naudokite likusius šio failo viršuje rodomus metaduomenis.
1. ["Alchemy" partnerių portale](https://alchemyportal.azurewebsites.net)eikite į skyrių Klientų įžvalgų **pavadinimas:** ir naudokite jį kaip H1 pavadinimo pradžios tašką įžvalgai. 

**Pastaba:** Alchemija Įžvalgos turi turėti tik vieną H1 viršuje arba jie sulaužys gamybą. H2s ne atvaizduoja taip, kad **atskiros** sekcijos būtų vadinamos paryškintuoju šriftu arba kitomis konvencijomis.
1. Tada užpildykite tekstą naudodami juodraščio medžiagą puslapio "Alchemy"Customer Insights" sekcijoje
    1. Sąrašai su ženkleliais yra puikūs
    1. Numeruoti sąrašai taip pat
    1. **Paryškintasis** *ir pasvirasis* yra gerai
    1. Saitai visada turi būti **"saitai į žiniatinklį" /** išoriniai ARBA giluminiai **saitai su vartotojo sąsajos elementais, o** ne vidiniais saitais.
    1. Šiuo metu paveikslėliai oficialiai nepalaikomi, tačiau jie pateikiami veiksmų plane.

Ir tai tikrai jau šiek tiek per ilgas. Geriausia praktika yra apie 400 simbolių ---------------------------------

Kai turinys bus paruoštas, patraukite jį į tiesioginę šaką. Tada eikite į ["Alchemy" partnerių portalą](https://alchemyportal.azurewebsites.net) ir įveskite failo vardą į url lauką. 