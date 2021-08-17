---
title: Nepavyksta siųsti / gauti el. laiškų į /iš Office 365 dėl TLS 1.0 ir TLS 1.1 išjungimo
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054914"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nepavyksta siųsti / gauti el. laiškų į /iš Office 365 dėl TLS 1.0 ir TLS 1.1 išjungimo

Kaip patvirtino pranešimų centro pranešimas MC229914, TLS 1.0 ir TLS 1.1, "Exchange Online" pašto srauto galinių punktų naikinimas. Netrukus Office 365 tls 1.0 ir TLS 1.1 el. pašto ryšių iš išorinių šaltinių. Be to, Exchange Online niekada nenaudos TLS 1.0 arba 1.1 siunčiamų el. laiškų. Jei susiduriate su problemomis dėl TLS 1.0 arba 1.1 išjungimo, galite pastebėti vieną iš šių klaidų:

- Siuntėjas gauna NDR atmetimą atgal – "421 4.4.2 Ryšys numestas dėl SocketError"
- Vietinio serverio, siunčiančio el. laiškus 365– "421 4.4.2 Connection dropped due to SocketError", eilės peržiūros programos klaida
- Klaida siuntimo jungties [protokolo žurnale](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveryje, siunčiantį el. Office 365– TLS derybos nepavyko dėl klaidos SocketError
- Klaida siuntimo arba gavimo jungties protokolo žurnale – "451 5.7.3 Pirmiausia turi būti išsiųsta KOMANDA STARTTLS"

Jei kyla kuri nors iš anksčiau nurodytų klaidų, įsitikinkite, kad serveryje, kuris siunčia arba gauna el. laiškus, įgalintas TLS 1.2 tikrinant šiuos registro raktus–

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Jei pakeisite anksčiau nurodytus registro raktus, kad įgalintumėte TLS 1.2, iš naujo paleiskite serverį, kad pakeitimai įsigaliotų. Taip pat įsitikinkite, kad turite naujausius Windows Exchange naujinimus.

Daugiau informacijos rasite:

- [Exchange Server TLS rekomendacijos, 1 dalis: Pasiruošimas TLS 1.2 – "Microsoft Tech Community"](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS rekomendacijų 2 dalis: TLS 1.2 įgalinimas ir klientų, kurie jos nenaudoja, nustatymas – "Microsoft Tech Community"](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [El. pašto scenarijų supratimas, jei NEGALIMA susitarti dėl TLS versijų su "Exchange Online " – "Microsoft Tech Community"](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
