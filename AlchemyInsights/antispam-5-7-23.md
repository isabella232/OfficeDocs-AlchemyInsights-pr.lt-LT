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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821419"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>El. pašto pristatymo problemų sprendimas dėl klaidos kodo 5.7.23

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintoją žiniatinklyje.

Patikrinkite, ar "Microsoft" neįvardifikuoja siunčiamo pranešimo kaip pašto šiukšlių ir nukreipiamas per [didelės rizikos pristatymo telkinį.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Pranešimai didelės rizikos pristatymo telkinyje neišduos SPF patikrų, todėl paskirties el. pašto organizacija jų nepriims.

Jei problema išlieka, gali tekti kreiptis į pašto pagrindinio kompiuterio, į kurį bandote siųsti el. paštą, administratorių. Atkreipkite dėmesį į išsamią išorinę klaidą, galimų atmetimo pranešime. "Microsoft" palaikymas gali nepadėti toliau.
