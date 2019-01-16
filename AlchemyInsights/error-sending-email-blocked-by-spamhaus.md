---
title: Klaida siunčiant laišką užblokavo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301997"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="03872-102">Klaida siunčiant laišką: kliento kompiuterio blokuoti naudojant Spamhaus</span><span class="sxs-lookup"><span data-stu-id="03872-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="03872-p101">IP adresą, kuris siunčiamas pranešimas yra blokuojamų svetainių sąrašą, priklausanti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Priežastis yra užblokuotas Spamhaus pavojus apima pažeista mašinos viešasis IP adresas, ir interneto paslaugų teikėjo (ISP) politiką. Galimus sprendimus yra:</span><span class="sxs-lookup"><span data-stu-id="03872-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="03872-106">Užblokuotų gaunamų pranešimų į "Office 365", kur jums kontroliuoti šaltinio el. pašto serverio, jums reikia nustatyti priežastis ir pašalinti blokas iš Spamhaus interneto svetainėje.</span><span class="sxs-lookup"><span data-stu-id="03872-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="03872-p102">Užblokuotų gaunamų pranešimų į "Office 365", kai šaltinio IP adresas priklauso kam nors kitam, adresas savininkas turi pašalinti blokas iš Spamhaus svetainėje. Jei IP adresas su politikos blokas sąrašą (PBL), savininkas gali paskirti kitą statinį IP adresą arba pašalinti adresą iš to PBL.</span><span class="sxs-lookup"><span data-stu-id="03872-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="03872-p103">Užblokuotų siunčiamų pranešimų iš "Office 365" domeno, galite gauti šį klaidos jei pranešimai yra nukreipiami per 3rd party paslaugų. WHOIS paieškos įrankį galite rasti blokuojamų IP adresų savininkas.</span><span class="sxs-lookup"><span data-stu-id="03872-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

