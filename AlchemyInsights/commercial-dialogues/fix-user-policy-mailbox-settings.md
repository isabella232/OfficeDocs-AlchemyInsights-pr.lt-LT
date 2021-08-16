---
title: Vartotojo strategijos / pašto dėžutės parametrų taisymas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034726"
---
# <a name="fix-user-policymailbox-settings"></a>Vartotojo strategijos / pašto dėžutės parametrų taisymas

Pašto dėžutės nepageidaujamo pašto parametrai paveikė šį pranešimą. Norėdami peržiūrėti parametrus, atlikite šiuos veiksmus:

1. Paleiskite Exchange valdymo aplinką. Daugiau informacijos žr. [Valdymo aplinkos Exchange atidarymas.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Vykdykite šią komandą (naudodami vartotojo el. pašto adresą):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Patikrinkite, ar siuntėjo el. pašto adresas priklauso **"TrustedSendersAndDomains"** arba **"BlockedSendersAndDomains".** Jei el. pašto adresas yra viename iš sąrašų, gali tekti jį pašalinti. Norėdami sužinoti daugiau, [žr. Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
