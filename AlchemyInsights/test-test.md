---
title: "\"SharePoint Online\" terminų saugyklos sąlygos"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750459"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo su "Intune" įgalinimas

"Intune Endpoint Protection" strategiją galima naudoti norint sukonfigūruoti "Windows" įrenginių Boitlocker šifravimo parametrus, kaip aprašyta: Windows10 (ir vėlesni) parametrai, skirti apsaugoti įrenginius naudojant Intune

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos. Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti. Išsamiau žr DUK.


DUK   k: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant Endpoint Protection strategiją?
 A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant "BitLocker" CSP.Ne visi leidimai ir "Windows" komponavimo versijos nepalaiko "BitLocker" CSP. 
      Šiuo metu "Windows" leidimuose: Enterprise; Švietimo, mobilioji, mobilioji įmonė ir specialistas (1809 komponavimo versijoje) yra palaikomos.




K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai šifravimo metodui ir šifro atsparumui OS numatytuosius parametrus (XTS-AES-128) bus taikoma strategija su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?

A.: Ne. Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.

Pastaba "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta "Intune" strategija, kuri leidžia naudoti strategijos parametrus vietoj OS numatytųjų reikšmių




K jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?

A: šifravimo susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.




K: Kodėl Intune atitikties strategija rodo, kad mano įrenginys neturi "BitLocker" įjungtas, bet jis yra?

A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą. Šis klientas tik matuoja įrenginio būseną įkrovimo metu. Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.