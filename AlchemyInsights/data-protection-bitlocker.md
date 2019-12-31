---
title: DataProtection-"BitLocker"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908717"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>"BitLocker" šifravimo įgalinimas naudojant "Intune"

 Intune Endpoint Protection politika gali būti naudojama konfigūruoti BitLocker šifravimo parametrus Windows įrenginiams. Daugiau informacijos rasite ["Windows 10" (ir naujesniuose) parametruose, kad apsaugotume įrenginius naudojant "Intune"](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Turėtumėte žinoti, kad daug naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas netaikant MDM strategijos. Tai gali paveikti strategijos taikymą, jei sukonfigūruoti ne numatytieji parametrai. Daugiau informacijos rasite toliau pateiktuose DUK.
 
Informacijos apie "BitLocker" trikčių šalinimą rasite ["Microsoft Intune" "BitLocker" strategijos trikčių diagnostika](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Duk**

 Klausimas: kokie leidimai Windows palaikymo įrenginių šifravimo naudojant galinio punkto apsaugos strategijos?<br>
 A: Intune galinio punkto apsaugos strategijos parametrai yra įgyvendinami naudojant " [BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne visi leidimai ar komponavimo versijos Windows palaiko BitLocker CSP. <br><br>
      Šiuo metu palaikomi šie Windows leidimai: Enterprise, Education, Mobile, Mobile Enterprise ir Professional (statyti 1809 ir vėliau).
 
Q: Jei įrenginys jau yra užšifruotas naudojant "BitLocker" naudodami numatytuosius OS parametrus šifravimo metodui ir šifro patvarumui (XTS-AES-128), taikant strategiją su skirtingais parametrais, automatiškai suaktyvins disko šifravimą su naujais parametrais?<br>
A: ne. Norint taikyti naują šifro parametrus, diskas pirmiausia turi būti iššifruotas.<br><br>
**Pastaba:** Prietaisų, kurie mokosi su Autopilotas, automatinio šifravimo, kad atsirastų OOBE metu nėra paleidžiamas kol Intune strategija yra vertinama, kuri leidžia strategijos parametrai turi būti naudojami vietoj OS numatytąsias reikšmes.
 
Q: Jei įrenginys yra užšifruotas dėl Intune strategijos taikymo, ar jis bus iššifruoti, kai ši politika bus pašalinta?<br>
A: pašalinus šifravimo susijusios politikos ne rezultatas iššifravimas diskus, kurie buvo sukonfigūruotas.
 
Klausimas: Kodėl Intune atitikties politika rodo, kad mano įrenginys nėra įgalintas "BitLocker", nors ji yra?<br>
A: "BitLocker" įjungtas "nustatymas Intune atitikties strategijos naudoja" Windows "įrenginio sveikatos patvirtinimo (DHA) kliento. Šis klientas tik priemonės prietaiso būseną įkrovos metu. Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo baigtas, DHA kliento tarnyba nebus pranešti "BitLocker" kaip aktyvus.
 
 