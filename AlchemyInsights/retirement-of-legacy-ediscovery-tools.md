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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798557"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="87d07-102">Senstelėjusių el. duomenų aptikimo įrankių išėjimas</span><span class="sxs-lookup"><span data-stu-id="87d07-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="87d07-103">Dėl naujų ir patobulintų el. duomenų aptikimo funkcijų "Microsoft 365" atitikties centre ateinančiais mėnesiais bus panaikinti šie senesni el. duomenų aptikimo įrankiai ir komandos:</span><span class="sxs-lookup"><span data-stu-id="87d07-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="87d07-104">[Vietoje eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span><span class="sxs-lookup"><span data-stu-id="87d07-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="87d07-105">"Exchange Online PowerShell" "cmdlet", kurios In-Place el. duomenų aptikimą ir In-Place sulaikymas.</span><span class="sxs-lookup"><span data-stu-id="87d07-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="87d07-106">(Šios "cmdlet" bendrai identifikuojamos kaip \*-MailboxSearch cmdlet.) Tai apima šias "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="87d07-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="87d07-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="87d07-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="87d07-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="87d07-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="87d07-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="87d07-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="87d07-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="87d07-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="87d07-111">["Exchange](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Online PowerShell" ieškos pašto dėžutės "cmdlet".</span><span class="sxs-lookup"><span data-stu-id="87d07-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="87d07-112">Toliau nurodytos operacijos "Exchange Web Services" API:</span><span class="sxs-lookup"><span data-stu-id="87d07-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="87d07-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="87d07-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="87d07-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="87d07-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="87d07-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="87d07-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="87d07-116">Išplėstinis el. duomenų aptikimas v1.0</span><span class="sxs-lookup"><span data-stu-id="87d07-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="87d07-117">**Išėjimo į pensiją laiko planavimo juosta:**</span><span class="sxs-lookup"><span data-stu-id="87d07-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="87d07-118">**2020 m. liepos 1 d.** Nebegalėsite kurti naujų paieškų ir sulaikytus įrašus, bet galite vykdyti, redaguoti ir naikinti esamas ieškas savo pačių rizika.</span><span class="sxs-lookup"><span data-stu-id="87d07-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="87d07-119">"Microsoft" palaikymas nebepalaiko In-Place el. duomenų aptikimo & EAC laiko.</span><span class="sxs-lookup"><span data-stu-id="87d07-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="87d07-120">**2020 m. spalio 1** d. In-Place eDiscovery & Holds" funkcijos EAC bus įdėtos tik skaitymo režimu, todėl galima pašalinti tik esamas ieškas ir sulaikytus.</span><span class="sxs-lookup"><span data-stu-id="87d07-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="87d07-121">**Daugiau informacijos žr.:**</span><span class="sxs-lookup"><span data-stu-id="87d07-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="87d07-122">Senstelėjusios el. duomenų aptikimo ieškos ir laiko perkėlimas į "Microsoft 365" atitikties centrą</span><span class="sxs-lookup"><span data-stu-id="87d07-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="87d07-123">Senstelėjusių el. duomenų aptikimo įrankių išėjimas</span><span class="sxs-lookup"><span data-stu-id="87d07-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="87d07-124">DUK apie "In-Place" el. duomenų aptikimą ir In-Place "Holds"</span><span class="sxs-lookup"><span data-stu-id="87d07-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



