---
title: Norite, kad domenas arba pašto siuntėjas būtų saugūs?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803253"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Norite, kad domenas arba pašto siuntėjas būtų saugūs?

- **Saugių siuntėjų sąrašų naudojimas nerekomenduojamas** , nes jis atveria jūsų organizacijai pašto šiukšlių, apsimetimo ir imitavimo atakų.
- Tačiau, jei yra verslo reikalavimas, **rekomenduojame** naudoti " **[mail Flow" taisykles](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (tikrina, ar siuntimo domenas nėra apsimetimo). **Pastaba**: nerekomenduojame naudoti neteisingus teigiamus rezultatus naudojant patikimų siuntėjų sąrašus, nes išimtys pašto šiukšlių filtrui gali atidaryti jūsų organizaciją į saugos atakas. Jei jūsų vartotojas (-iai) gauna laiškus, netinkamai pažymėtus kaip pašto šiukšles arba nepageidaujamą paštą, praneškite **[apie laiškus ir failus "Microsoft"](https://protection.office.com/reportsubmission)**.
- **Reikia vengti** patikimų siuntėjų programoje "Outlook", leidžiančio siuntėjų sąrašo arba leidžiamo domenų sąrašo apsaugos nuo pašto šiukšlių politikoje, nes siuntėjai apeina visus pašto šiukšlių, apgaulingas ir pašto apsaugos bei siuntėjo autentifikavimo (SPF, DKIM, DMARC). Šis metodas geriausiai tinka tik laikiniesiems bandymams.
