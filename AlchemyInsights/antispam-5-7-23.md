---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932177"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>El. pašto pristatymo problemų sprendimas dėl klaidos kodo 5.7.23

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintoją žiniatinklyje.

Patikrinkite, ar "Microsoft" neįvardifikuoja siunčiamo pranešimo kaip pašto šiukšlių ir nukreipiamas per [didelės rizikos pristatymo telkinį.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Pranešimai didelės rizikos pristatymo telkinyje neišduos SPF patikrų, todėl paskirties el. pašto organizacija jų nepriims.

Jei problema išlieka, gali tekti kreiptis į pašto pagrindinio kompiuterio, į kurį bandote siųsti el. paštą, administratorių. Atkreipkite dėmesį į išsamią išorinę klaidą, galimų atmetimo pranešime. "Microsoft" palaikymas gali nepadėti toliau.
