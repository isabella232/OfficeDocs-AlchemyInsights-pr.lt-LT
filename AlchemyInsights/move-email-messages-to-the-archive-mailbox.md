---
title: Perkelti el. laiškus į archyvo pašto dėžutę
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822170"
---
# <a name="move-email-to-the-archive-mailbox"></a>Perkelti el. paštą į archyvo pašto dėžutę

1. Patvirtinkite, kad įgalinta **archyvo pašto dėžutė** . Jei ne, naudokite [šiame straipsnyje](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.

2. Norint automatiškai archyvuoti pranešimus į archyvo pašto dėžutę, saugojimo žymė su veiksmu **perkelti į archyvą** turi būti nustatyta **automatiškai taikoma visai pašto dėžutei (numatytoji) žymėje**. Norėdami sukurti žymę, pasinaudokite čia esančiais žingsniais: [archyvuokite numatytąją žymę](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tada pridėkite **archyvo** žymę prie saugojimo strategijos. "Exchange" administravimo centre pasirinkite **saugojimo strategijos** > įtraukite **perkelti į archyvą žymę** į strategiją > **įrašyti**.

4. Dabar [priskirti saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutės. Ta pati strategija bus taikoma ir **pirminei** , ir **archyvo** pašto dėžutei.

Gali reikėti priversti valdomojo aplanko asistentą (MFP) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutei. Kai [prisijungėte prie "EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) " Norėdami paleisti konkrečios pašto dėžutės valdomojo aplanko asistentą, vykdykite šią komandą:
  
Start-ManagedFolderAssistant-tapatybė<name of the mailbox>

Daugiau informacijos apie archyvavimo strategijos nustatymą ieškokite [pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  