---
title: Nustatyti išorinės pašto persiuntimo pašto dėžučių audito žurnaluose
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417219"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Nustatyti sukonfigūravus pašto dėžutės išorinio el. pašto peradresavimas

Kai vartotojas konfigūruoja išorės el. laiškų peradresavimas į pašto dėžutę, veiklos auditą kaip į **Set-Mailbox** cmdlet. Jūs galite pamatyti veiklos audito žurnalo paieškos naudojimas – saugos & atitikties užtikrinimo centre.

1. Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/)

2. Spustelėkite **paieškos ir tyrimas** ir pasirinkite **Audito žurnalo paieška**.

3. Pasirinkite datos intervalą laukuose **pradžios data** ir **pabaigos data** . Jums nereikia nurodyti vartotojo vardą. Patikrinkite, ar **veiklos** laukas yra nustatytas **Rodyti visą veiklą, rezultatus**.

4. Spustelėkite **Ieškoti**.

Rezultatuose spustelėkite **Filtruoti rezultatus** ir veiklos filtras lauke įveskite **Set-Mailbox** . Pasirinkite įrašą audito rezultatus. **Detalių** išskleidžiamojo meniu spustelėkite **daugiau informacijos**. Jūs turite žiūrėti į išsamią informaciją apie kiekvieno audito įrašas nustatyti, jeigu veikla yra susijusi su el. pašto persiuntimas.

- **ObjectId**: pseudonimas vertės pašto dėžutę, kuri buvo modifikuota.

- **Parametrai**: _ForwardingSmtpAddress_ rodo, tikslinių el. pašto adresą.

- **Vartotojo ID**: vartotojo, kuris sukonfigūruotas el. pašto peradresavimas **ObjectId** srities pašto dėžutės.

Norėdami gauti daugiau informacijos, peržiūrėkite [renkant, kuris sukūrė el. pašto peradresavimo pašto dėžutės](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
