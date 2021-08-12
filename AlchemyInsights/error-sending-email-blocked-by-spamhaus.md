---
title: Klaida siunčiant el. laiškus, užblokuotus "SpamHaus"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946766"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Klaida siunčiant el. laišką: kliento pagrindinis kompiuteris užblokuotas naudojant "Spamhaus"

Pranešimą išsiuntęs IP adresas yra blokų sąraše, kuris priklauso ["Spamhaus".](https://go.microsoft.com/fwlink/p/?linkid=123245) "Spamhaus" blokavimo priežastys apima pažeistas paskyras, pažeistus įrenginius, kurie bendrina viešąjį IP adresą, ir interneto paslaugų teikėjo (ISP) strategijas. Galimi pataisymai:
  
- Užblokuotų gaunamų pranešimų, kuriuose valdote šaltinio el. pašto serverį, atveju turite nustatyti priežastį ir pašalinti bloką iš "Spamhaus" svetainės.

- Blokuojamų gaunamų pranešimų, kurių šaltinio IP adresas priklauso kam nors kitam, atveju adreso savininkas turi pašalinti bloką iš "Spamhaus" svetainės. Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitą statinį IP adresą arba pašalinti adresą iš PBL.

- Jei blokuojami siunčiami pranešimai iš jūsų domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei pranešimai nukreipiami per trečiosios šalies tarnybą. Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte užblokuotą IP adreso savininką.
