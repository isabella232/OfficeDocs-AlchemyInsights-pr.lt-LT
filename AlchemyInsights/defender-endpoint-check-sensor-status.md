---
title: Sargybos pabaigos taško tikrinimo jutiklio būsena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676343"
---
# <a name="defender-endpoint-check-sensor-status"></a>Sargybos pabaigos taško tikrinimo jutiklio būsena

Plytelė **Įrenginiai su jutiklio** problemomis yra saugos operacijų ataskaitų srityje. Šioje plytelėje pateikiama informacija apie atskiro įrenginio galimybę pateikti jutiklio duomenis ir bendrauti su galinio punkto tarnybos sargyba. Ji praneša, kiek įrenginių reikia atkreipti dėmesį ir padeda nustatyti probleminius įrenginius ir imtis veiksmų, kad būtų išsekusi žinomos problemos.

Du plytelės būsenos indikatoriai pateikia informaciją apie įrenginių, kurie netinkamai praneša tarnybai, skaičių:

- **Netinkamai sukonfigūruota** Įrenginiai, kurie gali iš dalies pranešti jutiklio duomenis galinio punkto tarnybos sargybai ir gali turėti konfigūracijos klaidų, kurias reikia ištaisyti.
- **Neaktyvus** Įrenginiai, kurie nustojo teikti ataskaitas galinio punkto tarnybos sargybai daugiau nei septynias dienas per pastarąjį mėnesį.

Spustelėjus bet kurią iš grupių, nukreipiama į sąrašą Įrenginiai, filtruojamas pagal jūsų pasirinkimus. Sąraše Įrenginiai galite filtruoti sveikatos būsenų sąrašą pagal šią būseną:

- **Aktyvus** Įrenginiai, kurie aktyviai praneša pabaigos taško tarnybos sargybai.
- **Netinkamai sukonfigūruota** Įrenginiai, kurie gali iš dalies pranešti jutiklio duomenis galinio punkto tarnybos sargybai, tačiau turi konfigūracijos klaidų, kurias reikia ištaisyti. Netinkamai sukonfigūruotuose įrenginiuose gali būti viena iš šių problemų arba jų derinys:

    - Nėra jutiklio duomenų – įrenginiai nustojo siųsti jutiklio duomenis. Iš įrenginio gali būti paleidžiami riboti įspėjimai.
    - Sutrikę ryšiai – galimybė bendrauti su įrenginiu yra sutrikusi. Failų siuntimas giliai analizei, failų blokavimas, įrenginio izoliavimas nuo tinklo ir kiti veiksmai, kuriems reikia ryšio su įrenginiu, gali neveikti.
- **Neaktyvus** Įrenginiai, kurie nustojo teikti ataskaitas galinių punktų tarnybos sargybai.

Galite atsisiųsti visą sąrašą CSV formatu naudodami eksportavimo funkciją.

Daugiau informacijos žr. Jutiklio [sveikatos būsenos tikrinimas "Microsoft" sargybos galinį punktą](/microsoft-365/security/defender-endpoint/check-sensor-status).

Daugiau informacijos apie tai, dėl ko įrenginys buvo neaktyvus arba netinkamai sukonfigūruotas, žr. Nesveikų jutiklių taisymas ["Microsoft Defender", skirtame galinių punktų .](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
