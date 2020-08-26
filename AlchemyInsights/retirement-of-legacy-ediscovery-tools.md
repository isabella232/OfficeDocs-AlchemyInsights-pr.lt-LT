---
title: Senstelėjusių "Udiscovery" įrankių išėjimas
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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902628"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="4ea68-102">Senstelėjusių "Udiscovery" įrankių išėjimas</span><span class="sxs-lookup"><span data-stu-id="4ea68-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="4ea68-103">"Microsoft 365" atitikties centre naudojant naująsias ir geresnes "eDiscovery" funkcijas, toliau pateikti senstelėjusių eDiscovery įrankiai ir commandlet bus išėję per ateinančius mėnesius:</span><span class="sxs-lookup"><span data-stu-id="4ea68-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="4ea68-104">[Vietoje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) "Exchange" administravimo centre [turi](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) būti "e" aptikimas ir vietos.</span><span class="sxs-lookup"><span data-stu-id="4ea68-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="4ea68-105">"Exchange Online" "PowerShell" cmdlet, palaikančių vietinį "Udiscovery" ir vietinį sulaikymą.</span><span class="sxs-lookup"><span data-stu-id="4ea68-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="4ea68-106">(Šios "cmdlet" bendrai identifikuotos kaip \*-MailboxSearch "cmdlet"). Tai aprėpia šias "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="4ea68-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="4ea68-107">Naujoji MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4ea68-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="4ea68-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4ea68-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="4ea68-109">"Stop-MailboxSearch"</span><span class="sxs-lookup"><span data-stu-id="4ea68-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="4ea68-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="4ea68-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="4ea68-111">[Ieškos pašto dėžutės](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet "Exchange Online PowerShell".</span><span class="sxs-lookup"><span data-stu-id="4ea68-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="4ea68-112">Toliau nurodytos "Exchange" žiniatinklio tarnybų API operacijos:</span><span class="sxs-lookup"><span data-stu-id="4ea68-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="4ea68-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="4ea68-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="4ea68-114">Setholdonupašto dėžutės</span><span class="sxs-lookup"><span data-stu-id="4ea68-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="4ea68-115">Getholdonpašto dėžutės</span><span class="sxs-lookup"><span data-stu-id="4ea68-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="4ea68-116">Išplėstinė "Udiscovery" v 1.0</span><span class="sxs-lookup"><span data-stu-id="4ea68-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="4ea68-117">**Išėjimo į pensiją grafikas**:</span><span class="sxs-lookup"><span data-stu-id="4ea68-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="4ea68-118">**2020 liepos 1 d** . Nebegalite kurti naujų paieškų ir sulaikymų, tačiau galite vykdyti, redaguoti ir naikinti esamą iešką savo pačių rizika.</span><span class="sxs-lookup"><span data-stu-id="4ea68-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="4ea68-119">"Microsoft" palaikymo tarnyba nebepalaiko in-Place udiscovery & priklauso EAC.</span><span class="sxs-lookup"><span data-stu-id="4ea68-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="4ea68-120">**Spalio 1 d., 2020** Vietoje "udiscovery" & turi funkciją EAC bus Patalpinta tik skaitymo režimu, todėl galite pašalinti tik esamas paieškas ir sulaikymus.</span><span class="sxs-lookup"><span data-stu-id="4ea68-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="4ea68-121">**Daugiau informacijos rasite**:</span><span class="sxs-lookup"><span data-stu-id="4ea68-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="4ea68-122">Senstelėjusių e. duomenų aptikimo paieškų ir sulaikymų "Microsoft 365" atitikties centro perkėlimas</span><span class="sxs-lookup"><span data-stu-id="4ea68-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="4ea68-123">Senstelėjusių "Udiscovery" įrankių išėjimas</span><span class="sxs-lookup"><span data-stu-id="4ea68-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="4ea68-124">DUK apie vietinį "Udiscovery" ir vietinį sulaikymą</span><span class="sxs-lookup"><span data-stu-id="4ea68-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



