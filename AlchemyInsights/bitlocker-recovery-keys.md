---
title: "\"BitLocker\" atkūrimo klavišai"
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060072"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prieiga prie "BitLocker" atkūrimo raktų

Konfigūruojant "BitLocker" parametrus "Intune Endpoint Protection" strategiją, galima nustatyti, ar "Bitlocker" atkūrimo informacija turėtų būti saugoma ""Azure Active Directory"".

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

Jei sukonfigūravote galinio punkto apsaugos strategiją, kad atkūrimo raktas būtų saugomas ""Azure Active Directory"", bet konkretaus įrenginio raktas nebuvo nusiųstas, galite paleisti nusiuntimą pasukdami to įrenginio atkūrimo raktą iš MEM konsolės. Daugiau informacijos žr. ["BitLocker" atkūrimo klavišų pasukimas](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

