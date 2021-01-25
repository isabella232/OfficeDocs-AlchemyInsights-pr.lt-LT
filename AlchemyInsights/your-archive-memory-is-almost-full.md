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
# <a name="your-archive-mailbox-is-almost-full"></a>Jūsų archyvo pašto dėžutė beveik U3/4imta

Jei vartotojas gauna įspėjimą; **Jūsų archyvo pašto dėžutė yra beveik visa** arba reikia padidinti jų archyvo pašto dėžutę, Štai keletas patarimų:

1. Jei vartotojui priskirtas "Exchange Online" 1 planas, atnaujinkite versiją į " **Exchange Online" 2 plano** licenciją, kad padidintumėte dydį nuo 50 GB iki 100gb.
1. Jei vartotojui jau priskirtas vienas iš šių veiksmų: " **Exchange Online" 2 planas** arba "Exchange Online" 1 planas su "Exchange Online" archyvavimo papildyme, atlikite toliau nurodytus veiksmus, kad įgalintumėte automatiškai plėsti archyvavimą:.
 
    1. [Prisijungimas prie "Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)" "PowerShell".
    2. Paleiskite šį commandleisti vartotojui:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Vykdykite šią komandą, kad patvirtintumėte, jog jis įgalintas vartotojui:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Daugiau informacijos rasite:

- [ Neriboto archyvavimo – administratorių žinynas – "Microsoft 365" atitiktis | "Microsoft" dokumentai](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- ["Exchange Online" limitai – paslaugų aprašai | "Microsoft" dokumentai](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Versijos naujinimas į kitą verslo planą | "Microsoft" dokumentai](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

