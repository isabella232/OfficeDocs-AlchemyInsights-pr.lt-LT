---
title: Klaida siunčiant laišką, blokuojamą "SpamHaus"
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783811"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d002a-102">Klaida siunčiant laišką: kliento pagrindinis kompiuteris užblokuotas naudojant "SpamHaus"</span><span class="sxs-lookup"><span data-stu-id="d002a-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d002a-103">Pranešimą išsiuntę IP adresas priklauso " [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245)" blokinio sąrašo blokams.</span><span class="sxs-lookup"><span data-stu-id="d002a-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d002a-104">Priežastys, dėl kurių užblokavo "SpamHaus", apima pažeistas paskyras, "kompromisus" kompiuterius, kuriuose yra viešasis IP adresas ir interneto paslaugų teikėjo (ISP) strategijos.</span><span class="sxs-lookup"><span data-stu-id="d002a-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d002a-105">Galimos pataisos:</span><span class="sxs-lookup"><span data-stu-id="d002a-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d002a-106">Norėdami užblokuoti gautinus laiškus, kur kontroliuojate šaltinio el. pašto serverį, turite nustatyti priežastį ir pašalinti bloką iš "SpamHaus" žiniatinklio svetainės.</span><span class="sxs-lookup"><span data-stu-id="d002a-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="d002a-107">Norėdami užblokuoti Gaunamųjų žinučių, kai šaltinio IP adresas priklauso kam nors kitam, adreso savininkui reikia pašalinti bloką iš "SpamHaus" svetainės.</span><span class="sxs-lookup"><span data-stu-id="d002a-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d002a-108">Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitokį statinį IP adresą arba pašalinti adresą iš PBL.</span><span class="sxs-lookup"><span data-stu-id="d002a-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="d002a-109">Jei norite užblokuoti siuntimo laišką iš domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei laiškai nukreipiami trečiosios šalies tarnyba.</span><span class="sxs-lookup"><span data-stu-id="d002a-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d002a-110">Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte blokuojamą IP adreso savininką.</span><span class="sxs-lookup"><span data-stu-id="d002a-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
