---
title: Legacy eDiscovery įrankiai išėjimo į pensiją
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157652"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Legacy eDiscovery įrankiai išėjimo į pensiją

Dėl naujos ir patobulintos eDiscovery funkcijos Microsoft 365 atitikties centras, šių senesnius eDiscovery įrankiai ir commandlet bus pensininkas per ateinančius mėnesius:

- Vietoje [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ir [vietoje sulaikymai](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administravimo centro.

- Exchange Online "PowerShell" cmdlet, kurie palaiko vietoje eDiscovery ir vietoje sulaikymų. (Šie cmdlet yra bendrai identifikuojami kaip *-MailboxSearch cmdlet.) Tai apima šias cmdlet:

    - [Naujas MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Pradėti MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stotelė-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet Exchange Online "PowerShell".
- Toliau nurodytos "Exchange" žiniatinklio paslaugų API operacijos:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdondėžučių](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes pašto dėžutės](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Išplėstinė eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Išėjimo į pensiją laiko skalė**:
- Balandžio 1, 2020: negalėsite kurti naujų paieškų ir sulaikymų, tačiau vis tiek galite vykdyti, redaguoti ir naikinti esamas paieškas savo pačių rizika. Microsoft Support nebepalaikys vietoje eDiscovery & sulaikymų EAC.

- Liepos 1, 2020: vietoje eDiscovery & turi funkcionalumą, EAC bus padėtas tik skaitymo režimu. Tai reiškia, kad galėsite pašalinti tik esamas paieškas ir sulaikymus.

**Daugiau informacijos rasite**:

 - [Perkelti senstelėjusios įrangos eDiscovery paieškas ir sulaikymus Microsoft 365 atitikties centras](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Senstelėjusių eDiscovery įrankių išėjimas į pensiją](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [DUK apie vietoje aptikimą ir vietos sulaikymus](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



