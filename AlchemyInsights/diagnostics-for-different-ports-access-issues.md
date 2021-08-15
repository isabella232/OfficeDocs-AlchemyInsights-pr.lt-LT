---
title: Skirtingų prievadų prieigos problemų diagnostika
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030910"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Skirtingų prievadų prieigos problemų diagnostika

Norėdami išspręsti skirtingas prievado prieigos problemas, atlikite šiuos veiksmus:

1. Sustabdykite / išskirstykite virtualiąją mašiną (VM) iš portalo, iš naujo paleiskite VM ir dar kartą patikrinkite. 
2. Patikrinkite VM tinklo parametrus, kad nustatytumėte, ar turite tinklo saugos grupių (NSGs) blokuojamą srautą. Taip pat galite naudoti tinklo stebėjimo priemonės [IP srauto](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) tikrinimo įrankį, kad patikrinsite, ar NSG blokuoja srautą, "User-Defined Routes" (UDR) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0) arba į tinklo įrenginį.
Jei išbandę anksčiau nurodytus veiksmus vis tiek kyla problemų, pateikite VM pavadinimą ir TCP prievadą, į kurį bandote siųsti laiškus, kad būtų galima atlikti tolesnę diagnostiką.

**Rekomenduojami dokumentai**

[Siuntimo el. laiškų siuntimo per 25 prievadą apribojimai ir rekomendacijos](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)