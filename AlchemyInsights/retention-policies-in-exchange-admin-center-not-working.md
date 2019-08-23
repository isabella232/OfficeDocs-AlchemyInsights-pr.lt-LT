---
title: Saugojimo strategijos, Exchange administravimo centro neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551351"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos, Exchange administravimo centro

 **Klausimas:** Naujai sukurta ar atnaujinta saugojimo strategijos, Exchange administravimo centro netaiko į pašto dėžutes arba nėra perkeliami į archyvo pašto dėžutę arba pašalinus elementus. 
  
 **Priežastis:**
  
- Tai gali būti todėl, kad **Valdomojo aplanko asistentas** ne perdirbo vartotojo pašto dėžutėje. Valdomojo aplanko asistentas bando tvarkyti kiekvieną pašto dėžutės į nuotolinių išteklių saugyklomis pagrįstos organizacijos kas septynias dienas. Jei pakeitėte saugojimo žymę arba taikyti kitą saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomas aplankas padeda apdoroja pašto dėžutę, arba galite paleisti Start-ManagedFolderAssistant cmdlet ir paleisti valdomojo aplanko asistentas apdoroti tam tikrą pašto dėžutės. Vykdyti į cmdlet yra naudinga bandyti ar trikčių šalinimo saugojimo strategijos ar saugojimo ˛ymės parametrus. Norėdami gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Sprendimas:** Vykdykite šią komandą pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Taip, gali nutikti, jei **RetentionHold** buvo **įjungtas** į pašto dėžutę. Jei pašto dėžutės buvo skiriamas į RetentionHold, saugojimo strategijos pašto dėžutės bus apdorotos per tą laiką. Dėl daugiau pateikiamoje RetentionHold parametrą žr: [Pašto dėžutės saugojimo palaikykite](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Sprendimas:**
    
  - Patikrinkite, ar RetentionHold nustatyti konkrečias [EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)pašto dėžutės:
    
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
 
Daugiau informacijos apie saugojimo strategijos, Exchange administravimo centro, žr.:
- [Saugojimo ˛ymes ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Taikyti saugojimo strategijos į pašto dėžutes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Pridėti arba pašalinti saugojimo žymes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kaip nustatyti tos rūšies palaikykite ant pašto dėžutės](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
