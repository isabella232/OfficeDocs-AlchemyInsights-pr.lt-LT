---
title: El. laiškų perkėlimas į archyvo pašto dėžutę
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974965"
---
# <a name="move-email-to-the-archive-mailbox"></a>El. pašto perkėlimas į archyvo pašto dėžutę

Jei norite, kad automatiškai patikrindami toliau nurodytus parametrus, šio puslapio viršuje pasirinkite mygtuką Atgal <- ir įveskite vartotojo, kuris susiduria su problemomis perkeliant el. paštą į savo archyvo pašto dėžutę, el. pašto adresą.

1. Patvirtinkite, **kad įgalinta archyvo** pašto dėžutė. Jei ne, atlikite šiame straipsnyje nurodytus [veiksmus, kad įgalintumėte](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) archyvo pašto dėžutę.

2. Norint automatiškai archyvuoti laiškus į archyvo pašto dėžutę, saugojimo žymė su veiksmu Perkelti į **archyvą** turi būti nustatyta automatiškai taikyti visai pašto **dėžutės (numatytoji) žymai.** Norėdami sukurti žymę, atlikite čia nurodytus veiksmus: [Archyvuoti numatytąją žymę](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tada įtraukite **archyvo žymę** į saugojimo strategiją. Administravimo Exchange pasirinkite Saugojimo strategijos ir **>** žymę Perkelti į **archyvą** į strategiją, > **Įrašyti.**

4. Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutei. Ta pati strategija bus taikoma ir pašto dėžutėms **Pirminis,** ir **Archyvuoti.**

Gali tekti priversti valdomojo aplanko pagalbinę priemonę (MFA) vykdyti ir taikyti naujus parametrus vartotojo pašto dėžutei. Vykdykite šią komandą, kai [esate prisijungę prie "EXO PowerShell",](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) kad paleisite konkrečios pašto dėžutės valdomų aplankų pagalbinę priemonę:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Daugiau informacijos apie archyvo strategijos nustatymą žr. [Pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  