---
title: Pašto dėžučių peradresavimo adresų tikrinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482776"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="876db-102">Pašto dėžučių peradresavimo adresų tikrinimas</span><span class="sxs-lookup"><span data-stu-id="876db-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="876db-103">Kartais "hackers" peradresuoja vartotojų el. laiškus, todėl pirmiausia patikrinsime, ar pašto dėžutėje yra peradresuotų adresų ir taisyklių.</span><span class="sxs-lookup"><span data-stu-id="876db-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="876db-104">Tada patikrinsime audito žurnalus.</span><span class="sxs-lookup"><span data-stu-id="876db-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="876db-105">Štai kaip patikrinti, ar yra peradresuotų adresų:</span><span class="sxs-lookup"><span data-stu-id="876db-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="876db-106">Pasirinkite **vartotojai**  >  **aktyvūs vartotojai**.</span><span class="sxs-lookup"><span data-stu-id="876db-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="876db-107">Pasirinkite vartotoją, kurio paskyra buvo pažeista.</span><span class="sxs-lookup"><span data-stu-id="876db-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="876db-108">Pasirodžiusiame iškeliamojo dialogo lange išplėskite **pašto parametrai**, tada spustelėkite **Redaguoti** el. **pašto peradresavimą**.</span><span class="sxs-lookup"><span data-stu-id="876db-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="876db-109">Pašalinkite visus peradresavimo adresus, kurių neatpažįstate.</span><span class="sxs-lookup"><span data-stu-id="876db-109">Remove any forwarding addresses you don't recognize.</span></span>