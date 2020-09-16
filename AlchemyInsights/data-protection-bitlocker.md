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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731247"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo su "Intune" įgalinimas

 "Intune Endpoint Protection" strategiją galima naudoti konfigūruojant "BitLocker" šifravimo parametrus "Windows" įrenginiuose. Daugiau informacijos rasite ["Windows 10" (ir vėlesnės versijos) parametruose, kad apsaugotumėte įrenginius naudodami Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos. Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti. Daugiau informacijos rasite toliau pateiktuose DUK.
 
Informacijos apie "BitLocker" problemų diagnostiką ieškokite ["BitLocker" strategijų trikčių diagnostika "Microsoft Intune"](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**DUK**

 K: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant galinio punkto apsaugos strategiją?<br>
 A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant ["BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi "Windows" leidimai arba komponavimo versijos palaiko "BitLocker" CSP. <br><br>
      Šiuo metu palaikomi šie "Windows" leidimai: "Enterprise", "Education", mobilusis, mobiliųjų įrenginių įmonė ir profesionalai (1809 Komponavimo versija ir vėlesnė versija).
 
K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai "BitLocker" yra šifravimo metodo ir šifro stiprumo parametrai (XTS-AES – 128), pritaikys strategiją su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?<br>
A.: Ne. Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.<br><br>
**Pastaba:** "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta Intune strategija, kuri leidžia naudoti strategijos parametrus, naudojamus vietoj OS numatytųjų reikšmių.
 
K: Jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?<br>
A: su šifravimu susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.
 
K: Kodėl Intune atitikties strategija rodo, kad mano įrenginyje nėra įgalintas "BitLocker", net jei jis yra?<br>
A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą. Šis klientas tik matuoja įrenginio būseną įkrovimo metu. Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.
 
 