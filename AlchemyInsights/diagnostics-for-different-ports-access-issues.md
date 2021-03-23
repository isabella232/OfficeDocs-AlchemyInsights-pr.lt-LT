---
title: Įvairių prievadų prieigos trikčių diagnostika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035779"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Įvairių prievadų prieigos trikčių diagnostika

Norėdami išspręsti skirtingas prievadų prieigos problemas, atlikite šiuos veiksmus:

1. Stop/dealrasti virtualios mašinos (VM) iš portalo, iš naujo paleiskite VM ir bandykite dar kartą. 
2. Patikrinkite VM tinklo parametrus, kad nustatytumėte, ar turite tinklo saugos grupes (NSGs) blokuoja srautą. Taip pat galite naudoti [tinklo watcher IP srauto tikrinimo įrankį](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , kad patikrintumėte, ar yra nsgs blokavimas srauto, User-Defined maršrutų (udrs) nukreipia srautą atgal į vietinę ("Numatytasis maršrutas ' 0.0.0.0/0) arba tinklo Appliance.
Jei vis dar kyla problemų bandant atlikti anksčiau nurodytus veiksmus, pateikite VM pavadinimą ir TCP prievadą, kurį mėginate siųsti paštu tolesniam diagnozavimui.

**Rekomenduojami dokumentai**

[Siuntimo elektroninio pašto siuntimo per 25 prievadą apribojimai ir rekomendacijos](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)