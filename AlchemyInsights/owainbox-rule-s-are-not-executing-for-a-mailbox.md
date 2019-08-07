---
title: 1332 OWA - aplankui Gauta yra ne vykdančiajai pašto dėžutės
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204068"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="11f9f-102">Aplanko Gauta taisyklę neveikia kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="11f9f-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="11f9f-103">Patikrinkite šiuos parametrus:</span><span class="sxs-lookup"><span data-stu-id="11f9f-103">Verify the following settings:</span></span>

- <span data-ttu-id="11f9f-104">Pranešimas gali būti nukreipti, persiųsti ar atsakymų į automatiškai remiantis aplanko Gauta taisykles tik vieną kartą.</span><span class="sxs-lookup"><span data-stu-id="11f9f-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="11f9f-105">Nukreipiama taisyklė (yra aplanko Gauta taisyklę arba pašto srauto taisyklės, taip pat žinomas kaip transportavimo taisyklę) galite pridėti ne daugiau kaip dešimt persiuntimo gavėjams žinutę.</span><span class="sxs-lookup"><span data-stu-id="11f9f-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="11f9f-106">Norėdami gauti daugiau informacijos, peržiūrėkite [žurnalo, transporto ir pašto dėžutę taisyklė apriboja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="11f9f-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="11f9f-107">Aplanko Gauta taisykles neveikia dėl pakaitinių registravimo žurnale pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="11f9f-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="11f9f-108">Daugiau informacijos apie alternatyvius registravimo žurnale pašto dėžutę, ieškokite [alternatyvų registravimo žurnale pašto dėžutę](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="11f9f-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="11f9f-109">Norėdami išspręsti šias problemas, peržiūrėkite [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="11f9f-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="11f9f-110">Jei nereikia taikyti ankstesnius jo numerius, paleisti aplanko Gauta taisyklę diagnostikos ataskaitą prieš galite eskaluoti šią problemą į Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="11f9f-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="11f9f-111">Atidaryti pašto dėžutę programoje "Outlook" internete, ir spustelėkite</span><span class="sxs-lookup"><span data-stu-id="11f9f-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="11f9f-112">**Parametrai** > **Peržiūrėti visus "Outlook" parametrai** > **Mail** > **taisykles**.</span><span class="sxs-lookup"><span data-stu-id="11f9f-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="11f9f-113">Puslapio apačioje spustelėkite, **Jei jūsų taisyklės neveikia Paspaudę nuorodą sukurti diagnostikos ataskaitą**.</span><span class="sxs-lookup"><span data-stu-id="11f9f-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
