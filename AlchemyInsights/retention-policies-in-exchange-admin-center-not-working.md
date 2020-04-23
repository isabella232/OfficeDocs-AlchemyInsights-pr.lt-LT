---
title: Saugojimo strategijos Exchange administravimo centro neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742441"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos "Exchange" administravimo centre

 **Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos "Exchange" administravimo centre netaikomos pašto dėžutėms arba elementai neperkeliami į archyvo pašto dėžutę arba panaikinami. 
  
 **Priežastis:**
  
- Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės. Valdomojo aplanko asistentas bando apdoroti kiekvieną nuotolinių išteklių saugyklomis pagrįstoje organizacijoje pašto dėžutę kartą per septynias dienas. Jei pakeisite saugojimo žymę arba pašto dėžutei taikote kitą saugojimo strategiją, galite palaukti, kol valdomos aplanko pagalbinė priemonė apdoros pašto dėžutę, arba galite paleisti cmdlet Start-ManagedFolderAssistant, kad paleistumėte valdomojo aplanko asistentą, kad apdorotumėte konkrečią pašto dėžutę. Šios cmdlet vykdymas naudingas tikrinant arba šalinant saugojimo strategiją arba saugojimo žymės parametrus. Jei norite gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tai taip pat gali įvykti, jei **RetentionHold** buvo **įjungtas** pašto dėžutės. Jei pašto dėžutės buvo įrašytas į RetentionHold, saugojimo strategija pašto dėžutės nebus tvarkomi per tą laiką. Daugiau informaton dėl RetentionHold parametrą žr.: [Pašto dėžutės saugojimo sulaikymo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Tirpalas:**
    
  - Patikrinkite, ar retentionHold parametro būseną konkrečios pašto dėžutės [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Vykdykite šią komandą **norėdami išjungti** RetentionHold konkrečioje pašto dėžutėje:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Dabar iš naujo paleiskite valdomojo aplanko asistentas:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdoroti pašto dėžutės.
 
Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:
- [Saugojimo žymės ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Saugojimo žymių pridėjimas arba šalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kaip nustatyti sulaikymo, padėto pašto dėžutėje, tipą](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
