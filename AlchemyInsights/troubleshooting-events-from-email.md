---
title: Trikčių diagnostika įvykių el. paštu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569137"
---
# <a name="troubleshooting-events-from-email"></a>Trikčių diagnostika įvykių el. paštu

1. Patikrinkite, ar funkcija įgalinta pašto dėžutės: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Tada peržiūrėkite "Įvykiai iš el. pašto" žurnalus **Eksporto-MailboxDiagnosticLogs <mailbox> komponento TimeProfile**

3. Žurnaluose "Įvykiai iš el. pašto" raskite internetMessageId, kuris atitinka pašto dėžutės elementą.  

4. TrustScore nustato, ar elementas yra įtrauktas, ar ne. Įvykiai bus įtraukti tik tada, jei TrustScore = "Patikimas".

TrustScore nustatomas pagal SPF, Dkim arba Dmarc ypatybes, kurios yra pranešimo antraštėje.

Norėdami peržiūrėti šias ypatybes:

**Darbalaukio "Outlook"**

- Atidaryti elementą
- Failų > ypatybės – > interneto antraštės

Arba

**MFCMapi (Netoli viešbučio mfc)**

- Pereiti į aplanko Gauta elementą
- Ieškokite PR_TRANSPORT_MESSAGE_HEADERS_W

Šios savybės nustatomos ir registruojamos transportavimo ir maršruto parinkimo metu. Jei reikia daugiau trikčių šalinimo, gali tekti stebėti, kaip palaikymo tarnyba dėl SPF, DKIM ir.arba DMARC trikčių.