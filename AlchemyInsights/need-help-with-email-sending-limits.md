---
title: Reikia pagalbos dėl el. pašto siuntimo apribojimų?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357867"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="30af8-102">Reikia pagalbos dėl el. pašto siuntimo apribojimų?</span><span class="sxs-lookup"><span data-stu-id="30af8-102">Need help with email sending limits?</span></span>

<span data-ttu-id="30af8-103">Žemiau yra **by-design siuntimo apribojimai** vykdomi paslauga.</span><span class="sxs-lookup"><span data-stu-id="30af8-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="30af8-104">Daugiau informacijos apie šias ribas yra dokumentuojama [čia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="30af8-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="30af8-105">Norėdami neskatinti neprašytų masinių pranešimų pristatymo, taikome kiekvieno vartotojo **gavėjų tarifo apribojimus visiems siunčiamiems ir vidiniams pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="30af8-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="30af8-106">Visose SKU ribos yra **10 000 gavėjų per dieną**.</span><span class="sxs-lookup"><span data-stu-id="30af8-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="30af8-107">Klientai, kuriems reikia siųsti teisėtą masinį komercinį el. laišką (pvz., klientų informacinius biuletenius), turėtų naudoti trečiųjų šalių teikėjus, kurie specializuojasi šiose paslaugose.</span><span class="sxs-lookup"><span data-stu-id="30af8-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="30af8-108">**Pastaba:** pasiekus gavėjo tarifo ribą, pranešimai negali būti siunčiami iš pašto dėžutės, kol gavėjų, kurie buvo išsiųsti pranešimai per pastarąsias 24 valandas, skaičius nukris žemiau ribos.</span><span class="sxs-lookup"><span data-stu-id="30af8-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="30af8-109">Vartotojas negalės siųsti pranešimų iki to momento.</span><span class="sxs-lookup"><span data-stu-id="30af8-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="30af8-110">Pranešimų dažnio limitas **30 pranešimų per minutę** taikomas visiems SKU.</span><span class="sxs-lookup"><span data-stu-id="30af8-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="30af8-111">Tai nustato, kiek pranešimų vartotojas gali siųsti iš savo Exchange Online abonemento per nurodytą laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="30af8-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="30af8-112">Maksimalus gavėjų, leidžiamų vieno el. laiško **laukuose Kam, Kopija ir Nematoma kopija, skaičius** visuose SKU yra **1000 gavėjų.**</span><span class="sxs-lookup"><span data-stu-id="30af8-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="30af8-113">Norėdami tinkinti šią ribą, eikite [čia](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="30af8-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
