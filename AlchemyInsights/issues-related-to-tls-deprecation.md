---
title: Nepavyksta siųsti/gauti el. laiško į/iš "Office 365", nes TLS 1,0 ir TLS 1,1 neįgalūs
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747123"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nepavyksta siųsti/gauti el. laiško į/iš "Office 365", nes TLS 1,0 ir TLS 1,1 neįgalūs

Kaip patvirtino pranešimų centro pašto MC229914, TLS 1,0 ir TLS 1,1 nuteistųjų pradėjo vykdyti "Exchange Online" pašto srauto pabaigos taškus. Netrukus "Office 365" nebepriims TLS 1,0 ir TLS 1,1 elektroninio pašto ryšių iš išorinių šaltinių. Be to, "Exchange Online" niekada nenaudos TLS 1,0 arba 1,1 siųsti siunčiamus laiškus. Jei susiduriate su problemomis dėl TLS 1,0 arba 1,1 negalios, galite susidurti su viena iš šių klaidų –

- Siuntėjas gauna NDR Bounce atgal – "421 4.4.2" sujungimas dėl "SocketError"
- Klaida, esanti vietinio serverio, kuris siunčia laišką į pareigūno 365 – "421 4.4.2" jungtį, dėl "SocketError", eilėje.
- Klaida siunčiant jungties [protokolo prisijungimo](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveryje laišką siunčiant į "Office 365" – TLS derybos nepavyko dėl klaidos SocketError
- Klaida siuntimo arba gavimo jungties protokolo logaritme – "451" 5.7.3 turi būti pirmoji "STARTTLS" komanda.

Jei susiduriate su bet kuria iš aukščiau nurodytų klaidų, įsitikinkite, kad serveryje, kuris siunčia arba gauna laišką, TLS 1,2 įjungėte patikrindami šiuos registro raktus –

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klientas] **"DisabledByDefault" = DWORD: 00000000 "= DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ serveris] **" DisabledByDefault "= DWORD: 00000000" įjungtas "= DWORD: 00000001**

Jei pakeisite anksčiau nurodytus registro raktus, Norėdami įgalinti TLS 1,2, iš naujo paleiskite serverį, kad įsigaliotų pakeitimai. Taip pat įsitikinkite, kad įdiegėte naujausius "Windows" ir "Exchange" naujinimus.

Daugiau informacijos rasite:

- ["Exchange Server" TLS nuorodos, 1 dalyje: Pasiruošimas TLS 1,2-"Microsoft" technologijų bendruomenė](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- ["Exchange Server" TLS rekomendacijų 2 dalyje: TLS 1,2 ir klientų tapatybės nustatymas nenaudojant IT – "Microsoft" technologijų bendruomenė](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [El. pašto scenarijų supratimas, jei negalima susitarti dėl TLS versijų naudojant "Exchange Online" – "Microsoft" technologijų bendruomenė](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
