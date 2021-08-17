---
title: 618 Kalendoriaus bendrinimo strategija
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091611"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Strategijos klaida bendrinant kalendorių

1. Atlikite vieną iš šių veiksmų, atsižvelgiant į jūsų situaciją:
    - Prisijungimas Exchange Online naudodami nuotolinę "PowerShell". Daugiau informacijos žr. ["Prisijungimas" Exchange Online "Remote PowerShell" naudojimas.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Vietiniame serveryje atidarykite "Exchange aplinką.
2. Nustatykite vartotojui priskirtą bendrinimo strategiją. Norėdami tai padaryti, vykdykite šią komandą ir atkreipkite dėmesį į grąžintas strategijas:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atnaujinkite vartotojo bendrinimo strategiją. Jei norite tai padaryti, atlikite tokius veiksmus:
    - Atidarykite Exchange administravimo centrą.
    - Spustelėkite **Organizacija**, tada dukart spustelėkite strategiją, kuri priskirta vartotojui dalyje Atskiras **bendrinimas.** Tai strategija, kuri buvo grąžinta 2 veiksme.
    - Puslapyje Bendrinimo taisyklė pasirinkite kalendoriaus bendrinimo lygį, kurį norite leisti dalyje **Nurodykite, kokią informaciją norite bendrinti;** spustelėkite **Įrašyti**.

Daugiau informacijos žr.: "Strategija neleidžia suteikti teisių šiam lygiui vienam ar keliems gavėjui [(-ams)",](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)kai vartotojas bando bendrinti kalendorių .
