---
title: 618 kalendoriaus naudojimo strategija
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684238"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Strategijos klaida, kai dalijamasi su kalendoriumi

1. Atsižvelgdami į situaciją atlikite vieną iš šių veiksmų:
    - Prisijungimas prie "Exchange Online" naudojant nuotolinį "PowerShell". Daugiau informacijos ieškokite [prisijungimas prie "Exchange Online" naudojant nuotolinę "PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)".
    - Vietiniame serveryje atidarykite "Exchange" valdymo aplinką.
2. Nustatykite vartotojui priskirtą bendro naudojimo strategiją. Norėdami tai padaryti, vykdykite šią komandą ir užsirašykite strategiją:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atnaujinkite vartotojo bendro naudojimo strategiją. Jei norite tai padaryti, atlikite tokius veiksmus:
    - Atidarykite "Exchange" administravimo centrą.
    - Spustelėkite **organizacija**, tada dukart spustelėkite strategiją, priskirtą vartotojui pagal **atskirą bendrą naudojimą**. Tai strategija, kuri buvo grąžinta atliekant 2 veiksmą.
    - Puslapyje bendrinimo taisyklės pasirinkite kalendoriaus bendrinimo lygį, kurį norite leisti dalyje nurodykite, kurią **informaciją norite bendrinti**; spustelėkite **įrašyti**.

Daugiau informacijos rasite: ["strategija neleidžia šiuo lygiu suteikti teises vienam ar daugiau gavėjo (-ų)" klaida, kai vartotojas bando bendrinti kalendorių](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
