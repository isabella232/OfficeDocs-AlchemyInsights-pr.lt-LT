---
title: Nustatyti išorinės pašto persiuntimo pašto dėžučių audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539109"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Nustatyti sukonfigūravus pašto dėžutės išorinio el. pašto peradresavimas

Kai "Office 365" vartotojas konfigūruoja išorės el. laiškų peradresavimas į pašto dėžutę, veiklos auditą kaip į **Set-Mailbox** cmdlet. Jūs galite pamatyti veiklos audito žurnalo paieškos naudojimas – saugos & atitikties užtikrinimo centre.

1. Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/).

2. Grįžti į **paieškos** > **audito žurnalo paieškos** puslapyje.

3. Pasirinkite datos intervalą laukuose **pradžios data** ir **pabaigos data** . Jums nereikia nurodyti vartotojo vardą. Patikrinkite, ar **veiklos** laukas yra nustatytas **Rodyti visą veiklą, rezultatus**.

4. Spustelėkite **Ieškoti**.

Rezultatuose spustelėkite **Filtruoti rezultatus** ir veiklos filtras lauke įveskite **Set-Mailbox** . Pasirinkite įrašą audito rezultatus. **Detalių** išskleidžiamojo meniu spustelėkite **daugiau informacijos**. Jūs turite žiūrėti į išsamią informaciją apie kiekvieno audito įrašas nustatyti, jeigu veikla yra susijusi su el. pašto persiuntimas.

- **ObjectId**: pseudonimas vertės pašto dėžutę, kuri buvo modifikuota.

- **Parametrai**: _ForwardingSmtpAddress_ rodo, tikslinių el. pašto adresą.

- **Vartotojo ID**: vartotojo, kuris sukonfigūruotas el. pašto peradresavimas **ObjectId** srities pašto dėžutės.

Norėdami gauti daugiau informacijos, peržiūrėkite [renkant, kuris sukūrė el. pašto peradresavimo pašto dėžutės](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
