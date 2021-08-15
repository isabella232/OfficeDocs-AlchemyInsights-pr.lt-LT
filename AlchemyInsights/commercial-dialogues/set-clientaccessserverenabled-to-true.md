---
title: Nustatyti ClientAccessServerEnabled kaip True
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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994873"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nustatyti ClientAccessServerEnabled kaip True

Jei negalite atidaryti šifruoto el. laiško ir vietoj to **matote rpmsg priedą,** atlikite šiuos veiksmus:

1. Prisijungimas "Exchange Online PowerShell".

> [!NOTE]
> Norėdami prisijungti prie "Exchange Online PowerShell", turite prisijungti naudodami visuotinį administratorių arba Exchange administratoriaus paskyrą.

   a. Atidarykite Windows PowerShell, tada vykdykite šią komandą:`$UserCredential = Get-Credential`
b. Dialogo **Windows PowerShell kredencialų užklausa** įveskite savo darbo arba mokymo įstaigos paskyrą ir slaptažodį, c. Spustelėkite **Gerai**. 

2. Norėdami sukurti naują seansą, vykdykite šią komandą:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Vykdykite toliau nurodytą komandą.
    
    `Import-PSSession $Session -DisableNameChecking`

3. Vykdyti `Get-IRMConfiguration` komandą.

4. Patikrinkite **parametrą ClientAccessServerEnabled.** 

    a. Jei **Parametras ClientAccessServerEnabled** nustatytas kaip **False**, vykdykite šią "cmdlet": `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Visada uždarykite "PowerShell" seansą naudodami šią komandą: `Remove-PSSession $Session`

Daugiau informacijos žr. Exchange Online ["PowerShell".](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

