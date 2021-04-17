---
title: "\"Android\" įrenginių registracijos \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830950"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>"Android" įrenginių registracijos "Microsoft Intune" trikčių šalinimas

Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.
  
Kai kurios dažniausios problemos ir sprendimo veiksmai:
  
 **Įrenginio nešifruota klaida įmonės portale:** Naujesnėms "Android" versijoms, ypač pradedant nuo v7.0, reikalingas paleisties slaptasis kodas, kad įsitikintumėte, jog jūsų įrenginys visiškai užšifruotas. Bendrieji sprendimai yra įjungti paleisties smeigtuką arba visiškai šifruoti įrenginį. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) jei reikia daugiau informacijos.
  
 **Įrenginiams nepavyksta prisijungti naudojant "Intune" tarnybą arba "Intune" administravimo konsolėje rodyti kaip "Nesveika":** Kai kurie "Samsung 4.4" ir "5.5" įrenginiai gali nepatikrinti paslaugos. Yra 3 galimi šios problemos sprendimai:
  
1. Rankiniu būdu atidarykite "Intune" įmonės portalo programą, kuri automatiškai inicijuoja įrenginio sinchronizavimą.

2. Atnaujinkite įrenginį į "Android 6.0" arba naujesnė versija.

3. Išjunkite "Samsung Smart Manager" nuo "Intune" įmonės portalo valdymo. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) jei reikia daugiau informacijos apie šias problemas ir sprendimą.

 **Klaida Vartotojo licencijos tipas** **netinkamas arba Vartotojo** vardas neatpažintas: vartotojui turi būti priskirta "Intune" arba EMS licencija. Peržiūrėkite šiuos dokumentus ir priskirkite licenciją per: "Office" administravimo centrą arba "Azure" portalą.
  
Papildomi ištekliai, kurie padės išspręsti problemą:
  
1. Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.

2. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) kad peržiūrėtumėte dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieną iš jų, sąrašą.

3. [Sužinokite, kaip užregistruoti "Android" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/android-enroll)
