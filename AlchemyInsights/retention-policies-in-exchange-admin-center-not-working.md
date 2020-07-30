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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522815"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos "Exchange" administravimo centre

Jei norite, kad mes vykdome toliau nurodytų parametrų automatinius patikrinimus, šio puslapio viršuje pasirinkite mygtuką "Atgal" <-- ir įveskite vartotojo, turinčio problemų dėl saugojimo strategijų, el. pašto adresą.

 **Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos Exchange administravimo centro netaikomos pašto dėžutės arba elementai nėra perkeliami į archyvo pašto dėžutę arba panaikinami. 
  
 **Priežastis:**
  
- Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės. Valdomojo aplanko asistentas bando apdoroti kiekvieną pašto dėžutę nuotolinių išteklių saugyklomis pagrįstoje organizacijoje kartą per septynias dienas. Jei pakeisite saugojimo žymę arba pritaikysite kitą saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomojo aplanko pagalbinė priemonė apdoros pašto dėžutę, arba galėsite paleisti cmdlet Start-ManagedFolderAssistant, kad paleistumėte valdomojo aplanko asistentą, kad apdorotumėte konkrečią pašto dėžutę. Šio cmdlet vykdymas naudingas tikrinant arba šalinant saugojimo strategijos arba saugojimo žymės parametrų triktis. Jei norite gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Taip gali atsitikti ir tuo atveju, jei **Saugojimhold** buvo **įjungtas** pašto dėžutės. Jei pašto dėžutės buvo ant RetentionHold, saugojimo strategijos pašto dėžutės nebus tvarkomi per tą laiką. Jei norite gauti daugiau informacijos apie RetentionHold parametrą žr.: [Pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Tirpalas:**
    
  - Patikrinkite, ar statusu RetentionHold parametrą konkrečios pašto dėžutės [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Vykdykite šią komandą norėdami **išjungti** RetentionHold konkrečioje pašto dėžutėje:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Dabar iš naujo paleiskite valdomojo aplanko asistentą:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdoroti pašto dėžutės.
 
Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:
- [Saugojimo žymės ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Saugojimo žymių pridėjimas arba šalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kaip nustatyti pašto dėžutės sulaikymo tipą](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
