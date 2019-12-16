---
title: Trūksta SharePoint Online terminas parduotuvė sąlygos
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053521"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo įgalinimas naudojant "Intune"

Intune galinio punkto apsaugos politika gali būti naudojama konfigūruoti Boitlocker šifravimo parametrus Windows įrenginių, kaip aprašyta: Windows10 (ir vėliau) parametrai apsaugoti įrenginius naudojant Intune

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10" palaiko automatinį "BitLocker" šifravimą, kuris suaktyvinamas netaikant MDM strategijos. Tai gali paveikti strategijos taikymą, jei sukonfigūruoti ne numatytieji parametrai. Daugiau informacijos rasite DUK.


DUK  klausimas: kokie "Windows" palaikymo įrenginių šifravimo leidimai naudojami naudojant galinio punkto apsaugos strategiją?
 A: Intune galinio punkto apsaugos strategijos parametrai yra įgyvendinami naudojant BitLocker CSP.Ne visi leidimai, nei komponavimo versijos "Windows" palaiko BitLocker CSP. 
      Šiuo metu "Windows" leidimai: įmonė; Švietimas, Mobile, Mobile Enterprise ir Professional (nuo statyti 1809 ir vėliau) yra remiami.




Q: Jei įrenginys jau yra užšifruotas su "BitLocker" naudojant OS numatytuosius parametrus šifravimo metodas ir šifro stiprumas (XTS-AES-128) bus taikyti politiką su skirtingais parametrais automatiškai sukelti iš naujo šifravimo disko su naujais parametrais?

A: ne. Norint taikyti naują šifro parametrus, pirmiausia turi būti iššifruotas diskas.

Pastaba įrenginiuose, kurie įtraukti į AutoPilot automatinio šifravimo, kad atsirastų per OOBE nėra paleidžiamas kol Intune strategija yra vertinama, kuri leidžia strategijos parametrus, kurie turi būti naudojami vietoj OS numatytosios




Q Jei prietaisas yra užšifruotas dėl Intune politikos taikymo bus iššifruoti, kai ši politika yra pašalinama?

A: pašalinus šifravimo susijusios politikos ne rezultatas iššifravimas diskus, kurie buvo sukonfigūruotas.




Klausimas: Kodėl Intune atitikties strategija rodo, kad mano įrenginys neturi "BitLocker įjungta", bet ji yra?

A: "BitLocker" įjungtas "parametras Intune atitikties strategijos naudoja Windows įrenginio sveikatos patvirtinimo (DHA) klientas. Šis klientas tik priemonės prietaiso būseną įkrovos metu. Taigi, jei įrenginys buvo paleistas iš naujo, nes "BitLocker" šifravimas buvo baigtas DHA klientų aptarnavimo nepateiks "BitLocker" kaip aktyvus.