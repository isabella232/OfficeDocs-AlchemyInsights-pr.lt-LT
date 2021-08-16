---
title: "\"Exchange Online PowerShell\" naudojimas norint įgalinti DKIM konkrečiam domenui"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070316"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>"Exchange Online PowerShell" naudojimas norint įgalinti DKIM konkrečiam domenui

Jei negalite sukurti DKIM DNS įrašų administravimo centre, pabandykite naudoti "Exchange Online PowerShell". 

Norėdami sukurti DKIM DNS įrašą naudodami "Exchange Online PowerShell", atlikite šiuos veiksmus:

1. Atidarykite Windows PowerShell administratoriaus teisėmis ir vykdykite toliau nurodytas komandas aprašyta seka:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jei kyla problemų jungiantis prie "Exchange Online PowerShell", [žr. Prisijungimas to Exchange Online PowerShell".](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kai prisijungsite prie "Exchange Online PowerShell", vykdykite šią komandą:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Sėkmingai įvykdžius anksčiau nurodytą komandą, vykdykite šią komandą, kad nutrauktų "PowerShell" Exchange Online seansą:

    `Remove-PSSession $Session` 



