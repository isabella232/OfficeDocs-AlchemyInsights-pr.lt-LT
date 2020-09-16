---
title: Trikčių šalinimo įvykiai iš elektroninio pašto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658742"
---
# <a name="troubleshooting-events-from-email"></a>Trikčių šalinimo įvykiai iš elektroninio pašto

1. Patikrinkite, ar įgalinta pašto dėžutės funkcija: **get-Eventsofromemailconfiguration – tapatybė <mailbox> **

2. Tada Pažvelkite į "įvykiai iš pašto" žurnalai **Export-MailboxDiagnosticLogs <mailbox> -komponento timeprofile**

3. Žurnaluose "įvykiai iš pašto" raskite InternetMessageId, atitinkantį elementą pašto dėžutėje.  

4. TrustScore nustato, ar elementas įtrauktas, ar ne. Įvykiai bus įtraukti tik jei TrustScore = "patikimas".

TrustScore nustatomas pagal SPF, DKIM arba DMARC ypatybes, kurios yra pranešimo antraštėje.

Norėdami peržiūrėti šias ypatybes:

**Kompiuterio "Outlook"**

- Atidaryti elementą
- Failų > ypatybės – > interneto antraštės

arba

**MFCMapi**

- Pereiti į aplanko Gauta elementą
- Ieškoti PR_TRANSPORT_MESSAGE_HEADERS_W

Šios ypatybės nustatomos ir registruojamos transportavimo ir nukreipimo metu. Norėdami gauti daugiau trikčių diagnostikos, jums gali tekti stebėti transportavimo palaikymą apie NPN, DKIM ir. or DMARC gedimus.