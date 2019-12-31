---
title: "\"BitLocker\" atkūrimo raktai"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908822"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prieiga prie "BitLocker" atkūrimo raktų

Konfigūruojant BitLocker parametrus Intune Endpoint Protection strategijos, galima nustatyti, ar "BitLocker" atkūrimo informacija turi būti saugoma Azure Active Directory.

Jei šis parametras sukonfigūruotas, saugomi atkūrimo duomenys turi būti matomi Intune administratorius kaip įrenginio įrašo duomenų Intune įrenginių ašmenys dviem būdais:

Įrenginiai – "Azure AD" įrenginiai – > "įrenginys" arba įrenginiai – > visi įrenginiai – > "įrenginys" – > atkūrimo raktai

Arba, jei yra administratoriaus prieigos prie paties įrenginio, atkūrimo rakto (slaptažodis) galima matyti vykdydami šią komandą iš didesnių teisių komandų eilutėje:

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
Jei įrenginys buvo užšifruotas prieš registracija į Intune, atkūrimo raktas gali būti susietas su "Microsoft account" (MSA), naudojama prisijungti prie įrenginio OOBE metu. Tokiu atveju norint pasiekti https://onedrive.live.com/recoverykey ir prisijungti prie MSA turėtų būti rodomi įrenginiai, kuriems atkūrimo raktai buvo saugomi.
 
Jei įrenginys buvo užšifruotas dėl konfigūracijos naudojant domeno grupės strategiją, atkūrimo informacija gali būti saugoma vietiniame Active Directory.
 

