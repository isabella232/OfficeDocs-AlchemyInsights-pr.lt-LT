---
title: Terminų trūksta "SharePoint Online Term Store"
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106434"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo įgalinimas naudojant "Intune"

Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in: Windows10 (and later) settings to protect devices using Intune

Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia Windows 10 palaiko automatinį "bitlocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos. Tai gali turėti įtakos strategijos taikymui, jei sukonfigūruoti ne numatytieji parametrai. Daugiau informacijos žr. DUK.


DUK K: kurie "Windows įrenginio šifravimo leidimai naudojant galinio punkto apsaugos strategiją?
A: "Intune Endpoint Protection" strategijos parametrai įgyvendinami naudojant "BitLocker" CSP.  Ne visi "Bitlocker" CSP Windows komponavimo versijos. Šiuo metu Windows: Enterprise; Švietimo, mobiliųjų įrenginių, mobiliųjų įrenginių ir profesionalų (nuo 1809 komponavimo versijos) palaikomi.




K: Jei įrenginys jau užšifruotas naudojant "BitLocker" naudojant numatytuosius OS šifravimo metodo parametrus ir šifravimo stiprumą (XTS-AES-128), strategija su skirtingais parametrais automatiškai suaktyvins disko šifravimą iš naujo su naujais parametrais?

A.: Ne. Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti diską.

Pastaba Įrenginiams, kurie yra užregistruoti naudojant "Autopilot", automatinis šifravimas, kuris būtų OOBE metu, nebus paleidžiamas, kol bus įvertinta "Intune" strategija, kuri leidžia strategijos pagrindu pagrįstus parametrus naudoti vietoje OS numatytųjų reikšmių




K Jei įrenginys šifruojamas dėl "Intune" strategijos taikymo, jis bus iššifruotas, kai ši strategija bus pašalinta?

A: Pašalinus su šifravimu susijusią strategiją, iššifruoti nekonfigūruoti diskai.




K: kodėl "intune" atitikties strategija rodo, kad mano įrenginyje nėra "Įgalinta "Bitlocker", bet taip yra?

A: "BitLocker enabled" parametras intune atitikties strategijos naudoja Windows įrenginio sveikatos patvirtinimo (DHR) klientą. Šis klientas įrenginio būseną tik įkelia metu. Taigi, jei įrenginys nebuvo paleistas iš naujo, nes "bitLocker" šifravimas buvo baigtas, DHR kliento tarnyba neinsins apie "bitlocker" kaip aktyvią.