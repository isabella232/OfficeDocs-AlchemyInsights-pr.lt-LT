---
title: "\"OneDrive\" gedimų trikčių diagnostika"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749162"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="deb41-102">"OneDrive" gedimų trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="deb41-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="deb41-103">Jei "OneDrive" kelis kartus užstringa, pabandykite atlikti šiuos trikčių šalinimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="deb41-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="deb41-104">**Įsitikinkite, kad registro raktai nenustatti:**</span><span class="sxs-lookup"><span data-stu-id="deb41-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="deb41-105">Naudodami registro rengyklę, eikite į HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="deb41-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="deb41-106">Jei DisableFileSyncNGSC yra ir nustatyta kaip 1, atidarykite raktą ir pakeiskite reikšmę į 0.</span><span class="sxs-lookup"><span data-stu-id="deb41-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="deb41-107">Rankiniu būdu paleiskite "OneDrive" nuėję į pradžios ekraną</span><span class="sxs-lookup"><span data-stu-id="deb41-107">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="deb41-109">, ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" darbalaukio programėlę.</span><span class="sxs-lookup"><span data-stu-id="deb41-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="deb41-110">**Iš naujo nustatyti "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="deb41-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="deb41-111">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="deb41-111">Notes:</span></span>

- <span data-ttu-id="deb41-112">Iš naujo nustačius "OneDrive" atjungimi visi esami sinchronizavimo ryšiai (įskaitant asmeninį "OneDrive", jei nustatyta).</span><span class="sxs-lookup"><span data-stu-id="deb41-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="deb41-113">Nenusirausdami failų ar duomenų iš naujo nustatydami "OneDrive" kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="deb41-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="deb41-114">**Norėdami iš naujo nustatyti "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="deb41-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="deb41-115">Atidarykite dialogo langą Vykdyti paspausdami "Windows" klavišą ir R.</span><span class="sxs-lookup"><span data-stu-id="deb41-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="deb41-116">Įveskite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ir paspauskite Gerai.</span><span class="sxs-lookup"><span data-stu-id="deb41-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="deb41-117">Komandų langas gali pasirodyti trumpai.</span><span class="sxs-lookup"><span data-stu-id="deb41-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="deb41-118">Rankiniu būdu paleiskite "OneDrive" nuėję į pradžios ekraną</span><span class="sxs-lookup"><span data-stu-id="deb41-118">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="deb41-120">, ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" darbalaukio programėlę.</span><span class="sxs-lookup"><span data-stu-id="deb41-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="deb41-121">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="deb41-121">Notes:</span></span>

- <span data-ttu-id="deb41-122">Jei pasirinkote sinchronizuoti tik kai kuriuos aplankus prieš nustatymą iš naujo, turėsite tai padaryti dar kartą, kai sinchronizavimas bus baigtas.</span><span class="sxs-lookup"><span data-stu-id="deb41-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="deb41-123">Skaitykite Norėdami gauti daugiau informacijos, skaitykite [Pasirinkite, kuriuos "OneDrive" aplankus sinchronizuoti su kompiuteriu.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  </span><span class="sxs-lookup"><span data-stu-id="deb41-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="deb41-124">Tai turėsite atlikti asmeniniam "OneDrive" ir "OneDrive" verslui.</span><span class="sxs-lookup"><span data-stu-id="deb41-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>