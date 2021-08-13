---
title: "\"Android\" įrenginių registracijos \"\"Microsoft Intune\""
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008086"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>"Android" įrenginių registracijos ""Microsoft Intune"

Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.
  
Kai kurios dažniausios problemos ir sprendimo veiksmai:
  
 **Įrenginyje šifruota klaida Company Portal:** Naujesnėms "Android" versijoms, ypač pradedant nuo v7.0, reikalingas paleisties slaptasis kodas, kad įsitikintumėte, jog jūsų įrenginys visiškai užšifruotas. Bendrieji sprendimai yra įjungti paleisties smeigtuką arba visiškai šifruoti įrenginį. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) jei reikia daugiau informacijos.
  
 **Įrenginiams nepavyksta prisijungti naudojant "Intune" tarnybą arba "Intune" administravimo konsolėje rodyti kaip "Nesveika":** Kai kurie "Samsung 4.4" ir "5.5" įrenginiai gali nepatikrinti paslaugos. Yra 3 galimi šios problemos sprendimai:
  
1. Rankiniu būdu atidarykite Intune Company Portal programą, kuri automatiškai inicijuoja įrenginio sinchronizavimą.

2. Atnaujinkite įrenginį į "Android 6.0" arba naujesnė versija.

3. Išjunkite "Samsung Smart Manager" Intune Company Portal. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) jei reikia daugiau informacijos apie šias problemas ir sprendimą.

 **Klaida Vartotojo licencijos tipas** **netinkamas arba Vartotojo** vardas neatpažintas: vartotojui turi būti priskirta "Intune" arba EMS licencija. Peržiūrėkite šiuos dokumentus ir priskirkite licenciją naudodami: Office administravimo centrą arba "Azure" portalą.
  
Papildomi ištekliai, kurie padės išspręsti problemą:
  
1. Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.

2. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) kad peržiūrėtumėte dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieną iš jų, sąrašą.

3. [Sužinokite, kaip užregistruoti "Android" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/android-enroll)
