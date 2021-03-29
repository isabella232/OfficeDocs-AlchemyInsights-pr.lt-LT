---
title: Pašto dėžučių adresų peradresavimo tikrinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403319"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="155ba-102">Pašto dėžučių adresų peradresavimo tikrinimas</span><span class="sxs-lookup"><span data-stu-id="155ba-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="155ba-103">Kartais programišiai persiunčia vartotojų el. laiškus sau, todėl pirmiausia patikrinsime, ar nėra pašto dėžutės adresų ir taisyklių.</span><span class="sxs-lookup"><span data-stu-id="155ba-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="155ba-104">Tada patikrinsime audito žurnalus.</span><span class="sxs-lookup"><span data-stu-id="155ba-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="155ba-105">Štai kaip patikrinti, ar yra peradresavimo adresų:</span><span class="sxs-lookup"><span data-stu-id="155ba-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="155ba-106">Pasirinkite **Vartotojai**  >  **Aktyvūs vartotojai**.</span><span class="sxs-lookup"><span data-stu-id="155ba-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="155ba-107">Pasirinkite vartotoją, kurio paskyra buvo pažeista.</span><span class="sxs-lookup"><span data-stu-id="155ba-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="155ba-108">Rodomame iškeliamame meniu išplėskite **Pašto parametrai**, tada spustelėkite **Redaguoti el.** **pašto peradresavimui.**</span><span class="sxs-lookup"><span data-stu-id="155ba-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="155ba-109">Pašalinkite visus neatpažinus peradresavimo adresus.</span><span class="sxs-lookup"><span data-stu-id="155ba-109">Remove any forwarding addresses you don't recognize.</span></span>