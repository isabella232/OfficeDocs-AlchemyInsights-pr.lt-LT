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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Klaida siunčiant laišką: kliento pagrindinis kompiuteris užblokuotas naudojant "SpamHaus"

Pranešimą išsiuntę IP adresas priklauso " [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245)" blokinio sąrašo blokams. Priežastys, dėl kurių užblokavo "SpamHaus", apima pažeistas paskyras, "kompromisus" kompiuterius, kuriuose yra viešasis IP adresas ir interneto paslaugų teikėjo (ISP) strategijos. Galimos pataisos:
  
- Norėdami užblokuoti gautinus laiškus, kur kontroliuojate šaltinio el. pašto serverį, turite nustatyti priežastį ir pašalinti bloką iš "SpamHaus" žiniatinklio svetainės.

- Norėdami užblokuoti Gaunamųjų žinučių, kai šaltinio IP adresas priklauso kam nors kitam, adreso savininkui reikia pašalinti bloką iš "SpamHaus" svetainės. Jei IP adresas yra strategijos blokų sąraše (PBL), savininkas gali priskirti kitokį statinį IP adresą arba pašalinti adresą iš PBL.

- Jei norite užblokuoti siuntimo laišką iš domeno, prijungto prie "Microsoft", galite gauti šią klaidą, jei laiškai nukreipiami trečiosios šalies tarnyba. Galite naudoti WHOIS peržvalgos įrankį, kad rastumėte blokuojamą IP adreso savininką.
