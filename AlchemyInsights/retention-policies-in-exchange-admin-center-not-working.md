---
title: "\"Exchange\" administravimo centro neveikia saugojimo strategijos"
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740518"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos "Exchange" administravimo centre

Jei norite, kad būtų atlikti automatizuoti toliau nurodytų parametrų tikrinimai, pasirinkite mygtuką atgal <--šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų su saugojimo strategijomis, el. pašto adresą.

 **Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos "Exchange" administravimo centre netaikomos pašto dėžutėms arba elementai neperkeliami į archyvo pašto dėžutę arba panaikinta. 
  
 **Pagrindinės priežastys:**
  
- Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės. Valdomojo aplanko asistentas kiekvieną nuotolinių išteklių saugyklomis pagrįstos organizacijos pašto dėžutę bando apdoroti kas septynias dienas. Jei keičiate saugojimo žymę arba taikote kitokią saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomojo aplanko pagalba apdoros pašto dėžutę, arba galite paleisti "Start-ManagedFolderAssistant" cmdlet, kad paleistumėte valdomojo aplanko asistentą ir apdorotų konkrečią pašto dėžutę. Paleidus šią "cmdlet" galima išbandyti arba pašalinti saugojimo strategijos arba išsaugojimo žymių parametrus. Norėdami gauti daugiau informacijos, apsilankykite [valdomojo aplanko pagalbinės priemonės paleidimas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Taip pat gali nutikti, jei pašto dėžutėje **įgalintas** **RetentionHold** . Jei pašto dėžutė yra įtraukta į Retentionsulaikymą, pašto dėžutės saugojimo strategija tuo metu nebus apdorota. Daugiau informacijos apie RetentionHold parametrą matyti: [pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Tirpalo**
    
  - Pažymėkite " [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)" konkrečios pašto dėžutės parametro RetentionHold būseną:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Vykdykite šią komandą, kad **išjungtumėte** RetentionHold konkrečioje pašto dėžutėje:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Dabar iš naujo paleiskite valdomojo aplanko asistentą:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Pastaba:** Jei pašto dėžutė yra mažesnė nei 10 MB, valdomojo aplanko asistentas automatiškai neapdoros pašto dėžutės.
 
Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:
- [Saugojimo žymės ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Saugojimo žymių įtraukimas arba šalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kaip nustatyti pašto dėžutėje esančio sulaikymo tipą](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
