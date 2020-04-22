---
title: Nustatyti išorinį el. pašto peradresavimą pašto dėžutėse audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716468"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Nustatyti, kada išorinių el. laiškų peradresavimas sukonfigūruotas pašto dėžutėse

Kai "Microsoft 365" vartotojas konfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla audituojama kaip **Set-Mailbox** cmdlet dalis. Veiklą galite peržiūrėti naudodami audito žurnalo iešką saugos & atitikties centre.

1. Prisijunkite prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).

2. Eikite į **ieškos** > **tikrinimo žurnalo ieškos** puslapį.

3. Laukuose **Pradžios data** ir **Pabaigos data** pasirinkite dienų seką. Nebūtina nurodyti naudotojo vardo. Patikrinkite, ar laukas **Veiklos** nustatyta rodyti **visų veiklų rezultatus.**

4. Spustelėkite **Ieškoti**.

Rezultatuose spustelėkite **Filtruoti rezultatus** ir veiklos filtro lauke įveskite **Set-Mailbox.** Rezultatuose pasirinkite audito įrašą. Iškeliamame pranešime **Išsami informacija** spustelėkite **Daugiau informacijos**. Turite peržiūrėti kiekvieno audito įrašo informaciją, kad nustatytumėte, ar veikla susijusi su el. pašto peradresavimu.

- **ObjectId**: Modifikuotos pašto dėžutės pseudonimo reikšmė.

- **Parametrai**: _ForwardingSmtpAddress_ nurodo paskirties el. pašto adresą.

- **UserId**: Vartotojas, kuris sukonfigūravo el. pašto peradresavimą pašto dėžutės **objectid** lauke.

Daugiau informacijos [ieškokite Nustatymas, kas nustato pašto dėžutės el. pašto peradresavimą](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
