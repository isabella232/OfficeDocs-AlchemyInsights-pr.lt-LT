---
title: Laiškų perkėlimas į archyvo pašto dėžutę
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799788"
---
# <a name="move-email-to-the-archive-mailbox"></a>Perkelti laišką į archyvo pašto dėžutę

Jei norite, kad būtų atlikti automatizuoti toliau nurodytų parametrų tikrinimai, pasirinkite mygtuką atgal <--šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų perkeliant laiškus į archyvo pašto dėžutę, el. pašto adresą.

1. Patikrinkite, ar įgalintas **archyvo pašto dėžutė** . Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.

2. Kad laiškai automatiškai būtų archyvuojami į archyvo pašto dėžutę, saugojimo žymė su veiksmu **perkelti į archyvą** turi būti nustatyta **automatiškai pritaikyta visai pašto dėžutei (numatytoji)**. Atlikite toliau nurodytus veiksmus, kad sukurtumėte žymę: [archyvuoti numatytąjį žymę](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tada įtraukite **archyvo** žymę į saugojimo strategiją. "Exchange" administravimo centre pasirinkite **saugojimo strategijos** > įtraukite **perkėlimo į archyvą žymę** į strategiją > **įrašyti**.

4. Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrečiam vartotojo pašto dėžutei. Ta pati strategija bus taikoma ir **pirminės** ir **archyvo** pašto dėžutei.

Gali reikėti priverstinai vykdyti valdomojo aplanko asistentą (MFA) ir taikyti naujus parametrus vartotojo pašto dėžutei. Norėdami paleisti konkrečios pašto dėžutės valdomojo aplanko asistentą, būdami [prisijungę prie "EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) " vykdykite šią komandą:
  
Start – ManagedFolderAssistant – tapatybė <name of the mailbox>

Daugiau informacijos apie archyvavimo strategijos nustatymą rasite [pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  