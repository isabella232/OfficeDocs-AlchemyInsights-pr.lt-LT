---
title: Trikčių diagnostika įvykių el. paštu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569137"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="dd544-102">Trikčių diagnostika įvykių el. paštu</span><span class="sxs-lookup"><span data-stu-id="dd544-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="dd544-103">Patikrinkite, ar funkcija įgalinta pašto dėžutės: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="dd544-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="dd544-104">Tada peržiūrėkite "Įvykiai iš el. pašto" žurnalus **Eksporto-MailboxDiagnosticLogs <mailbox> komponento TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="dd544-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="dd544-105">Žurnaluose "Įvykiai iš el. pašto" raskite internetMessageId, kuris atitinka pašto dėžutės elementą.</span><span class="sxs-lookup"><span data-stu-id="dd544-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="dd544-106">TrustScore nustato, ar elementas yra įtrauktas, ar ne.</span><span class="sxs-lookup"><span data-stu-id="dd544-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="dd544-107">Įvykiai bus įtraukti tik tada, jei TrustScore = "Patikimas".</span><span class="sxs-lookup"><span data-stu-id="dd544-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="dd544-108">TrustScore nustatomas pagal SPF, Dkim arba Dmarc ypatybes, kurios yra pranešimo antraštėje.</span><span class="sxs-lookup"><span data-stu-id="dd544-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="dd544-109">Norėdami peržiūrėti šias ypatybes:</span><span class="sxs-lookup"><span data-stu-id="dd544-109">To view these properties:</span></span>

<span data-ttu-id="dd544-110">**Darbalaukio "Outlook"**</span><span class="sxs-lookup"><span data-stu-id="dd544-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="dd544-111">Atidaryti elementą</span><span class="sxs-lookup"><span data-stu-id="dd544-111">Open the item</span></span>
- <span data-ttu-id="dd544-112">Failų > ypatybės – > interneto antraštės</span><span class="sxs-lookup"><span data-stu-id="dd544-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="dd544-113">Arba</span><span class="sxs-lookup"><span data-stu-id="dd544-113">or</span></span>

<span data-ttu-id="dd544-114">**MFCMapi (Netoli viešbučio mfc)**</span><span class="sxs-lookup"><span data-stu-id="dd544-114">**MFCMapi**</span></span>

- <span data-ttu-id="dd544-115">Pereiti į aplanko Gauta elementą</span><span class="sxs-lookup"><span data-stu-id="dd544-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="dd544-116">Ieškokite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="dd544-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="dd544-117">Šios savybės nustatomos ir registruojamos transportavimo ir maršruto parinkimo metu.</span><span class="sxs-lookup"><span data-stu-id="dd544-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="dd544-118">Jei reikia daugiau trikčių šalinimo, gali tekti stebėti, kaip palaikymo tarnyba dėl SPF, DKIM ir.arba DMARC trikčių.</span><span class="sxs-lookup"><span data-stu-id="dd544-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>