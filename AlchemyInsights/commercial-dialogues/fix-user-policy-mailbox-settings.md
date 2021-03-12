---
title: Vartotojų strategijos/pašto dėžutės parametrų taisymas
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750556"
---
# <a name="fix-user-policymailbox-settings"></a>Vartotojų strategijos/pašto dėžutės parametrų taisymas

Pašto dėžutės nepageidaujamo pašto parametrai paveikė šį pranešimą. Norėdami peržiūrėti parametrus, atlikite šiuos veiksmus:

1. "Exchange Management Shell" Paleistis. Daugiau informacijos ieškokite " [Exchange" valdymo aplinkos atidarymas](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Vykdykite šią komandą (naudodami vartotojo elektroninio pašto adresą):  **get-mailboxjunkmailconfiguration-tapatybė "user@domain.com"**
3. Patikrinkite, ar siuntėjo elektroninio pašto adresas priklauso **TrustedSendersAndDomains** arba **Blockedsendersanddomains**. Jei el. pašto adresas yra viename iš sąrašų, gali tekti jį pašalinti. Norėdami sužinoti daugiau, žiūrėkite [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
