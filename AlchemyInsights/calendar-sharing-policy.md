---
title: 618 Kalendoriaus bendrinimo strategija
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373007"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Strategijos klaida bendrinant kalendorių

1. Atlikite vieną iš šių veiksmų, atsižvelgdami į savo situaciją:
    - Prisijunkite prie "Exchange Online" naudodami nuotolinę "PowerShell". Daugiau informacijos [ieškokite Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Vietiniame serveryje atidarykite "Exchange" valdymo aplinką.
2. Nustatykite vartotojui priskirtą bendrinimo strategiją. Norėdami tai padaryti, vykdykite šią komandą ir atkreipkite dėmesį, kad strategija grįžo:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atnaujinkite vartotojo bendrinimo strategiją. Jei norite tai padaryti, atlikite tokius veiksmus:
    - Atidarykite "Exchange" administravimo centrą.
    - Spustelėkite **Organizacija**, tada dukart spustelėkite strategiją, priskirtą vartotojui dalyje **Individualus bendrinimas**. Tai politika, kuri buvo grąžinta 2 veiksme.
    - Puslapyje Bendrinimo taisyklė pasirinkite kalendoriaus bendrinimo lygį, kurį norite leisti dalyje **Nurodykite, kokią informaciją norite bendrinti;** spustelėkite **Įrašyti**.

Daugiau informacijos rasite: ["Strategija neleidžia suteikti teises šiame lygyje vienam ar daugiau gavėjo (-ų)" klaida, kai vartotojas bando bendrinti kalendorių](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
