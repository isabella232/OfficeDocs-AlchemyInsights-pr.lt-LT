---
title: El. laiškų perkėlimas į archyvo pašto dėžutę
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713654"
---
# <a name="move-email-to-the-archive-mailbox"></a>El. pašto perkėlimas į archyvo pašto dėžutę

1. Patvirtinkite, kad **įgalinta archyvo pašto dėžutė.** Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.

2. Norint automatiškai archyvuoti pranešimus į archyvo pašto dėžutę, saugojimo žyma su veiksmu **Perkelti į archyvą** turi būti nustatyta taip, kad automatiškai **būtų taikoma visai pašto dėžutei (numatytoji) žymai**. Norėdami sukurti žymę, atlikite čia nurodytus veiksmus: [Archyvo numatytoji žymė](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tada įtraukite **archyvo** žymę į saugojimo strategiją. "Exchange" administravimo centre pasirinkite **Saugojimo strategijos** > įtrauktumėte **žymę Perkelti į archyvą** į strategijos > **Įrašyti**.

4. Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutei. Ta pati strategija bus taikoma ir **pirminio,** ir **archyvo** pašto dėžutei.

Gali tekti priversti valdomojo aplanko asistentas (DTS) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutę. Norėdami paleisti konkrečios pašto dėžutės valdomos aplanko asistentą, [vykdykite](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) šią komandą:
  
Start-ManagedFolderAssistant -tapatybės<name of the mailbox>

Daugiau informacijos apie archyvo strategijos nustatymą ieškokite [Pašto dėžučių archyvo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  