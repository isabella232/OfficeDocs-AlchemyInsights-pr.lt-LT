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
# <a name="teams-client-crashing"></a><span data-ttu-id="515a0-102">Teams kliento gedimas</span><span class="sxs-lookup"><span data-stu-id="515a0-102">Teams client crashing</span></span>

<span data-ttu-id="515a0-103">Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="515a0-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="515a0-104">Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="515a0-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="515a0-105">Įsitikinkite, kad [visi Microsoft 365 URL ir adresų diapazonai](/microsoftteams/connectivity-issues) yra pasiekiami.</span><span class="sxs-lookup"><span data-stu-id="515a0-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="515a0-106">Prisijunkite naudodami savo nuomotojo administratoriaus paskyrą ir patikrinkite tarnybos sveikatos ataskaitų [sritį,](/office365/enterprise/view-service-health) kad įsitikintų, jog nėra atėjimo ar tarnybos blogėjimo.</span><span class="sxs-lookup"><span data-stu-id="515a0-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="515a0-107">Pašalinkite ir iš naujo įdiekite "Teams taikomąją programą</span><span class="sxs-lookup"><span data-stu-id="515a0-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="515a0-108">Eikite į aplanką %appdata%\Microsoft\Teams\ kompiuteryje ir panaikinkite visus to katalogo failus.</span><span class="sxs-lookup"><span data-stu-id="515a0-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="515a0-109">[Atsisiųskite ir įdiekite "Teams"](https://www.microsoft.com/microsoft-teams/download-app)programą ir, jei įmanoma, įdiekite "Teams kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite Vykdyti **administratoriaus teisėmis,** jei yra).</span><span class="sxs-lookup"><span data-stu-id="515a0-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="515a0-110">Jei jūsų Teams klientas vis dar sugenda, pabandykite atkurti problemą.</span><span class="sxs-lookup"><span data-stu-id="515a0-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="515a0-111">Jei galite:</span><span class="sxs-lookup"><span data-stu-id="515a0-111">If you can:</span></span>

1. <span data-ttu-id="515a0-112">Norėdami užfiksuoti veiksmus, naudokite veiksmų rašytuvą.</span><span class="sxs-lookup"><span data-stu-id="515a0-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="515a0-113">Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.</span><span class="sxs-lookup"><span data-stu-id="515a0-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="515a0-114">Paleiskite veiksmų rašytuvą ir atkartokite problemą prisijungę naudodami paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="515a0-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="515a0-115">[Surinkite komandų žurnalus, kurie užfiksuoja įrašytus pakartotinio pelno veiksmus.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="515a0-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="515a0-116">**Pastaba:** įsitikinkite, kad užfiksuojate paveikto vartotojo prisijungimo adresą.</span><span class="sxs-lookup"><span data-stu-id="515a0-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="515a0-117">Rinkite iškelties ir (arba) gedimų talpyklos informaciją (Windows).</span><span class="sxs-lookup"><span data-stu-id="515a0-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="515a0-118">Paleiskite Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas (po kiekvienos komandos paspauskite "Enter"):</span><span class="sxs-lookup"><span data-stu-id="515a0-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="515a0-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="515a0-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="515a0-120">Kai teksto failas sugeneruojamas ir rodomas ekrane, įrašykite failą ir pridėkite jį prie tarnybos užklausos.</span><span class="sxs-lookup"><span data-stu-id="515a0-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
