---
title: Trikčių šalinimas naudojant "Microsoft Intune" "Android" įrenginius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689962"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Trikčių šalinimas naudojant "Microsoft Intune" "Android" įrenginius

Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar.
  
Kai kurios Dažniausios problemos ir sprendimo veiksmai:
  
 **Įrenginio neužšifruota klaida įmonės portale:** Naujesnės "Android" versijos, ypač pradedant nuo v 7.0, reikalauja paleisties slaptojo kodo, kad įsitikintumėte, jog jūsų įrenginys visiškai šifruotas. Įprasti sprendimai yra įgalinti paleisties PIN arba visiškai užšifruoti įrenginį. Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Įrenginių nepavyksta patikrinti naudojant Intune tarnybą arba Rodyti kaip "nesveika" Intune administravimo konsolėje:** Kai kurie "Samsung" 4,4 ir "5,5" įrenginiai gali netikrinti tarnybos. Yra 3 galimi šios problemos sprendimo būdai:
  
1. Neautomatiškai atidarykite "Intune" įmonės portalo programą, kuri automatiškai pradės įrenginio sinchronizavimą.

2. Atnaujinkite įrenginį į "Android" 6,0 arba naujesnę versiją.

3. Išjunkite "Samsung Smart Manager" naudodami "Intune" įmonės portalą. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , kad sužinotumėte daugiau apie šias problemas ir rezoliucijas.

 **Vartotojo licencijos tipas neleistinas** arba **vartotojo vardas neatpažinta klaida:** vartotojui reikia priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją naudodami: "Office" administravimo centras arba "Azure" portalas.
  
Papildomi ištekliai, padėsiantys išspręsti problemą:
  
1. Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau.

2. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , kad būtų dažnai pasitaikančių klaidų, neleidžiančių atlikti įtraukimo ir sprendimų, sąrašas.

3. [Sužinokite, kaip užregistruoti "Android" įrenginius programoje "Microsoft Intune"](https://docs.microsoft.com/intune/android-enroll).
