---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815623"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo įgalinimas naudojant "Intune"

"Intune Endpoint Protection" strategiją galima naudoti "BitLocker" šifravimo parametrams konfigūruoti "Windows" įrenginiuose. Daugiau informacijos žr. ["Windows 10" (ir naujesnės versijos) parametrai, skirti įrenginiams apsaugoti naudojant "Intune".](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Be galinio punkto apsaugos strategijos, taip pat yra šifravimo ataskaita, kurioje pateikiamas išsamesnis įrenginių šifravimo būsenos rodinys. Šią ataskaitą galima pasiekti iš MEM portalo dalyje Įrenginiai **> Monitorius**, tada dalyje **Konfigūravimas** pasirinkite [Šifravimo ataskaita](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jei pastebėsite, kad nepavyksta įgalinti "BitLocker" kaip tikėtasi arba profilis, naudojamas "Bitlocker" įgalinti, yra klaidos būsenos, peržiūrėkite šifravimo ataskaitą, kad geriau suprastumėte, kodėl vyksta veikimas.

Norėdami rasti išsamios informacijos, kaip interpretuoti ataskaitą, įskaitant įvairias šifravimo būsenos reikšmes, žr. [Įrenginio šifravimo stebėjimas naudojant "Intune".](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos. Tai gali turėti įtakos strategijos taikymui, jei sukonfigūruoti ne numatytieji parametrai. Daugiau informacijos žr. toliau pateiktame DUK.

Informacijos apie "BitLocker" trikčių diagnostiką žr. ["BitLocker" strategijų trikčių šalinimas "Microsoft Intune".](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**DUK**

K: Kurie "Windows" palaikymo įrenginių šifravimo leidimai naudojant galinio punkto apsaugos strategiją?<br>
A: "Intune Endpoint Protection" strategijos parametrai įgyvendinami naudojant ["BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi "Windows" leidimai arba komponavimo versijos palaiko "BitLocker" CSP. <br><br>

K: Kaip galima įgalinti "BitLocker" įrenginiuose nereikalaujant galutinio vartotojo sąveikos?<br>
A: Kol bus įvykdytos būtinos būtinos sąlygos, galima įjungti "Bitlocker" "Silent Encryption" per "Intune". Peržiūrėkite išsamią informaciją apie įrenginio reikalavimus ir strategijos parametrų pavyzdžius, kad įgalintumėte tylų šifravimą šiame dokumente: [Tyliai įgalinkite "BitLocker" šifravimą](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

K: Jei įrenginys jau užšifruotas naudojant "BitLocker" naudojant numatytuosius OS šifravimo metodo parametrus ir šifravimo stiprumą (XTS-AES-128), ar taikant strategiją su skirtingais parametrais, automatiškai įjungiamas disko šifravimas iš naujo naudojant naujus parametrus?<br>
A.: Ne. Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti diską.<br><br>
**Pastaba:** Įrenginių, kurie yra užregistruoti naudojant "Autopilot", automatinis šifravimas, kuris būtų OOBE metu, nebus paleidžiamas, kol nebus įvertinta "Intune" strategija, todėl strategijos pagrindu pagrįstus parametrus galima naudoti vietoje OS numatytųjų reikšmių.
 
K: jei įrenginys užšifruotas dėl "Intune" strategijos taikymo, ar jis bus iššifruotas, kai ši strategija bus pašalinta?<br>
A: Pašalinus su šifravimu susijusią strategiją, iššifruoti nekonfigūruoti diskai.
 
K: kodėl "Intune" atitikties strategija rodo, kad mano įrenginyje neįgalinta "BitLocker", nors ji įjungta?<br>
A: "Bitlocker enabled" parametras "Intune" atitikties politikoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHR) klientą. Šis klientas įrenginio būseną tik įkelia metu. Taigi, jei įrenginys nebuvo paleistas iš naujo, nes "BitLocker" šifravimas buvo baigtas, DHR kliento tarnyba neinsins apie "BitLocker" kaip aktyvią.
 
 