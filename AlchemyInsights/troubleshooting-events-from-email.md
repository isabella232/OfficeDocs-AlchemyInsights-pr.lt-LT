---
title: Trikčių šalinimo įvykiai iš elektroninio pašto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658742"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="88ec0-102">Trikčių šalinimo įvykiai iš elektroninio pašto</span><span class="sxs-lookup"><span data-stu-id="88ec0-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="88ec0-103">Patikrinkite, ar įgalinta pašto dėžutės funkcija: \*\*get-Eventsofromemailconfiguration – tapatybė <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="88ec0-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="88ec0-104">Tada Pažvelkite į "įvykiai iš pašto" žurnalai **Export-MailboxDiagnosticLogs <mailbox> -komponento timeprofile**</span><span class="sxs-lookup"><span data-stu-id="88ec0-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="88ec0-105">Žurnaluose "įvykiai iš pašto" raskite InternetMessageId, atitinkantį elementą pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="88ec0-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="88ec0-106">TrustScore nustato, ar elementas įtrauktas, ar ne.</span><span class="sxs-lookup"><span data-stu-id="88ec0-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="88ec0-107">Įvykiai bus įtraukti tik jei TrustScore = "patikimas".</span><span class="sxs-lookup"><span data-stu-id="88ec0-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="88ec0-108">TrustScore nustatomas pagal SPF, DKIM arba DMARC ypatybes, kurios yra pranešimo antraštėje.</span><span class="sxs-lookup"><span data-stu-id="88ec0-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="88ec0-109">Norėdami peržiūrėti šias ypatybes:</span><span class="sxs-lookup"><span data-stu-id="88ec0-109">To view these properties:</span></span>

<span data-ttu-id="88ec0-110">**Kompiuterio "Outlook"**</span><span class="sxs-lookup"><span data-stu-id="88ec0-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="88ec0-111">Atidaryti elementą</span><span class="sxs-lookup"><span data-stu-id="88ec0-111">Open the item</span></span>
- <span data-ttu-id="88ec0-112">Failų > ypatybės – > interneto antraštės</span><span class="sxs-lookup"><span data-stu-id="88ec0-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="88ec0-113">arba</span><span class="sxs-lookup"><span data-stu-id="88ec0-113">or</span></span>

<span data-ttu-id="88ec0-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="88ec0-114">**MFCMapi**</span></span>

- <span data-ttu-id="88ec0-115">Pereiti į aplanko Gauta elementą</span><span class="sxs-lookup"><span data-stu-id="88ec0-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="88ec0-116">Ieškoti PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="88ec0-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="88ec0-117">Šios ypatybės nustatomos ir registruojamos transportavimo ir nukreipimo metu.</span><span class="sxs-lookup"><span data-stu-id="88ec0-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="88ec0-118">Norėdami gauti daugiau trikčių diagnostikos, jums gali tekti stebėti transportavimo palaikymą apie NPN, DKIM ir. or DMARC gedimus.</span><span class="sxs-lookup"><span data-stu-id="88ec0-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>