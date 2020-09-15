---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717333"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Klaidos kodo 5.7.23. pašto pristatymo problemų sprendimas

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamame SPF arba DNS įrašų tikrintuve žiniatinklyje.

Patikrinkite, ar siuntimo laiškas nebuvo identifikuojamas kaip šlamštas "Microsoft" ir nukreipiamas per [didelės rizikos pristatymo telkinį](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Didelės rizikos pristatymo telkinio laiškai nepereis SPF, todėl nebus priimami paskirties el. pašto organizacija.

Jei problema kartojasi, jums gali tekti kreiptis į pašto pagrindinio kompiuterio, kuriam bandote siųsti laišką, administratorių. Užsirašykite išsamią išorinę klaidą, esančią peradresavimo pranešime. "Microsoft" palaikymo tarnyba gali būti nepajėgi toliau padėti.
