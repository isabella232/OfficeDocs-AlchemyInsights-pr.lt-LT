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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522779"
---
# <a name="move-email-to-the-archive-mailbox"></a>El. laiško perkėlimas į archyvo pašto dėžutę

Jei norite, kad mes vykdome automatinius patikrinimus dėl toliau nurodytų nustatymų, pasirinkite mygtuką "Atgal" < -- šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų perkeliant el. laišką į savo archyvo pašto dėžutę, el. pašto adresą.

1. Patvirtinkite, kad **įgalinta archyvo pašto dėžutė.** Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.

2. Norint automatiškai archyvuoti laiškus į archyvo pašto dėžutę, saugojimo žymė su veiksmu **Perkelti į archyvą** turi būti nustatyta **kaip automatiškai taikoma visai pašto dėžutei (numatytoji) žymei**. Norėdami sukurti žymę, atlikite čia nurodytus veiksmus: [Archyvuoti numatytąją žymą](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tada pridėkite **žymę Archyvuoti** prie saugojimo strategijos. "Exchange" administravimo centre pasirinkite **Saugojimo strategijos** > į strategiją > **Įrašyti** **įtrauktumėte žymę Perkelti į archyvą** .

4. Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutei. Ta pati strategija bus taikoma ir **pirminio,** ir **archyvo** pašto dėžutei.

Gali prireikti priversti valdomojo aplanko asistentas (DTS) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutės. Vykdykite šią komandą, kai [prijungtas prie EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) paleisti valdomos aplanko asistentas konkrečios pašto dėžutės:
  
Start-ManagedFolderAssistant -tapatybės<name of the mailbox>

Daugiau informacijos apie archyvo strategijos nustatymą [ieškokite Pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  