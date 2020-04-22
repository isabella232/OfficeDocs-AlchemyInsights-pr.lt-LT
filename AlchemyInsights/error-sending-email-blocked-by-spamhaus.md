---
title: Klaida siunčiant laišką užblokuotas SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714266"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Klaida siunčiant el. laišką: Kliento pagrindinis kompiuteris užblokuotas naudojant "Spamhaus"

IP adresas, kuris išsiuntė pranešimą, yra blokų sąraše, priklausančiame ["Spamhaus".](https://go.microsoft.com/fwlink/p/?linkid=123245) Nepageidaujamo e. Paštas yra užblokuotos paskyros, įkompromisiniai įrenginiai, bendrinami viešuoju IP adresu, ir interneto paslaugų teikėjo (ISP) strategijos. Galimi pataisymai yra:
  
- Užblokuotiems gaunamiems pranešimams, kuriuose valdote šaltinio el. pašto serverį, turite nustatyti priežastį ir pašalinti bloką iš "Spamhaus" svetainės.

- Užblokuotiems gaunamiems pranešimams, kuriuose šaltinio IP adresas priklauso kam nors kitam, adreso savininkas turi pašalinti bloką iš "Spamhaus" svetainės. Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitą statinį IP adresą arba pašalinti adresą iš PBL.

- Užblokuotų siunčiamų pranešimų iš domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei pranešimai nukreipiami per trečiosios šalies tarnybą. Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte užblokuotą IP adreso savininką.
