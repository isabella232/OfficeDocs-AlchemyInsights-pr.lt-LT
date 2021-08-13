---
title: El. pašto profilių naudojimas su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919431"
---
# <a name="using-email-profiles-with-intune"></a>El. pašto profilių naudojimas su "Intune"

"Intune" galima naudoti kuriant ir diegiant vietinių (įtaisytųjų) el. pašto klientų el. pašto profilius keliose įrenginių platformose.

Informacijos apie kai kuriuos su el. pašto profiliais susijusius apribojimus, įskaitant esamų profilių buvimo įvertinimą ir el. pašto profilių šalinimą, žr. El. pašto parametrų įtraukimas į įrenginius naudojant ["Intune".](https://docs.microsoft.com/intune/email-settings-configure)

Daugiau informacijos apie tai, kaip kurti el. pašto profilius kiekvienoje įrenginio platformoje, žr.:

["Android" įrenginio parametrai, kad sukonfigūruotų el. paštą, autentifikavimą ir sinchronizavimą "Intune"](https://docs.microsoft.com/intune/email-settings-android)  
["iOS" ir "iPadOS" įrenginių el. pašto parametrų įtraukimas programoje ""Microsoft Intune"](https://docs.microsoft.com/intune/email-settings-ios)  
[El. pašto profilio parametrai "Microsoft Intune" įrenginiuose, kuriuose veikia "Windows Phone" 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[El. pašto profilio parametrai įrenginiams, Windows 10 veikia "Microsoft Intune"](https://docs.microsoft.com/intune/email-settings-windows-10)

**Dažna sinchronizavimo problema**

**KNOX "Android" el. pašto profilyje neleidžia vartotojo kontaktams, kalendoriui ir užduotims sinchronizuoti su vartotojų įrenginiais.**

KNOX "Android KNOX" el. pašto profilyje administratoriui suteikia galimybę nuspręsti, kurie turinio tipai bus sinchronizuojami su įrenginiu, kiekvieną nustačius kaip įgalinusį.

Jei bet kurio turinio tipo parametras  nustatytas kaip Nesukonfigūruotas (numatytasis), turinio tipas nėra sinchronizuojamas automatiškai. Vartotojas gali įgalinti norimą turinio tipą tiesiogiai įrenginyje rankiniu būdu, tačiau tą konfigūraciją perrašo strategijos parametras "Intune", o sinchronizavimo su tuo turinio tipu sustoja.

