---
title: Įvykių trikčių šalinimas iš el. pašto
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834847"
---
# <a name="troubleshooting-events-from-email"></a>Įvykių trikčių šalinimas iš el. pašto

1. Patikrinkite, ar įgalinta pašto dėžutės funkcija: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Tada peržiūrėkite žurnalus "Įvykiai iš el. pašto" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Žurnaluose "Įvykiai iš el. pašto" raskite "InternetMessageId", kuris atitinka pašto dėžutės elementą.  

4. Patikimumo įvertinimą nustato, ar elementas yra įtrauktas, ar ne. Įvykiai bus įtraukti tik tada, jei TrustScore = "Patikimas".

Patikimumo įvertinimą nustato SPF, Dkim arba Dmarc ypatybės, kurios yra laiško antraštėje.

Norėdami peržiūrėti šias ypatybes:

**Darbalaukio "Outlook"**

- Atidaryti elementą
- File -> Properties -> Internet Headers

arba

**MFCMapi**

- Pereiti prie aplanko Gauta elemento
- Ieškokite PR_TRANSPORT_MESSAGE_HEADERS_W

Šios ypatybės nustatomos ir įrašomos transportavimo ir nukreipimo metu. Jei norite gauti daugiau trikčių šalinimo, gali tekti stebėti transportavimo palaikymą dėl SPF, DKIM ir.arba DMARC trikčių.