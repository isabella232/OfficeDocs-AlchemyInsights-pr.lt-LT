---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052394"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

Windows Virtualusis darbalaukis (WVD) siūlo diagnostikos įrankį, kuris leidžia administratoriams identifikuoti klaidas naudojant vieną sąsają. Šis įrankis registruoja su diagnostika susijusią informaciją, kai WVD naudoja kas nors, kam priskirtas WVD vaidmuo. Kiekviename žurnale yra informacija apie WVD vaidmenį, kuris dalyvauja veikloje, klaidų pranešimus, rodomus seanso metu, ir informaciją apie nuomotoją ir vartotoją. "Azure Log Analytics" galima sukonfigūruoti taip, kad būtų užfiksuotas diagnostikos įrankio sukurtas veiklos žurnalas. Toliau nurodyta, kaip tai padaryti.

1. Sukurkite žurnalo analizės darbo sritį naudodami ["Azure" portalą](https://go.microsoft.com/fwlink/?linkid=2129500) arba ["Azure PowerShell".](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Prisijungimas Windows į "Azure Monitor".](https://go.microsoft.com/fwlink/?linkid=2129913) Gaukite darbo srities ID ir pirminį darbo srities raktą. Sąrankos vediklis turi šią informaciją tinkamai sukonfigūruoti agentą ir užtikrinti, kad jis galėtų bendrauti su "Azure Monitor".
1. [Stumkite diagnostikos duomenis į savo darbo sritį.](https://go.microsoft.com/fwlink/?linkid=2128284) Galite stumti diagnostikos duomenis iš savo WVD nuomotojo į darbo srities žurnalo analizę.
1. [Nustatykite ir diagnozuokite](https://go.microsoft.com/fwlink/?linkid=2128338) problemas, kurios yra vidinės arba išorinės WVD atžvilgiu.

Norėdami sužinoti daugiau apie WVD tarnybos diagnostikos įrankio konfigūravimą, [žr. Žurnalo analizės naudojimas diagnostikos funkcijai](https://go.microsoft.com/fwlink/?linkid=2128084).
