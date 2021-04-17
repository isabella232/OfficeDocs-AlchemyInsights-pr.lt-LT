---
title: "\"OneDrive\" gedimų šalinimas"
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826207"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="a891c-102">"OneDrive" gedimų šalinimas</span><span class="sxs-lookup"><span data-stu-id="a891c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="a891c-103">Jei "OneDrive" kelis kartus sugenda, pabandykite atlikti šiuos trikčių šalinimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a891c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="a891c-104">**Įsitikinkite, kad registro raktai nėra nustatyti:**</span><span class="sxs-lookup"><span data-stu-id="a891c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="a891c-105">Naudodami registro rengyklę eikite į HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="a891c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="a891c-106">Jei Yra DisableFileSyncNGSC ir nustatyta kaip 1, atidarykite raktą ir pakeiskite reikšmę į 0.</span><span class="sxs-lookup"><span data-stu-id="a891c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="a891c-107">Rankiniu būdu paleiskite "OneDrive" nueidami į Pradžia</span><span class="sxs-lookup"><span data-stu-id="a891c-107">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a891c-109">, ieškos lauke įveskite OneDrive, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="a891c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a891c-110">**"OneDrive" nustatymas iš naujo:**</span><span class="sxs-lookup"><span data-stu-id="a891c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="a891c-111">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="a891c-111">Notes:</span></span>

- <span data-ttu-id="a891c-112">Iš naujo nustačius "OneDrive", atjungiami visi esami sinchronizavimo ryšiai (įskaitant asmeninę "OneDrive", jei nustatyta).</span><span class="sxs-lookup"><span data-stu-id="a891c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="a891c-113">Iš naujo nustatydami "OneDrive" kompiuteryje neprarasite failų ar duomenų.</span><span class="sxs-lookup"><span data-stu-id="a891c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="a891c-114">**Norėdami iš naujo nustatyti "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="a891c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="a891c-115">Atidarykite dialogo langą Vykdyti paspausdami "Windows" klavišą ir R.</span><span class="sxs-lookup"><span data-stu-id="a891c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="a891c-116">Įveskite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ir paspauskite Gerai.</span><span class="sxs-lookup"><span data-stu-id="a891c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="a891c-117">Komandos langas gali būti rodomas trumpai.</span><span class="sxs-lookup"><span data-stu-id="a891c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="a891c-118">Rankiniu būdu paleiskite "OneDrive" nueidami į Pradžia</span><span class="sxs-lookup"><span data-stu-id="a891c-118">Manually launch OneDrive by going to Start</span></span> ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a891c-120">, ieškos lauke įveskite OneDrive, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="a891c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a891c-121">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="a891c-121">Notes:</span></span>

- <span data-ttu-id="a891c-122">Jei prieš iš naujo nustatę sinchronizavimą pasirinkote sinchronizuoti tik kai kuriuos aplankus, turėsite tai padaryti dar kartą, kai bus baigtas sinchronizavimas.</span><span class="sxs-lookup"><span data-stu-id="a891c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="a891c-123">Norėdami [gauti daugiau informacijos, skaitykite Pasirinkite, kuriuos "OneDrive" aplankus](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)sinchronizuoti su jūsų   kompiuteriu.</span><span class="sxs-lookup"><span data-stu-id="a891c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="a891c-124">Turėsite tai atlikti asmeninėje "OneDrive" ir "OneDrive" verslui.</span><span class="sxs-lookup"><span data-stu-id="a891c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>