---
title: "\"SharePoint Online\" terminų saugykloje trūksta sąlygų"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766861"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo įgalinimas naudojant "Intune"

Intune Endpoint Protection Policy gali būti naudojamas konfigūruoti Boitlocker šifravimo parametrus Windows įrenginių, kaip aprašyta: Windows10 (ir vėliau) parametrus apsaugoti įrenginius naudojant Intune

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "bitLocker" šifravimą, kuris paleidžiamas be MDM strategijos taikymo. Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti. Daugiau informacijos rasite DUK.


DUK  Q: Kurie "Windows" palaikymo įrenginių šifravimo leidimai naudojant galinio punkto apsaugos strategiją?
 A: Intune Endpoint Protection strategijos parametrai yra įgyvendinami naudojant "BitLocker" CSP.Ne visi "Windows" leidimai ir komponavimo versijos palaiko "BitLocker" CSP. 
      Šiuo metu "Windows" leidimai: įmonė; "Education", "Mobile", "Mobile" ir "Professional" (nuo 1809 m. komponavimo versijos) yra remiamos.




Klausimas: Jei įrenginys jau užšifruotas su "BitLocker" naudojant OS numatytuosius parametrus šifravimo metodui ir šifravimo stiprumas (XTS-AES-128) taiks strategiją su skirtingais parametrais automatiškai sukelti pakartotinį disko šifravimą su naujais parametrais?

Ats.: Ne. Norint taikyti naujus šifravimo parametrus, diskas pirmiausia turi būti iššifruotas.

Pastaba Įrenginiams, įtrauktiems su autopilotu, automatinis šifravimas, kuris įvyktų OOBE metu, neįjungiamas, kol neįvertinama Intune strategija, kuri leidžia naudoti strategijos pagrindu pagrįstus parametrus vietoj os numatytųjų reikšmių




K Jei įrenginys yra užšifruotas dėl Intune strategijos taikymo, ar jis bus iššifruotas, kai ši strategija bus pašalinta?

A: Šifravimo susijusios strategijos pašalinimas nesukelia sukonfigūruotidiskų iššifravimo.




K: Kodėl intune atitikties strategija rodo, kad mano įrenginyje nėra "BitLocker Įjungta", bet tai yra?

A: "BitLocker įjungtas" parametras intune atitikties strategija naudoja Windows įrenginio sveikatos patvirtinimo (Dha) kliento. Šis klientas matuoja tik įrenginio būseną įkrovos metu. Taigi, jei įrenginys nebuvo paleistas iš naujo, nes "bitLocker" šifravimas buvo baigtas, Dha kliento tarnyba nepraneš apie "bitLocker" kaip aktyvų.