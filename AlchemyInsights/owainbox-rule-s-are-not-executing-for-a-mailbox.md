---
title: 1332 OWA - aplankui Gauta yra ne vykdančiajai pašto dėžutės
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858752"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5d39a-102">Aplanko Gauta taisyklę neveikia kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="5d39a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5d39a-103">Patikrinkite šiuos parametrus:</span><span class="sxs-lookup"><span data-stu-id="5d39a-103">Verify the following settings:</span></span>

- <span data-ttu-id="5d39a-104">Pranešimas gali būti nukreipti, persiųsti ar atsakymų į automatiškai remiantis aplanko Gauta taisykles tik vieną kartą.</span><span class="sxs-lookup"><span data-stu-id="5d39a-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5d39a-105">Nukreipiama taisyklė (yra aplanko Gauta taisyklę arba pašto srauto taisyklės, taip pat žinomas kaip transportavimo taisyklę) galite pridėti ne daugiau kaip dešimt persiuntimo gavėjams žinutę.</span><span class="sxs-lookup"><span data-stu-id="5d39a-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5d39a-106">Norėdami gauti daugiau informacijos, peržiūrėkite [žurnalo, transporto ir pašto dėžutę taisyklė apriboja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="5d39a-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5d39a-107">Aplanko Gauta taisykles neveikia dėl pakaitinių registravimo žurnale pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="5d39a-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5d39a-108">Daugiau informacijos apie alternatyvius registravimo žurnale pašto dėžutę, ieškokite [alternatyvų registravimo žurnale pašto dėžutę](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5d39a-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5d39a-109">Norėdami išspręsti šias problemas, peržiūrėkite [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="5d39a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5d39a-110">Jei nereikia taikyti ankstesnius jo numerius, paleisti aplanko Gauta taisyklę diagnostikos ataskaitą prieš galite eskaluoti šią problemą į Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="5d39a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5d39a-111">Atidaryti pašto dėžutę programoje "Outlook" internete, ir spustelėkite **Parametrai** \> **funkcijos** \> **tvarkyti el. pašto** \> **aplanko Gauta taisykles**.</span><span class="sxs-lookup"><span data-stu-id="5d39a-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="5d39a-112">Puslapio apačioje spustelėkite, **Jei jūsų taisyklės neveikia Paspaudę nuorodą sukurti diagnostikos ataskaitą**.</span><span class="sxs-lookup"><span data-stu-id="5d39a-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
