---
title: Apsaugos nuo brukalo - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676505"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>El. pašto pristatymo problemų sprendimas klaidos kodas 5.7.23

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintuve žiniatinklyje.

Patikrinkite, ar "Microsoft" nenustatė siunčiamo pranešimo kaip pašto šiukšlių ir nurodė per [didelės rizikos pristatymo telkinį](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Didelės rizikos pristatymo telkinio pranešimai neišlaikys SPF patikrinimų, todėl paskirties el. pašto organizacija jų nepriims.

Jei problema išlieka, gali tekti susisiekti su pašto pagrindinio kompiuterio, į kurį bandote siųsti el. laiškus, administratoriumi. Užsirašykite išsamią išorinę klaidą, pasiekiamą atmetimo pranešime. "Microsoft" palaikymo tarnyba gali negalėti toliau padėti.
