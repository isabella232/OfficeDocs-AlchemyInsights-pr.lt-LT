---
title: El. pašto profilių naudojimas su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555251"
---
# <a name="using-email-profiles-with-intune"></a>El. pašto profilių naudojimas su "Intune"

Intune gali būti naudojamas sukurti ir įdiegti el. pašto profilius gimtoji (built-in) el. pašto klientas keliose įrenginių platformose.

Informacijos apie kai kuriuos apribojimus, susijusius su el. pašto profiliais, įskaitant tai, kaip tvarkomi esami profiliai ir kaip pašalinti el. pašto profilius, rasite [El. pašto parametrų įtraukimas į įrenginius naudojant "Intune".](https://docs.microsoft.com/intune/email-settings-configure)

Jei norite gauti daugiau informacijos apie tai, kaip sukurti el. pašto profilius kiekvienai įrenginio platformai, žr.:

["Android" įrenginio nustatymai, norint konfigūruoti el. paštą, autentifikavimą ir sinchronizavimą "Intune"](https://docs.microsoft.com/intune/email-settings-android)  
["iOS" ir "iPadOS" įrenginių el. pašto parametrų įtraukimas programoje "Microsoft Intune"](https://docs.microsoft.com/intune/email-settings-ios)  
[El. pašto profilio parametrai programoje "Microsoft Intune" įrenginiuose, kuriuose veikia "Windows Phone 8.1"](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[El. pašto profilio parametrai įrenginiams, kuriuose veikia "Windows 10" programoje "Microsoft Intune"](https://docs.microsoft.com/intune/email-settings-windows-10)

**Dažna sinchronizavimo problema**

**"Knox" "Android" el. pašto profilyje neleidžia naudotojams sinchronizuoti kontaktų, kalendoriaus ir užduočių su naudotojo įrenginiais.**

"Knox" "Android KNOX" el. pašto profilyje administratoriui suteikiama galimybė nuspręsti, kurie turinio tipai sinchronizuojami su įrenginiu, nustatant kiekvieną įjungtą.

Jei kurio nors turinio tipo parametras nustatytas kaip **Nesukonfigūruotas** (numatytasis), tas turinio tipas automatiškai nesinchronizuojamas. Vartotojas gali įgalinti turinio tipą, kurio jis nori tiesiogiai įrenginyje, rankiniu būdu, bet šią konfigūraciją perrašo "Intune" strategijos parametras, o sinchronizavimas sustabdomas to turinio tipui.

