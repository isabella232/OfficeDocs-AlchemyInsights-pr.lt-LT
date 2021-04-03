---
title: "\"BitLocker\" atkūrimo klavišai"
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505076"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prieiga prie "BitLocker" atkūrimo raktų

Konfigūruojant "BitLocker" parametrus "Intune Endpoint Protection" strategiją, galima nustatyti, ar "BitLocker" atkūrimo informacija turi būti saugoma "Azure Active Directory".

Jei šis parametras sukonfigūruotas, saugomi atkūrimo duomenys turi būti matomi "Intune" administratoriui kaip įrenginio įrašo duomenų dalis "Intune" įrenginių ašmenyje dviem būdais:

Įrenginiai – "Azure AD" > "Device" OR Devices -> All Devices -> "Device" -> Recovery keys

Arba, jei yra administratoriaus prieiga prie paties įrenginio, atkūrimo raktą (slaptažodį) galima matyti vykdant šią komandą iš didesnių teisių komandinės eilutės:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Jei įrenginys buvo užšifruotas prieš prisijungiant "Intune", atkūrimo raktas gali būti susietas su "Microsoft" paskyra (MSA), naudojama prisijungti prie įrenginio OOBE proceso metu. Tokiu atveju prieiga prie MSA ir prisijungimas prie jos turėtų rodyti įrenginius,  https://onedrive.live.com/recoverykey kuriuose buvo saugomi atkūrimo raktai.
 
Jei įrenginys buvo užšifruotas dėl konfigūracijos naudojant domeno grupės strategiją, atkūrimo informacija gali būti saugoma vietinėje "Active Directory".

Jei sukonfigūravote galinio punkto apsaugos strategiją, kad būtų saugomas atkūrimo raktas "Azure Active Directory", bet konkretaus įrenginio raktas nebuvo nusiųstas, galite paleisti nusiuntimą pasukdami to įrenginio atkūrimo raktą iš MEM konsolės. Daugiau informacijos žr. ["BitLocker" atkūrimo klavišų pasukimas](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

