---
title: Norite pažymėti domeną arba el. pašto siuntėją saugiai?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286688"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Norite pažymėti domeną arba el. pašto siuntėją saugiai?

- Patikimų **siuntėjų sąrašų naudoti nerekomenduojama,** nes ji atveria jūsų organizacijai pašto šiukšlių, sukčiavimo apsimetant ir apsimetimo atakomis.
- Tačiau, jei yra verslo reikalavimas, rekomenduojame **naudoti pašto** **[Flow taisykles.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (patikrina, ar siuntimo domenas nėra apgaulių). **Pastaba:** nerekomenduojame valdyti klaidingų teigiamų rezultatų naudojant patikimų siuntėjų sąrašus, nes pašto šiukšlių filtravimo išimtys gali atidaryti jūsų organizaciją saugos atakoms. Jei jūsų vartotojas (-ai) gauna laiškus, netinkamai pažymėtus kaip pašto šiukšlės arba nepageidaujamas el. paštas, **[praneškite apie pranešimus ir failus "Microsoft".](https://protection.office.com/reportsubmission)**
- Seifas Reikėtų vengti "Outlook", leidžiamų siuntėjų sąrašo arba leidžiamo domeno sąrašo apsaugos nuo pašto šiukšlių strategijose, nes siuntėjai apeina visus pašto šiukšles, apsimetant ir siuntėjų autentifikavimą (SPF, DKIM, DMARC).  Šis metodas geriausiai naudojamas tik laikinajam testavimui.
- Tikrinimą, kad tam tikras el. pašto apeinamo apsaugos nuo brukalo įvertinimas gali būti atliktas tikrinant "X-Forefront-Antispam-Report" pranešimo antraštę (SFV:SFE, SFV:SKA, SFV:SKN), žr. **[Anti-spam message headers](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- "Microsoft" nori apsaugoti [klientus](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)pagal numatytuosius parametrus, todėl kai kurie nuomotojo perrašymai nėra taikomi kenkėjiškai programinei įrangai ir didelio patikimumo apsimetant. Šie perrašymai apima: o Leidžiamų siuntėjų sąrašus arba leidžiamų domenų sąrašus (apsaugos nuo pašto šiukšlių strategijas) o Outlook Seifas Siuntėjai o IP leistinas sąrašas (ryšio filtravimas) 
- Vienintelis perrašymo būdas, leidžiantis sukčiavimo apsimetant pranešimui apeiti filtravimą, yra Exchange pašto srauto taisyklės (dar vadinamos transportavimo taisyklėmis). Norėdami naudoti pašto srauto taisykles norėdami apeiti filtravimą, žr. Pašto srauto taisyklių naudojimas pašto šiukšlių patikimumo **[lygiui (SCL) laiškuose nustatyti.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**