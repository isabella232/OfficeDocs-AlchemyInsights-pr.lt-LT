---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "Android" įrenginių
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655891"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Šalinkite triktis naudodami werbowania į Microsoft Intune "Android" įrenginių

Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai.
  
Kai kurios Dažnos problemos ir sprendimo veiksmai:
  
 **Prietaisas nėra šifruojami klaida įmonės portale:** Naujesnių versijų "Android", ypač pradedant v7.0, reikalauja paleisties kodą, norėdami įsitikinti, kad jūsų įrenginys yra visiškai iššifruoti. Bendri sprendimai yra įgalinti paleisties pin arba visiškai šifruoti prietaiso. Peržiūrėti [šio dokumento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dėl daugiau informacijos. 
  
 **Įrenginių nesugeba patikrinti su Intune tarnyba arba Rodyti kaip "Nesveiko" Intune administratoriaus konsolėje:** Kai kurios "Samsung" 4.4 ir 5.5 įrenginiai negali tikrinti ir eksploatuoti. Yra 3 galimi siekiant šią problemą: 
  
1. Rankiniu būdu atidaryti Intune įmonės portalo programą, kuri bus automatiškai pradėti įrenginio sinchronizavimą.
    
2. Atnaujinti įrenginio į "Android" 6.0 arba naujesnė.
    
3. Išjungti Samsung Smart Manager valdymo Intune įmonės portalas. Peržiūrėti daugiau informacijos apie šios problemos ir sprendimai [šiame dokumente](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) . 
    
 **Vartotojo licencijos tipas neteisingas** arba **vartotojo vardas nėra atpažįstamas klaida:** vartotojas turi priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus priskirti licenciją per: Office administravimo centro arba Azure portalas. 
  
Papildomų išteklių, kurie padės išspręsti jūsų problemą:
  
1. Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių. Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Peržiūrėti [šį dokumentą](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą. 
    
3. [Sužinokite, kaip Registruotis "Android" įrenginius į Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

