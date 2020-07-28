---
title: Keli objektai turi tą patį el. pašto adresą kaip ir tapatybė
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439190"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="2b75c-102">Keli objektai turi tą patį el. pašto adresą kaip ir tapatybė</span><span class="sxs-lookup"><span data-stu-id="2b75c-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="2b75c-103">**Keli objektai**</span><span class="sxs-lookup"><span data-stu-id="2b75c-103">**Multiple objects**</span></span>

<span data-ttu-id="2b75c-104">Viena iš dažniausiai pasitaikančių šios klaidos priežasčių yra neįmanoma tinkamai nukreipti "Outlook Web Access" užklausos, jei yra keli objektai, turintys tą patį el. pašto adresą kaip tapatybė.</span><span class="sxs-lookup"><span data-stu-id="2b75c-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="2b75c-105">Norėdami rasti šiuos objektus, vykdykite šias komandas:</span><span class="sxs-lookup"><span data-stu-id="2b75c-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="2b75c-106">· Gavėjas<email address></span><span class="sxs-lookup"><span data-stu-id="2b75c-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="2b75c-107">· Gaukite vartotoją<email address></span><span class="sxs-lookup"><span data-stu-id="2b75c-107">· Get-User <email address></span></span>

<span data-ttu-id="2b75c-108">· Get-User <email address> -SoftDeletedUser Get-User -SoftDeletedUser Get-User -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="2b75c-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="2b75c-109">· Susisiekite su mumis<email address></span><span class="sxs-lookup"><span data-stu-id="2b75c-109">· Get-Contact <email address></span></span>

<span data-ttu-id="2b75c-110">· Get-Mailbox -PublicFolder Gauti pašto dėžutės <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="2b75c-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="2b75c-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox Gauti pašto dėžutės - IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="2b75c-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="2b75c-112">· Get-Mailbox -InactiveMailboxOnly Gauti pašto dėžutės- <email address> InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="2b75c-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="2b75c-113">Norėdami išspręsti šią problemą, pašalinkite kelis objektus su tuo pačiu el. pašto tapatybe ir įsitikinkite, kad yra vienas objektas su konkrečiu el. pašto tapatybe ir kad jo gavėjo tipas yra UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="2b75c-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="2b75c-114">**Tas pats adresas naudojamas įmonėms ir vartotojų pašto dėžutėms**</span><span class="sxs-lookup"><span data-stu-id="2b75c-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="2b75c-115">Kita priežastis yra, kai tas pats adresas naudojamas verslo ir vartotojų pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="2b75c-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="2b75c-116">Tokiu atveju vartotojas turi pakeisti savo pagrindinį vartotojo pseudonimą, kol kavinė palaiko šį scenarijų.</span><span class="sxs-lookup"><span data-stu-id="2b75c-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="2b75c-117">Tai nuolatinė klaida, kuri neišeina be įsikišimo.</span><span class="sxs-lookup"><span data-stu-id="2b75c-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="2b75c-118">Išsamesnės informacijos [ieškokite "Microsoft" paskyros el. pašto adreso arba telefono numerio keitimas.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)</span><span class="sxs-lookup"><span data-stu-id="2b75c-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>