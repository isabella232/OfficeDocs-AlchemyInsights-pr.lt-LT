---
title: "\"Exchange Online\" \"PowerShell\" naudojimas \"DKIM\" konkrečiam domenui įgalinti"
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749724"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>"Exchange Online" "PowerShell" naudojimas "DKIM" konkrečiam domenui įgalinti

Jei negalite sukurti DKIM DNS įrašus administravimo centre, bandykite naudoti "Exchange Online" "PowerShell". 

Norėdami sukurti DKIM DNS įrašą naudodami "Exchange Online" "PowerShell", atlikite šiuos veiksmus:

1. Atidarykite "Windows PowerShell" kaip administratorius ir vykdykite šias komandas aprašyta seka:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jei kyla problemų jungiantis prie "Exchange Online PowerShell", peržiūrėkite [prisijungti prie "Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)".

2. Kai prisijungsite prie "Exchange Online PowerShell", vykdykite šią komandą:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Sėkmingai įvykdę aukščiau nurodytą komandą, vykdykite šią komandą, kad nutrauktų "Exchange Online" "PowerShell" seansą:

    `Remove-PSSession $Session` 



