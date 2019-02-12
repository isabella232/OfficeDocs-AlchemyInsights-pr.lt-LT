---
title: Perkelti el. laiškus į archyvo pašto dėžutę
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941722"
---
Problemų archyvuoti elementus į archyvo pašto dėžutę. Įsitikinkite, kad turite atlikti šiuos veiksmus:
  
1. Patvirtinkite, kad **archyvo pašto dėžutės** įgalintas. Jei ne, atlikite veiksmus [šiame](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) straipsnyje, kad archyvo pašto dėžutę. 
    
2. Exchange administravimo centro, pasirinkite **Saugojimo ˛ymes** pagal **Reikalavimų laikymosi valdymas**, sukurti **saugojimo žymę** **perkelti į archyvą** veiksmų, kuriame yra norimas **Saugojimo laiką**.
    
3. Exchange administravimo centro, pasirinkite **Saugojimo strategijas**, sukurti **Saugojimo strategija** ir pridėti savo **perkelti į archyvo** saugojimo žymę prie tos politikos. 
    
4. [Priskirti saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutėje. Ta pačia sutartimi taikysite į **pirminį** ir **archyvo** pašto dėžutę. 
    
Vartotojo pašto dėžutės dabar yra archyvavimo strategija galite perkelti elementus į archyvo pašto dėžutę. Reikia priversti valdomos aplanko asistentas (URM) vykdyti ir taikyti naujus parametrus vartotojo pašto dėžutėje. Vykdykite šią komandą kol [prijungtas prie EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Norite gauti daugiau informacijos apie archyvavimo strategijos nustatymas, žiūrėkite [nustatyti archyvavimo ir naikinimo politiką pašto dėžučių](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

