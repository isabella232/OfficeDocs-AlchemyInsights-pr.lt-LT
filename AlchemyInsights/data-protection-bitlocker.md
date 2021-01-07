---
title: "\"DataProtection\" – \"BitLocker\""
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778201"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo su "Intune" įgalinimas

"Intune Endpoint Protection" strategiją galima naudoti konfigūruojant "BitLocker" šifravimo parametrus "Windows" įrenginiuose. Daugiau informacijos rasite ["Windows 10" (ir vėlesnės versijos) parametruose, kad apsaugotumėte įrenginius naudodami Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Be galinio punkto apsaugos strategijos taip pat yra šifravimo ataskaita, kurioje pateikiamas išsamesnis įrenginių šifravimo būsenos rodinys. Šią ataskaitą galima pasiekti iš MEM portalo dalyje **įrenginiai > monitorius**, tada dalyje **konfigūracija** pasirinkite [šifravimo ataskaita](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jei pastebėsite, kad "BitLocker" nepavyksta įgalinti, kaip tikėtasi, arba kad "BitLocker" įgalinimas naudojamas profilis yra klaidos būsenos, peržiūrėkite šifruotės ataskaitą, kad geriau suprastumėte, kodėl vyksta veikimas.

Norėdami rasti išsamios informacijos apie tai, kaip interpretuoti ataskaitą, įskaitant įvairias šifravimo būsenas, žiūrėkite [įrenginių šifravimo su "Intune" stebėjimas](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos. Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti. Daugiau informacijos rasite toliau pateiktuose DUK.

Informacijos apie "BitLocker" problemų diagnostiką ieškokite ["BitLocker" strategijų trikčių diagnostika "Microsoft Intune"](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**DUK**

K: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant galinio punkto apsaugos strategiją?<br>
A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant ["BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi "Windows" leidimai arba komponavimo versijos palaiko "BitLocker" CSP. <br><br>

K: kaip "BitLocker" galima įjungti įrenginiuose be galutinio vartotojo veiksmo?<br>
A: tol, kol bus įvykdytos būtinos prielaidos, galima įjungti "BitLocker" tylųjį šifravimą per Intune. Peržiūrėkite išsamią informaciją apie įrenginio reikalavimus ir pavyzdinius strategijos parametrus, kad būtų įgalintas tylus šifravimas šiame doc: [tyliai įjunkite "BitLocker" šifravimą](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai "BitLocker" yra šifravimo metodo ir šifro stiprumo parametrai (XTS-AES – 128), pritaikys strategiją su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?<br>
A.: Ne. Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.<br><br>
**Pastaba:** "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta Intune strategija, kuri leidžia naudoti strategijos parametrus, naudojamus vietoj OS numatytųjų reikšmių.
 
K: Jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?<br>
A: su šifravimu susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.
 
K: Kodėl Intune atitikties strategija rodo, kad mano įrenginyje nėra įgalintas "BitLocker", net jei jis yra?<br>
A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą. Šis klientas tik matuoja įrenginio būseną įkrovimo metu. Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.
 
 