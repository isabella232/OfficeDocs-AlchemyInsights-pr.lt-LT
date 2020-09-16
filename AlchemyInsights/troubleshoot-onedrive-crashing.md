---
title: "\"OneDrive\" gedimų šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665006"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="eeebf-102">"OneDrive" gedimų šalinimas</span><span class="sxs-lookup"><span data-stu-id="eeebf-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="eeebf-103">Jei "OneDrive" kelis kartus sugenda, išbandykite šiuos trikčių šalinimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="eeebf-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="eeebf-104">**Įsitikinkite, kad registro raktų nėra nustatyta:**</span><span class="sxs-lookup"><span data-stu-id="eeebf-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="eeebf-105">Naudodami registro rengyklę eikite į HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="eeebf-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="eeebf-106">Jei yra "Disablefilesyncntgs" ir nustatote 1, atidarykite raktą ir pakeiskite reikšmę į 0.</span><span class="sxs-lookup"><span data-stu-id="eeebf-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="eeebf-107">Neautomatiškai paleiskite "OneDrive" nuėję į pradžios ekraną</span><span class="sxs-lookup"><span data-stu-id="eeebf-107">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="eeebf-109">, ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" kompiuterio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="eeebf-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="eeebf-110">**Iš naujo nustatyti "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="eeebf-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="eeebf-111">Pastabų</span><span class="sxs-lookup"><span data-stu-id="eeebf-111">Notes:</span></span>

- <span data-ttu-id="eeebf-112">Iš naujo nustačius "OneDrive", Atjungiami visi esami sinchronizavimo ryšiai (įskaitant asmeninę "OneDrive", jei nustatyta).</span><span class="sxs-lookup"><span data-stu-id="eeebf-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="eeebf-113">Neprarasite failų arba duomenų iš naujo nustatydami "OneDrive" savo kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="eeebf-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="eeebf-114">**Norėdami iš naujo nustatyti "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="eeebf-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="eeebf-115">Atidarykite dialogo langą vykdyti paspausdami "Windows" klavišą ir R.</span><span class="sxs-lookup"><span data-stu-id="eeebf-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="eeebf-116">Įveskite% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset ir paspauskite Gerai.</span><span class="sxs-lookup"><span data-stu-id="eeebf-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="eeebf-117">Gali būti trumpai rodomas komandos langas.</span><span class="sxs-lookup"><span data-stu-id="eeebf-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="eeebf-118">Neautomatiškai paleiskite "OneDrive" nuėję į pradžios ekraną</span><span class="sxs-lookup"><span data-stu-id="eeebf-118">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="eeebf-120">, ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" kompiuterio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="eeebf-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="eeebf-121">Pastabų</span><span class="sxs-lookup"><span data-stu-id="eeebf-121">Notes:</span></span>

- <span data-ttu-id="eeebf-122">Jei pasirinkote sinchronizuoti tik kai kuriuos aplankus prieš iš naujo, turėsite tai padaryti dar kartą baigus sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="eeebf-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="eeebf-123">Norėdami gauti daugiau informacijos, skaitykite [pasirinkite, kuriuos "OneDrive" aplankus sinchronizuoti su savo kompiuteriu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="eeebf-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="eeebf-124">Turėsite tai atlikti asmeniniams "OneDrive" ir "OneDrive" verslui.</span><span class="sxs-lookup"><span data-stu-id="eeebf-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>