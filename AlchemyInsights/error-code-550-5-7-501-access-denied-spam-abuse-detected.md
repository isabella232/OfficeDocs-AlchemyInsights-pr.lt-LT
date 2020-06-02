---
title: Klaidos kodas 550 5.7.501 Prieiga uždrausta, aptiktas piktnaudžiavimas šlamštu
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 9fd4f14798f27e7bf93daceb3620aff9b7f9e8ed
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506818"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="a1371-102">550 5.7.501 Prieiga uždrausta, aptiktas piktnaudžiavimas šlamštu</span><span class="sxs-lookup"><span data-stu-id="a1371-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="a1371-103">Paprastai šis pranešimas atsiranda, kai vartotojai siunčia el. laiškus iš IP adresų naudodami pradinį *.onmicrosoft.com* domeną, kuris priskirtas naujiems nuomininkams "Microsoft 365".</span><span class="sxs-lookup"><span data-stu-id="a1371-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="a1371-104">Lengviausias būdas išspręsti šią problemą yra:</span><span class="sxs-lookup"><span data-stu-id="a1371-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="a1371-105">[Įtraukite domeną į nuomotoją](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="a1371-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="a1371-106">[Pakeiskite pagrindinį naudotojų el. pašto adresą](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) į naują pasirinktinį domeną, kurį ką tik įtraukėte.</span><span class="sxs-lookup"><span data-stu-id="a1371-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
