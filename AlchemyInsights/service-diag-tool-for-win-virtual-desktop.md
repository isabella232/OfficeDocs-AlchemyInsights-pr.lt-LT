---
title: "\"Windows Virtual Desktop\" tarnybos diagnostikos įrankis"
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678625"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>"Windows Virtual Desktop" tarnybos diagnostikos įrankis

"Windows Virtual Desktop" (WVD) siūlo diagnostikos įrankį, leidžiantį administratoriams nustatyti klaidas per vieną sąsają. Šiame įrankyje yra su diagnostika susijusi informacija, kai "WVD" naudoja kas nors priskyrė "WVD" vaidmenį. Kiekviename logaritme yra informacijos apie "WVD" vaidmenį, susijusį su veikla, seanso metu rodomus klaidų pranešimus ir informaciją apie nuomotoją ir vartotoją. "Azure" žurnalų analizės galima sukonfigūruoti, kad būtų užfiksuoti veiklos registras, sukurtas diagnostikos įrankiu. Toliau nurodyta, kaip tai padaryti.

1. Sukurkite žurnalų analizės darbo sritį naudodami " [Azure" portalą](https://go.microsoft.com/fwlink/?linkid=2129500) arba " [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)".
1. [Prijunkite "Windows" kompiuterius prie "Azure Monitor"](https://go.microsoft.com/fwlink/?linkid=2129913). Gauti darbo srities ID ir savo darbo srities pirminį raktą. Sąrankos vediklyje reikia šios informacijos, kad būtų galima tinkamai sukonfigūruoti agentą ir užtikrinti, kad jis galėtų bendrauti su "Azure Monitor".
1. [Paspauskite diagnostikos duomenis į darbo sritį](https://go.microsoft.com/fwlink/?linkid=2128284). Galite stumti diagnostikos duomenis iš savo "WVD" nuomotojo prie savo darbo srities žurnalų analizės.
1. [Identifikuoti ir diagnozuoti](https://go.microsoft.com/fwlink/?linkid=2128338) vidines arba išorines problemas, susijusias su wvd.

Jei norite sužinoti daugiau apie "WVD" paslaugų diagnostikos įrankio konfigūravimą, žiūrėkite [diagnostikos funkcijai naudokite žurnalų analizės funkciją](https://go.microsoft.com/fwlink/?linkid=2128084).
