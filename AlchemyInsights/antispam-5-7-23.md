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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506451"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>El. pašto pristatymo problemų sprendimas klaidos kodas 5.7.23

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintuve žiniatinklyje.

Patikrinkite, ar "Microsoft" nenustatė siunčiamo pranešimo kaip pašto šiukšlių ir nurodė per [didelės rizikos pristatymo telkinį](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Didelės rizikos pristatymo telkinio pranešimai neišlaikys SPF patikrinimų, todėl paskirties el. pašto organizacija jų nepriims.

Jei problema išlieka, gali tekti susisiekti su pašto pagrindinio kompiuterio, į kurį bandote siųsti el. laiškus, administratoriumi. Užsirašykite išsamią išorinę klaidą, pasiekiamą atmetimo pranešime. "Microsoft" palaikymo tarnyba gali negalėti toliau padėti.
