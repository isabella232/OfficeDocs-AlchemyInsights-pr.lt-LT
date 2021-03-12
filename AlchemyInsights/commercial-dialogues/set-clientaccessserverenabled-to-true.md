---
title: Nustatykite ClientAccessServerEnabled į TRUE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749983"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nustatykite ClientAccessServerEnabled į TRUE

Jei negalite atidaryti užšifruotos el. laiško, o ne matyti **rpmsg** priedą, atlikite šiuos veiksmus:

1. Prisijungimas prie "Exchange Online" "PowerShell".

> [!NOTE]
> Norėdami prisijungti prie "Exchange Online PowerShell", turite prisijungti naudodami visuotinio administratoriaus arba "Exchange" administratoriaus paskyrą.

   a. Atidarykite "Windows PowerShell", tada vykdykite šią komandą: `$UserCredential = Get-Credential`
b. Dialogo lange **"Windows PowerShell" kredencialų užklausa** įveskite savo darbo arba mokymo įstaigos paskyrą ir slaptažodį, c. Spustelėkite **Gerai**. 

2. Vykdykite šią komandą, kad sukurtumėte naują seansą:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Vykdykite toliau nurodytą komandą.
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Komanda vykdyti.

4. Pažymėkite parametrą **Clientaccessserverenabled** . 

    a. Jei parametras **Clientaccessserverenabled** nustatytas kaip **klaidingas**, vykdykite šią "cmdlet": `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Visada uždarykite "PowerShell" seansą naudodami šią komandą: `Remove-PSSession $Session`

Daugiau informacijos ieškokite " [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)".

