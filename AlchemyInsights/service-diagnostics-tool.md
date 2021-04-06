---
title: Tarnybos diagnostikos įrankis, skirtas "Windows Virtual Desktop"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595866"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Tarnybos diagnostikos įrankis, skirtas "Windows Virtual Desktop"

"Windows Virtual Desktop" (WVD) siūlo diagnostikos įrankį, kuris leidžia administratoriams identifikuoti klaidas naudojant vieną sąsają. Šis įrankis registruoja su diagnostika susijusią informaciją, kai WVD naudoja kas nors, kam priskirtas WVD vaidmuo. Kiekviename žurnale yra informacija apie WVD vaidmenį, kuris dalyvauja veikloje, klaidų pranešimus, rodomus seanso metu, ir informaciją apie nuomotoją ir vartotoją. "Azure Log Analytics" galima sukonfigūruoti užfiksuoti diagnostikos įrankio sukurtą veiklos žurnalą, atlikdami šiuos veiksmus:

1. Sukurkite žurnalo analizės darbo sritį naudodami ["Azure" portalą](https://go.microsoft.com/fwlink/?linkid=2129500) arba ["Azure PowerShell".](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Prijunkite "Windows" kompiuterius prie "Azure Monitor".](https://go.microsoft.com/fwlink/?linkid=2129913) Gaukite darbo srities ID ir pirminį darbo srities raktą. Sąrankos vediklis turi šią informaciją tinkamai sukonfigūruoti agentą ir užtikrinti, kad jis galėtų bendrauti su "Azure Monitor".

1. [Stumkite diagnostikos duomenis į savo darbo sritį.](https://go.microsoft.com/fwlink/?linkid=2128284) Galite stumti diagnostikos duomenis iš savo WVD nuomotojo į darbo srities žurnalo analizę.

1. [Nustatykite ir diagnozuokite](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas, kurios yra vidinės arba išorinės WVD atžvilgiu.

Norėdami sužinoti daugiau apie WVD tarnybos diagnostikos įrankio konfigūravimą, žr. Žurnalo analizės naudojimas diagnostikos funkcijai.