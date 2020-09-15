---
title: "\"BitLocker\" atkūrimo raktai"
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685894"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Prieiga prie "BitLocker" atkūrimo raktų

Konfigūruojant "BitLocker" parametrų Intune Endpoint Protection strategiją, galima nustatyti, ar "BitLocker" atkūrimo informacija turėtų būti saugoma "Azure Active Directory".

Jei šis parametras sukonfigūruotas, saugomi atkūrimo duomenys turėtų būti matomi Intune admin kaip įrenginio įrašo duomenis "Intune" įrenginių ašmenimis dviem būdais:

Įrenginiai – "Azure AD" įrenginiai – > "įrenginys" arba įrenginiai – > visi įrenginiai – > "įrenginys" – > atkūrimo raktai

Arba, jei yra administracinė prieiga prie paties įrenginio, atkūrimo raktą (slaptažodį) galima matyti paleisdami šią komandą iš didesnių teisių komandų eilutės:

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
Jei įrenginys buvo užšifruotas prieš registraciją "Intune", atkūrimo kodas gali būti susietas su "Microsoft" abonementu (MSA), naudojamu prisijungti prie įrenginio OOBE proceso metu. Jei tai buvo atvejis, prisijungimas prie  https://onedrive.live.com/recoverykey MSA ir prisijungimas prie jos turėtų Rodyti įrenginius, kurių atkūrimo raktai buvo saugomi.
 
Jei įrenginys buvo užšifruotas kaip konfigūravimo rezultatas pagal domeno grupės strategiją, atkūrimo informacija gali būti saugoma vietiniame "Active Directory".
 

