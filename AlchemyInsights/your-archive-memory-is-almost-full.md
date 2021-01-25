---
title: Jūsų archyvo pašto dėžutė beveik U3/4imta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974408"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="b15e9-102">Jūsų archyvo pašto dėžutė beveik U3/4imta</span><span class="sxs-lookup"><span data-stu-id="b15e9-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="b15e9-103">Jei vartotojas gauna įspėjimą; **Jūsų archyvo pašto dėžutė yra beveik visa** arba reikia padidinti jų archyvo pašto dėžutę, Štai keletas patarimų:</span><span class="sxs-lookup"><span data-stu-id="b15e9-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="b15e9-104">Jei vartotojui priskirtas "Exchange Online" 1 planas, atnaujinkite versiją į " **Exchange Online" 2 plano** licenciją, kad padidintumėte dydį nuo 50 GB iki 100gb.</span><span class="sxs-lookup"><span data-stu-id="b15e9-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="b15e9-105">Jei vartotojui jau priskirtas vienas iš šių veiksmų: " **Exchange Online" 2 planas** arba "Exchange Online" 1 planas su "Exchange Online" archyvavimo papildyme, atlikite toliau nurodytus veiksmus, kad įgalintumėte automatiškai plėsti archyvavimą:.</span><span class="sxs-lookup"><span data-stu-id="b15e9-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="b15e9-106">[Prisijungimas prie "Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)" "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="b15e9-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="b15e9-107">Paleiskite šį commandleisti vartotojui:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="b15e9-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="b15e9-108">Vykdykite šią komandą, kad patvirtintumėte, jog jis įgalintas vartotojui:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="b15e9-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="b15e9-109">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="b15e9-109">For more information see:</span></span>

- [<span data-ttu-id="b15e9-110"> Neriboto archyvavimo – administratorių žinynas – "Microsoft 365" atitiktis | "Microsoft" dokumentai</span><span class="sxs-lookup"><span data-stu-id="b15e9-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="b15e9-111">"Exchange Online" limitai – paslaugų aprašai | "Microsoft" dokumentai</span><span class="sxs-lookup"><span data-stu-id="b15e9-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="b15e9-112">Versijos naujinimas į kitą verslo planą | "Microsoft" dokumentai</span><span class="sxs-lookup"><span data-stu-id="b15e9-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

