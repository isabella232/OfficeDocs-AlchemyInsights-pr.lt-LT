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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792140"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Norite pažymėti domeną arba el. pašto siuntėją saugiai?

- Patikimų **siuntėjų sąrašų naudoti nerekomenduojama,** nes ji atveria jūsų organizacijai pašto šiukšlių, sukčiavimo apsimetant ir apsimetimo atakomis.
- Tačiau, jei yra verslo reikalavimas, rekomenduojame **šiam atvejui** **[naudoti pašto](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** srauto taisykles. Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (patikrina, ar siuntimo domenas nėra apgaulių). **Pastaba:** nerekomenduojame valdyti klaidingų teigiamų rezultatų naudojant patikimų siuntėjų sąrašus, nes pašto šiukšlių filtravimo išimtys gali atidaryti jūsų organizaciją saugos atakoms. Jei jūsų vartotojas (-ai) gauna laiškus, netinkamai pažymėtus kaip pašto šiukšlės arba nepageidaujamas el. paštas, **[praneškite apie pranešimus ir failus "Microsoft".](https://protection.office.com/reportsubmission)**
- Patikimų siuntėjų programoje "Outlook", Leidžiamų siuntėjų sąraše  arba leidžiamų domenų sąraše apsaugos nuo pašto šiukšlių strategijose reikėtų vengti, nes siuntėjai apeina visus pašto šiukšles, apsimetimo apsimetant ir siuntėjų autentifikavimą (SPF, DKIM, DMARC). Šis metodas geriausiai naudojamas tik laikinajam testavimui.
