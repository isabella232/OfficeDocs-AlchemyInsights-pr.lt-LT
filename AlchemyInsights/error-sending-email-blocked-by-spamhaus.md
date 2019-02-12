---
title: Klaida siunčiant laišką užblokavo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912356"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Klaida siunčiant laišką: kliento kompiuterio blokuoti naudojant Spamhaus

IP adresą, kuris siunčiamas pranešimas yra blokuojamų svetainių sąrašą, priklausanti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Priežastis yra užblokuotas Spamhaus pavojus apima pažeista mašinos viešasis IP adresas, ir interneto paslaugų teikėjo (ISP) politiką. Galimus sprendimus yra:
  
- Užblokuotų gaunamų pranešimų į "Office 365", kur jums kontroliuoti šaltinio el. pašto serverio, jums reikia nustatyti priežastis ir pašalinti blokas iš Spamhaus interneto svetainėje.
    
- Užblokuotų gaunamų pranešimų į "Office 365", kai šaltinio IP adresas priklauso kam nors kitam, adresas savininkas turi pašalinti blokas iš Spamhaus svetainėje. Jei IP adresas su politikos blokas sąrašą (PBL), savininkas gali paskirti kitą statinį IP adresą arba pašalinti adresą iš to PBL.
    
- Užblokuotų siunčiamų pranešimų iš "Office 365" domeno, galite gauti šį klaidos jei pranešimai yra nukreipiami per 3rd party paslaugų. WHOIS paieškos įrankį galite rasti blokuojamų IP adresų savininkas.
    

