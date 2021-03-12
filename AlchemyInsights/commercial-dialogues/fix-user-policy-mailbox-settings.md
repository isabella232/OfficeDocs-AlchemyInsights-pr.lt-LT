---
title: Vartotojų strategijos/pašto dėžutės parametrų taisymas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750556"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="c82c4-102">Vartotojų strategijos/pašto dėžutės parametrų taisymas</span><span class="sxs-lookup"><span data-stu-id="c82c4-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="c82c4-103">Pašto dėžutės nepageidaujamo pašto parametrai paveikė šį pranešimą.</span><span class="sxs-lookup"><span data-stu-id="c82c4-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="c82c4-104">Norėdami peržiūrėti parametrus, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="c82c4-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="c82c4-105">"Exchange Management Shell" Paleistis.</span><span class="sxs-lookup"><span data-stu-id="c82c4-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="c82c4-106">Daugiau informacijos ieškokite " [Exchange" valdymo aplinkos atidarymas](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="c82c4-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="c82c4-107">Vykdykite šią komandą (naudodami vartotojo elektroninio pašto adresą):  **get-mailboxjunkmailconfiguration-tapatybė "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="c82c4-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="c82c4-108">Patikrinkite, ar siuntėjo elektroninio pašto adresas priklauso **TrustedSendersAndDomains** arba **Blockedsendersanddomains**.</span><span class="sxs-lookup"><span data-stu-id="c82c4-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="c82c4-109">Jei el. pašto adresas yra viename iš sąrašų, gali tekti jį pašalinti.</span><span class="sxs-lookup"><span data-stu-id="c82c4-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="c82c4-110">Norėdami sužinoti daugiau, žiūrėkite [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="c82c4-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
