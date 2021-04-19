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
# <a name="teams-client-crashing"></a><span data-ttu-id="d283f-102">Genda „Teams“ klientas?</span><span class="sxs-lookup"><span data-stu-id="d283f-102">Teams client crashing?</span></span>

<span data-ttu-id="d283f-103">Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="d283f-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="d283f-104">Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="d283f-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="d283f-105">Įsitikinkite, kad visi ["Microsoft 365" URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) yra pasiekiami.</span><span class="sxs-lookup"><span data-stu-id="d283f-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="d283f-106">Prisijunkite naudodami savo nuomotojo administratoriaus paskyrą ir patikrinkite tarnybos sveikatos ataskaitų [sritį,](https://docs.microsoft.com/office365/enterprise/view-service-health) kad įsitikintų, jog nėra atėjimo ar tarnybos blogėjimo.</span><span class="sxs-lookup"><span data-stu-id="d283f-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="d283f-107">"Teams" taikomosios programos šalinimas ir diegimas iš naujo (saitas)</span><span class="sxs-lookup"><span data-stu-id="d283f-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="d283f-108">Eikite į aplanką %appdata%\Microsoft\teams\ kompiuteryje ir panaikinkite visus to katalogo failus.</span><span class="sxs-lookup"><span data-stu-id="d283f-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="d283f-109">[Atsisiųskite ir įdiekite "Teams" programą](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ir, jei įmanoma, įdiekite "Teams" kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite "Vykdyti administratoriaus teisėmis", jei yra).</span><span class="sxs-lookup"><span data-stu-id="d283f-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="d283f-110">Jei jūsų "Teams" klientas vis dar sugenda, ar galite atkurti problemą?</span><span class="sxs-lookup"><span data-stu-id="d283f-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="d283f-111">Jei taip:</span><span class="sxs-lookup"><span data-stu-id="d283f-111">If so:</span></span>

1. <span data-ttu-id="d283f-112">Norėdami užfiksuoti veiksmus, naudokite veiksmų rašytuvą.</span><span class="sxs-lookup"><span data-stu-id="d283f-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="d283f-113">Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.</span><span class="sxs-lookup"><span data-stu-id="d283f-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="d283f-114">Paleiskite veiksmų rašytuvą ir atkartokite problemą prisijungę naudodami paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="d283f-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="d283f-115">[Surinkite komandų žurnalus, kurie užfiksuoja įrašytus pakartotinio pelno veiksmus.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="d283f-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="d283f-116">**Pastaba:** įsitikinkite, kad užfiksuojate paveikto vartotojo prisijungimo adresą.</span><span class="sxs-lookup"><span data-stu-id="d283f-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="d283f-117">Rinkite iškelties ir (arba) gedimų talpyklos informaciją ("Windows").</span><span class="sxs-lookup"><span data-stu-id="d283f-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="d283f-118">Paleiskite "Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas:</span><span class="sxs-lookup"><span data-stu-id="d283f-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="d283f-119">Pridėkite failą prie palaikymo atvejo.</span><span class="sxs-lookup"><span data-stu-id="d283f-119">Attach the file to your support case.</span></span>
