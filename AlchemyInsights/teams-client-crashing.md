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
# <a name="teams-client-crashing"></a><span data-ttu-id="ade4b-102">Genda „Teams“ klientas?</span><span class="sxs-lookup"><span data-stu-id="ade4b-102">Teams client crashing?</span></span>

<span data-ttu-id="ade4b-103">Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="ade4b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="ade4b-104">Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="ade4b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="ade4b-105">Įsitikinkite, kad visi ["Microsoft 365" URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) yra pasiekiami.</span><span class="sxs-lookup"><span data-stu-id="ade4b-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="ade4b-106">Prisijunkite naudodami nuomotojo administratoriaus abonementą ir patikrinkite [savo tarnybos sveikatos ataskaitų sritį,](https://docs.microsoft.com/office365/enterprise/view-service-health) kad patikrintumėte, ar nėra atjungimo ar tarnybos pablogėjimo.</span><span class="sxs-lookup"><span data-stu-id="ade4b-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="ade4b-107">"Teams" taikomosios programos pašalinimas ir diegimas iš naujo (saitas)</span><span class="sxs-lookup"><span data-stu-id="ade4b-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="ade4b-108">Raskite aplanką %appdata%\Microsoft\teams\ savo kompiuteryje ir panaikinkite visus tame kataloge esančius failus.</span><span class="sxs-lookup"><span data-stu-id="ade4b-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="ade4b-109">[Atsisiųskite ir įdiekite "Teams" programą](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ir, jei įmanoma, įdiekite "Teams" kaip administratorius (dešiniuoju pelės mygtuku spustelėkite "Teams" diegimo programą ir pasirinkite "Paleisti administratoriaus teisėmis", jei yra).</span><span class="sxs-lookup"><span data-stu-id="ade4b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="ade4b-110">Jei jūsų komandos klientas vis dar genda, ar galite atkurti problemą?</span><span class="sxs-lookup"><span data-stu-id="ade4b-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="ade4b-111">Jei taip:</span><span class="sxs-lookup"><span data-stu-id="ade4b-111">If so:</span></span>

1. <span data-ttu-id="ade4b-112">Norėdami užfiksuoti veiksmus, atlikite veiksmus.</span><span class="sxs-lookup"><span data-stu-id="ade4b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="ade4b-113">Uždarykite visas nereikalingas arba konfidencialias taikomąsias programas.</span><span class="sxs-lookup"><span data-stu-id="ade4b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="ade4b-114">Paleiskite veiksmų rašytuvą ir atkurkite problemą, kai prisijungė tedininkas su susijusio vartotojo abonementą.</span><span class="sxs-lookup"><span data-stu-id="ade4b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="ade4b-115">[Rinkti komandos žurnalus, kad užfiksuoti įrašytus repro veiksmus](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="ade4b-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="ade4b-116">**Pastaba:** įsitikinkite, kad fiksuojate paveikto naudotojo prisijungimo adresą.</span><span class="sxs-lookup"><span data-stu-id="ade4b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="ade4b-117">Rinkti iškelties ir / arba gedimų kibirą informacija (Windows).</span><span class="sxs-lookup"><span data-stu-id="ade4b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="ade4b-118">Paleiskite "Windows PowerShell" kompiuteryje, kuriame įvyksta gedimas, ir vykdykite šias komandas:</span><span class="sxs-lookup"><span data-stu-id="ade4b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="ade4b-119">Pridėkite failą prie palaikymo atvejo.</span><span class="sxs-lookup"><span data-stu-id="ade4b-119">Attach the file to your support case.</span></span>
