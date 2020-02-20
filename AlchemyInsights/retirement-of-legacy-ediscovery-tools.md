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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="45dff-102">Legacy eDiscovery įrankiai išėjimo į pensiją</span><span class="sxs-lookup"><span data-stu-id="45dff-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="45dff-103">Dėl naujos ir patobulintos eDiscovery funkcijos Microsoft 365 atitikties centras, šių senesnius eDiscovery įrankiai ir commandlet bus pensininkas per ateinančius mėnesius:</span><span class="sxs-lookup"><span data-stu-id="45dff-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="45dff-104">Vietoje [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ir [vietoje sulaikymai](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="45dff-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="45dff-105">Exchange Online "PowerShell" cmdlet, kurie palaiko vietoje eDiscovery ir vietoje sulaikymų.</span><span class="sxs-lookup"><span data-stu-id="45dff-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="45dff-106">(Šie cmdlet yra bendrai identifikuojami kaip \*-MailboxSearch cmdlet.) Tai apima šias cmdlet:</span><span class="sxs-lookup"><span data-stu-id="45dff-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="45dff-107">Naujas MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="45dff-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="45dff-108">Pradėti MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="45dff-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="45dff-109">Stotelė-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="45dff-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="45dff-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="45dff-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="45dff-111">[Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet Exchange Online "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="45dff-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="45dff-112">Toliau nurodytos "Exchange" žiniatinklio paslaugų API operacijos:</span><span class="sxs-lookup"><span data-stu-id="45dff-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="45dff-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="45dff-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="45dff-114">Setholdondėžučių</span><span class="sxs-lookup"><span data-stu-id="45dff-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="45dff-115">GetHoldOnMailboxes pašto dėžutės</span><span class="sxs-lookup"><span data-stu-id="45dff-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="45dff-116">Office 365 Išplėstinė eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="45dff-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="45dff-117">**Išėjimo į pensiją laiko skalė**:</span><span class="sxs-lookup"><span data-stu-id="45dff-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="45dff-118">Balandžio 1, 2020: negalėsite kurti naujų paieškų ir sulaikymų, tačiau vis tiek galite vykdyti, redaguoti ir naikinti esamas paieškas savo pačių rizika.</span><span class="sxs-lookup"><span data-stu-id="45dff-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="45dff-119">Microsoft Support nebepalaikys vietoje eDiscovery & sulaikymų EAC.</span><span class="sxs-lookup"><span data-stu-id="45dff-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="45dff-120">Liepos 1, 2020: vietoje eDiscovery & turi funkcionalumą, EAC bus padėtas tik skaitymo režimu.</span><span class="sxs-lookup"><span data-stu-id="45dff-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="45dff-121">Tai reiškia, kad galėsite pašalinti tik esamas paieškas ir sulaikymus.</span><span class="sxs-lookup"><span data-stu-id="45dff-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="45dff-122">**Daugiau informacijos rasite**:</span><span class="sxs-lookup"><span data-stu-id="45dff-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="45dff-123">Perkelti senstelėjusios įrangos eDiscovery paieškas ir sulaikymus Microsoft 365 atitikties centras</span><span class="sxs-lookup"><span data-stu-id="45dff-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="45dff-124">Senstelėjusių eDiscovery įrankių išėjimas į pensiją</span><span class="sxs-lookup"><span data-stu-id="45dff-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="45dff-125">DUK apie vietoje aptikimą ir vietos sulaikymus</span><span class="sxs-lookup"><span data-stu-id="45dff-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



