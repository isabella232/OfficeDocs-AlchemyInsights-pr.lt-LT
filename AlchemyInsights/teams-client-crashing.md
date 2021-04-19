---
title: Genda „Teams“ klientas?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826279"
---
# <a name="teams-client-crashing"></a>Genda „Teams“ klientas?

Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:

- Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Įsitikinkite, kad visi ["Microsoft 365" URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) yra pasiekiami.

- Prisijunkite naudodami savo nuomotojo administratoriaus paskyrą ir patikrinkite tarnybos sveikatos ataskaitų [sritį,](https://docs.microsoft.com/office365/enterprise/view-service-health) kad įsitikintų, jog nėra atėjimo ar tarnybos blogėjimo.

- "Teams" taikomosios programos šalinimas ir diegimas iš naujo (saitas)
    - Eikite į aplanką %appdata%\Microsoft\teams\ kompiuteryje ir panaikinkite visus to katalogo failus.
    - [Atsisiųskite ir įdiekite "Teams" programą](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ir, jei įmanoma, įdiekite "Teams" kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite "Vykdyti administratoriaus teisėmis", jei yra).

Jei jūsų "Teams" klientas vis dar sugenda, ar galite atkurti problemą? Jei taip:

1. Norėdami užfiksuoti veiksmus, naudokite veiksmų rašytuvą.
    - Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.
    - Paleiskite veiksmų rašytuvą ir atkartokite problemą prisijungę naudodami paveiktą vartotojo paskyrą.
    - [Surinkite komandų žurnalus, kurie užfiksuoja įrašytus pakartotinio pelno veiksmus.](https://docs.microsoft.com/microsoftteams/log-files) **Pastaba:** įsitikinkite, kad užfiksuojate paveikto vartotojo prisijungimo adresą.
    - Rinkite iškelties ir (arba) gedimų talpyklos informaciją ("Windows"). Paleiskite "Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Pridėkite failą prie palaikymo atvejo.
