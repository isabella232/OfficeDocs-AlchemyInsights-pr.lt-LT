---
title: Senstelėjusių el. duomenų aptikimo įrankių išėjimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074682"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Senstelėjusių el. duomenų aptikimo įrankių išėjimas

Dėl naujų ir patobulintų el. duomenų aptikimo funkcijų "Microsoft 365" atitikties centre ateinančiais mėnesiais bus panaikinti šie senesni el. duomenų aptikimo įrankiai ir komandos:

- [Vietoje eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [and In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.

- "Exchange Online PowerShell" "cmdlet", kurios palaiko In-Place el. duomenų aptikimą ir In-Place sulaikymas. (Šios "cmdlet" bendrai identifikuojamos kaip *-MailboxSearch cmdlet.) Tai apima šias "cmdlet":

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- ["PowerShell" ieškos](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) pašto dėžutės "cmdlet" Exchange Online".
- Toliau nurodytos operacijos Exchange žiniatinklio tarnybų API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Išėjimo į pensiją laiko planavimo juosta:**
- **2020 m. liepos 1 d.** Nebegalėsite kurti naujų paieškų ir sulaikytus įrašus, bet galite vykdyti, redaguoti ir naikinti esamas ieškas savo pačių rizika. "Microsoft" palaikymas nebepalaiko In-Place el. duomenų aptikimo & EAC laiko.
    
- **2020 m. spalio 1** d. In-Place eDiscovery & Holds" funkcijos EAC bus įdėtos tik skaitymo režimu, todėl galima pašalinti tik esamas ieškas ir sulaikytus.

**Daugiau informacijos žr.:**

 - [Senstelėjusios el. duomenų aptikimo ieškos ir laiko perkėlimas į "Microsoft 365" atitikties centras](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Senstelėjusių el. duomenų aptikimo įrankių išėjimas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [DUK apie "In-Place" el. duomenų aptikimą ir In-Place "Holds"](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



