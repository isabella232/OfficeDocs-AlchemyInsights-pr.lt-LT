---
title: "\"Android\" įrenginių įtraukimo į \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759628"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>"Android" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas

Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.
  
Kai kurios dažniausios problemos ir sprendimo veiksmai:
  
 **Įrenginio neužšifruota klaida įmonės portale:** Naujesnėms "Android" versijoms, ypač pradedant v7.0, reikia paleisties kodą, kad įsitikintumėte, jog jūsų įrenginys yra visiškai užšifruotas. Įprasti sprendimai yra įgalinti paleisties smeigtuką arba visiškai užšifruoti įrenginį. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) jei norite gauti daugiau informacijos.
  
 **Įrenginiai nepavyksta patikrinti su Intune paslauga arba rodyti kaip "Nesveika" Intune administratoriaus konsolėje:** Kai kurie "Samsung 4.4" ir "5.5" įrenginiai gali netikrinti paslaugos. Yra 3 galimi šios problemos sprendimai:
  
1. Rankiniu būdu atidarykite "Intune" įmonės portalo programą, kuri automatiškai pradės įrenginio sinchronizavimą.

2. Atnaujinkite įrenginį į 6.0 ar naujesnę "Android".

3. Išjunkite "Samsung Smart Manager" nuo "Intune" įmonės portalo valdymo. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) jei reikia daugiau informacijos šiais klausimais ir sprendimais.

 **Vartotojo licencijos tipas neleistinas** arba **vartotojo vardas neatpažintas klaida:** vartotojui reikia priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją per: "Office" administravimo centras arba "Azure" portalas.
  
Papildomi ištekliai, padėsiantys išspręsti problemą:
  
1. Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos.

2. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) kuriame pateikiamas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir priimti sprendimai kiekvienam, sąrašas.

3. [Sužinokite, kaip užregistruoti "Android" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/android-enroll)
