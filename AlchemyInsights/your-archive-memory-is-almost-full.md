---
title: Jūsų archyvo pašto dėžutė beveik pilna
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046760"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Jūsų archyvo pašto dėžutė beveik pilna

Jei vartotojas gauna įspėjimą; **Jūsų archyvo pašto dėžutė beveik** pilna arba reikia padidinti archyvo pašto dėžutės dydį, štai keli patarimai:

1. Jei vartotojui priskirtas 1 Exchange Online, atnaujinkite į **"Exchange Online 2** plano licenciją, kad padidintų dydį nuo 50 GB iki 100 GB.
1. Jei vartotojui jau priskirtas kuris nors iš šių veiksmų: **Exchange Online 2** planas arba "Exchange Online" 1 planas su ""Exchange Online" archyvavimas" papildinys, atlikite toliau nurodytus veiksmus, kad įgalintumėte automatinį archyvavimą:.
 
    1. [Prisijungimas "Exchange Online PowerShell".](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Vykdykite šią vartotojo komandinę komandą:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Vykdykite šią komandinę komandą, kad patvirtintumėte, kad ji įgalinta vartotojui:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Daugiau informacijos žr.:

- [Neriboto archyvavimo įgalinimas – administratoriaus žinynas – Microsoft 365 atitikties | "Microsoft" dokumentai](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online apribojimai – paslaugos aprašai | "Microsoft" dokumentai](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Versijos naujinimas į kitą verslo planą | "Microsoft" dokumentai](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

