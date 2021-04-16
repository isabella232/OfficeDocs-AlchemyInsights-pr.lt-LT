---
title: Klaida siunčiant el. laiškus, užblokuotus "SpamHaus"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813732"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3bca1-102">Klaida siunčiant el. laišką: kliento pagrindinis kompiuteris užblokuotas naudojant "Spamhaus"</span><span class="sxs-lookup"><span data-stu-id="3bca1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3bca1-103">Pranešimą išsiuntęs IP adresas yra blokų sąraše, kuris priklauso ["Spamhaus".](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="3bca1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3bca1-104">"Spamhaus" blokavimo priežastys apima pažeistas paskyras, pažeistus įrenginius, kurie bendrina viešąjį IP adresą, ir interneto paslaugų teikėjo (ISP) strategijas.</span><span class="sxs-lookup"><span data-stu-id="3bca1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3bca1-105">Galimi pataisymai:</span><span class="sxs-lookup"><span data-stu-id="3bca1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3bca1-106">Užblokuotų gaunamų pranešimų, kuriuose valdote šaltinio el. pašto serverį, atveju turite nustatyti priežastį ir pašalinti bloką iš "Spamhaus" svetainės.</span><span class="sxs-lookup"><span data-stu-id="3bca1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3bca1-107">Blokuojamų gaunamų pranešimų, kurių šaltinio IP adresas priklauso kam nors kitam, atveju adreso savininkas turi pašalinti bloką iš "Spamhaus" svetainės.</span><span class="sxs-lookup"><span data-stu-id="3bca1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3bca1-108">Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitą statinį IP adresą arba pašalinti adresą iš PBL.</span><span class="sxs-lookup"><span data-stu-id="3bca1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3bca1-109">Jei blokuojami siunčiami pranešimai iš jūsų domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei pranešimai nukreipiami per trečiosios šalies tarnybą.</span><span class="sxs-lookup"><span data-stu-id="3bca1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3bca1-110">Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte užblokuotą IP adreso savininką.</span><span class="sxs-lookup"><span data-stu-id="3bca1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
