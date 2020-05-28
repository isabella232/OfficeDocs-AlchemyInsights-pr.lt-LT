---
title: Genda „Teams“ klientas?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354060"
---
# <a name="teams-client-crashing"></a>Genda „Teams“ klientas?

Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:

- Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Įsitikinkite, kad visi ["Microsoft 365" URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) yra pasiekiami.

- Prisijunkite naudodami nuomotojo administratoriaus abonementą ir patikrinkite [savo tarnybos sveikatos ataskaitų sritį,](https://docs.microsoft.com/office365/enterprise/view-service-health) kad patikrintumėte, ar nėra atjungimo ar tarnybos pablogėjimo.

- "Teams" taikomosios programos pašalinimas ir diegimas iš naujo (saitas)
    - Raskite aplanką %appdata%\Microsoft\teams\ savo kompiuteryje ir panaikinkite visus tame kataloge esančius failus.
    - [Atsisiųskite ir įdiekite "Teams" programą](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ir, jei įmanoma, įdiekite "Teams" kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite "Paleisti administratoriaus teisėmis", jei yra).

Jei jūsų komandos klientas vis dar genda, ar galite atkurti problemą? Jei taip:

1. Norėdami užfiksuoti veiksmus, atlikite veiksmus.
    - Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.
    - Paleiskite veiksmų rašytuvą ir atkurkite problemą, kai prisijungė tedininkas su susijusio vartotojo abonementą.
    - [Rinkti komandos žurnalus, kad užfiksuoti įrašytus repro veiksmus](https://docs.microsoft.com/microsoftteams/log-files). **Pastaba:** įsitikinkite, kad fiksuojate paveikto naudotojo prisijungimo adresą.
    - Rinkti iškelties ir / arba gedimų kibirą informacija (Windows). Paleiskite "Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Pridėkite failą prie palaikymo atvejo.
