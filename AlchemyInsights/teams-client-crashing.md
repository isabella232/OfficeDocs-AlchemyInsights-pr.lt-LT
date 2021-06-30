---
title: Teams kliento gedimas
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187729"
---
# <a name="teams-client-crashing"></a>Teams kliento gedimas

Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:

- Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Įsitikinkite, kad [visi Microsoft 365 URL ir adresų diapazonai](/microsoftteams/connectivity-issues) yra pasiekiami.

- Prisijunkite naudodami savo nuomotojo administratoriaus paskyrą ir patikrinkite tarnybos sveikatos ataskaitų [sritį,](/office365/enterprise/view-service-health) kad įsitikintų, jog nėra atėjimo ar tarnybos blogėjimo.

- Pašalinkite ir iš naujo įdiekite "Teams taikomąją programą
    - Eikite į aplanką %appdata%\Microsoft\Teams\ kompiuteryje ir panaikinkite visus to katalogo failus.
    - [Atsisiųskite ir įdiekite "Teams"](https://www.microsoft.com/microsoft-teams/download-app)programą ir, jei įmanoma, įdiekite "Teams kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite Vykdyti **administratoriaus teisėmis,** jei yra).

Jei jūsų Teams klientas vis dar sugenda, pabandykite atkurti problemą. Jei galite:

1. Norėdami užfiksuoti veiksmus, naudokite veiksmų rašytuvą.
    - Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.
    - Paleiskite veiksmų rašytuvą ir atkartokite problemą prisijungę naudodami paveiktą vartotojo paskyrą.
    - [Surinkite komandų žurnalus, kurie užfiksuoja įrašytus pakartotinio pelno veiksmus.](/microsoftteams/log-files) **Pastaba:** įsitikinkite, kad užfiksuojate paveikto vartotojo prisijungimo adresą.
    - Rinkite iškelties ir (arba) gedimų talpyklos informaciją (Windows). Paleiskite Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas (po kiekvienos komandos paspauskite "Enter"):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kai teksto failas sugeneruojamas ir rodomas ekrane, įrašykite failą ir pridėkite jį prie tarnybos užklausos. 
