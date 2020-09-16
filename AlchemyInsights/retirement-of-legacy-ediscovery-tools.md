---
title: Senstelėjusių "Udiscovery" įrankių išėjimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727791"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Senstelėjusių "Udiscovery" įrankių išėjimas

"Microsoft 365" atitikties centre naudojant naująsias ir geresnes "eDiscovery" funkcijas, toliau pateikti senstelėjusių eDiscovery įrankiai ir commandlet bus išėję per ateinančius mėnesius:

- [Vietoje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) "Exchange" administravimo centre [turi](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) būti "e" aptikimas ir vietos.

- "Exchange Online" "PowerShell" cmdlet, palaikančių vietinį "Udiscovery" ir vietinį sulaikymą. (Šios "cmdlet" bendrai identifikuotos kaip *-MailboxSearch "cmdlet"). Tai aprėpia šias "cmdlet":

    - [Naujoji MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - ["Stop-MailboxSearch"](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Ieškos pašto dėžutės](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet "Exchange Online PowerShell".
- Toliau nurodytos "Exchange" žiniatinklio tarnybų API operacijos:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonupašto dėžutės](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonpašto dėžutės](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Išplėstinė "Udiscovery" v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Išėjimo į pensiją grafikas**:
- **2020 liepos 1 d** . Nebegalite kurti naujų paieškų ir sulaikymų, tačiau galite vykdyti, redaguoti ir naikinti esamą iešką savo pačių rizika. "Microsoft" palaikymo tarnyba nebepalaiko in-Place udiscovery & priklauso EAC.
    
- **Spalio 1 d., 2020** Vietoje "udiscovery" & turi funkciją EAC bus Patalpinta tik skaitymo režimu, todėl galite pašalinti tik esamas paieškas ir sulaikymus.

**Daugiau informacijos rasite**:

 - [Senstelėjusių e. duomenų aptikimo paieškų ir sulaikymų "Microsoft 365" atitikties centro perkėlimas](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Senstelėjusių "Udiscovery" įrankių išėjimas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [DUK apie vietinį "Udiscovery" ir vietinį sulaikymą](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



