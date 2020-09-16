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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653296"
---
# <a name="using-email-profiles-with-intune"></a>El. pašto profilių naudojimas su "Intune"

Intune gali būti naudojama kuriant ir diegiant "Native" (įtaisytąjį) elektroninio pašto klientą keliuose įrenginių platformose.

Informacijos apie kai kuriuos apribojimus, susijusius su pašto profiliais, įskaitant tai, kaip tvarkomi esami profiliai ir kaip pašalinti el. pašto profilius, rasite skyriuje [įtraukti el. pašto parametrus į įrenginius](https://docs.microsoft.com/intune/email-settings-configure), kuriuose naudojamas "Intune".

Daugiau informacijos apie tai, kaip kurti el. pašto profilius kiekvienai įrenginių platformai, ieškokite:

["Android" įrenginio parametrai, kad sukonfigūruotumėte elektroninio pašto, autentifikavimo ir sinchronizavimo "Intune"](https://docs.microsoft.com/intune/email-settings-android)  
["Microsoft Intune" "iOS" ir "iPadOS" įrenginių el. pašto parametrų įtraukimas](https://docs.microsoft.com/intune/email-settings-ios)  
["Microsoft Intune" el. pašto profilio parametrai įrenginiams, kuriuose veikia "Windows Phone" 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
["Microsoft Intune" įrenginių, kuriuose veikia "Windows 10", el. pašto profilio parametrai](https://docs.microsoft.com/intune/email-settings-windows-10)

**Įprastas sinchronizavimo klausimas**

**KNOX, esanti "Android" el. pašto profilyje, apsaugo vartotojų kontaktus, kalendorių ir užduotis, kad nebūtų sinchronizuojama su vartotojų įrenginiais.**

KNOX "Android KNOX" elektroninio pašto profilyje suteikia administratoriui galimybę nuspręsti, kurie turinio tipai yra sinchronizuojami su įrenginiu, nustatydami kiekvieną įgalintą.

Jei bet kurio turinio tipo parametras nustatytas kaip **nesukonfigūruotas** (numatytasis parametras), turinio tipas nesinchronizuojamas automatiškai. Vartotojas gali įgalinti turinio tipą, kurį jie nori naudoti tiesiogiai įrenginyje, tačiau ši konfigūracija perrašoma iš "Intune" strategijos parametro ir šio turinio tipo sinchronizavimo sustoja.

