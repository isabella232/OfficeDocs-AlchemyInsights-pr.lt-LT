---
title: Reikia pagalbos su el. laiškų siuntimo apribojimais?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836287"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="4025c-102">Reikia pagalbos su el. laiškų siuntimo apribojimais?</span><span class="sxs-lookup"><span data-stu-id="4025c-102">Need help with email sending limits?</span></span>

<span data-ttu-id="4025c-103">Žemiau pateikta **dizainu paremti siuntimo apribojimai** taikomi paslaugai.</span><span class="sxs-lookup"><span data-stu-id="4025c-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="4025c-104">Daugiau informacijos apie šiuos apribojimus pateikta [čia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="4025c-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="4025c-105">Norint apriboti neužsakytų masinių pranešimų pristatymą, kiekvienam vartotojui taikome **gavėjų kiekio apribojimus visiems siunčiamiems ir vidiniams pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="4025c-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="4025c-106">Visuose SKU, šis apribojimas yra **10 000 gavėjų per dieną**.</span><span class="sxs-lookup"><span data-stu-id="4025c-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="4025c-107">Klientai, kuriems reikia siųsti teisėtus komercinius masinius el. laiškus (pvz., naujienlaiškius klientams), turėtų naudoti trečiųjų šalių tiekėjus, kurie specializuojasi tokių paslaugų teikime.</span><span class="sxs-lookup"><span data-stu-id="4025c-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="4025c-108">**Pastaba**: Pasiekus gavėjų kiekio apribojimo limitą, pranešimų iš šios pašto dėžutės siųsti negalima, kol gavėjų, kuriems siunčiami pranešimai per pastarąsias 24 val., skaičius netaps mažesniu už limitą.</span><span class="sxs-lookup"><span data-stu-id="4025c-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="4025c-109">Vartotojas negalės siųsti pranešimų, kol taip neatsitiks.</span><span class="sxs-lookup"><span data-stu-id="4025c-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="4025c-110">Pranešimų kiekio apribojimas, **30 pranešimų per minutę**, taikomas visuose SKU.</span><span class="sxs-lookup"><span data-stu-id="4025c-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="4025c-111">Tai nustato, kiek pranešimų vartotojas gali siųsti iš savo „Exchange Online“ paskyros per nurodytą laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="4025c-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="4025c-112">**Didžiausias leistinas gavėjų skaičius laukuose Kam:, Kopija: ir Nematoma kopija** vienam el. laiškui, visuose SKU, yra **1 000 gavėjų**.</span><span class="sxs-lookup"><span data-stu-id="4025c-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="4025c-113">Norėdami tinkinti šį apribojimą, eikite [čia](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="4025c-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
