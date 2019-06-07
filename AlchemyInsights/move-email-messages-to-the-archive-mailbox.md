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
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762373"
---
# <a name="move-email-to-the-archive-mailbox"></a>Perkelti laišką į archyvo pašto dėžutę
 
1. Patvirtinkite, kad **archyvo pašto dėžutės** įgalintas. Jei ne, atlikite veiksmus [šiame](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) straipsnyje, kad archyvo pašto dėžutę.

2. Jei norite archyvuoti pranešimus automatiškai į archyvo pašto dėžutę, saugojimo žymę **perkelti į archyvą** veikla turi būti nustatytas kaip **automatiškai taikomas visą dėžutę (numatytoji) žymę**. Atlikite veiksmus čia sukurti žymę: [Archyvas numatytoji žymė](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Toliau, pridėkite **Archyvas** žymę su saugojimo strategija. Exchange administravimo centrą, pasirinkite **Saugojimo strategijos** > pridėti **perkelti į archyvo žymių** **įrašyti**politikos >. 
    
4. Dabar [priskirti saugojimo strategija](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) į konkrečius vartotojo pašto dėžutėje. Ta pačia sutartimi taikysite į **pirminį** ir **archyvo** pašto dėžutę. 
    
Reikia priversti valdomos aplanko asistentas (URM) vykdyti ir taikyti naujus parametrus vartotojo pašto dėžutėje. Vykdykite šią komandą kol [prijungtas prie EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Daugiau informacijos apie archyvavimo strategijos nustatymą, žiūrėkite [nustatyti archyvavimo ir naikinimo politiką pašto dėžučių](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

