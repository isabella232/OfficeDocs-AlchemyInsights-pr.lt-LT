---
title: Saugojimo strategijos, Exchange administravimo centro neveikia
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480849"
---
 **Klausimas:** Naujai sukurta ar atnaujinta saugojimo strategijos, Exchange administravimo centro netaiko į pašto dėžutes arba nėra perkeliami į archyvo pašto dėžutę arba pašalinus elementus. 
  
 **Priežastis:**
  
- Tai gali būti todėl, kad **Valdomojo aplanko asistentas** ne perdirbo vartotojo pašto dėžutėje. Valdomojo aplanko asistentas bando tvarkyti kiekvieną pašto dėžutės į nuotolinių išteklių saugyklomis pagrįstos organizacijos kas septynias dienas. Jei pakeitėte saugojimo žymę arba taikyti kitą saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomas aplankas padeda apdoroja pašto dėžutę, arba galite paleisti Start-ManagedFolderAssistant cmdlet ir paleisti valdomojo aplanko asistentas apdoroti tam tikrą pašto dėžutės. Vykdyti į cmdlet yra naudinga bandyti ar trikčių šalinimo saugojimo strategijos ar saugojimo ˛ymės parametrus. Norėdami gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Sprendimas:** Vykdykite šią komandą pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Taip, gali nutikti, jei **RetentionHold** buvo **įjungtas** į pašto dėžutę. Jei pašto dėžutės buvo skiriamas į RetentionHold, saugojimo strategijos pašto dėžutės bus apdorotos per tą laiką. Dėl daugiau pateikiamoje RetentionHold parametrą žr: [Pašto dėžutės saugojimo palaikykite](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    Sprendimas
    
  - Patikrinkite, ar RetentionHold nustatyti konkrečias [EXO "PowerShell"](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)pašto dėžutės:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Vykdyti šią komandą, Norėdami **išjungti** RetentionHold tam tikros pašto dėžutės: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Dabar, naujo paleisti valdomos aplanko asistentas:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdorojami, pašto dėžutės. 
  

