---
title: Klaida siunčiant laišką užblokuotas SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714266"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="7b654-102">Klaida siunčiant el. laišką: Kliento pagrindinis kompiuteris užblokuotas naudojant "Spamhaus"</span><span class="sxs-lookup"><span data-stu-id="7b654-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="7b654-103">IP adresas, kuris išsiuntė pranešimą, yra blokų sąraše, priklausančiame ["Spamhaus".](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="7b654-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="7b654-104">Nepageidaujamo e. Paštas yra užblokuotos paskyros, įkompromisiniai įrenginiai, bendrinami viešuoju IP adresu, ir interneto paslaugų teikėjo (ISP) strategijos.</span><span class="sxs-lookup"><span data-stu-id="7b654-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="7b654-105">Galimi pataisymai yra:</span><span class="sxs-lookup"><span data-stu-id="7b654-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="7b654-106">Užblokuotiems gaunamiems pranešimams, kuriuose valdote šaltinio el. pašto serverį, turite nustatyti priežastį ir pašalinti bloką iš "Spamhaus" svetainės.</span><span class="sxs-lookup"><span data-stu-id="7b654-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="7b654-107">Užblokuotiems gaunamiems pranešimams, kuriuose šaltinio IP adresas priklauso kam nors kitam, adreso savininkas turi pašalinti bloką iš "Spamhaus" svetainės.</span><span class="sxs-lookup"><span data-stu-id="7b654-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="7b654-108">Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitą statinį IP adresą arba pašalinti adresą iš PBL.</span><span class="sxs-lookup"><span data-stu-id="7b654-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="7b654-109">Užblokuotų siunčiamų pranešimų iš domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei pranešimai nukreipiami per trečiosios šalies tarnybą.</span><span class="sxs-lookup"><span data-stu-id="7b654-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="7b654-110">Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte užblokuotą IP adreso savininką.</span><span class="sxs-lookup"><span data-stu-id="7b654-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
