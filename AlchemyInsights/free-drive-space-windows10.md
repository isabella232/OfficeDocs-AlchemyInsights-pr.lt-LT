---
title: Atlaisvinkite „Windows 10“ disko vietos
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505364"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="38bac-102">Atlaisvinkite „Windows 10“ disko vietos</span><span class="sxs-lookup"><span data-stu-id="38bac-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="38bac-103">Čia pateikiami du būdai, kaip atlaisvinti „Windows“ disko vietos:</span><span class="sxs-lookup"><span data-stu-id="38bac-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="38bac-104">Atlaisvinkite „Windows 10“ disko vietos.</span><span class="sxs-lookup"><span data-stu-id="38bac-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="38bac-105">Atlaisvinkite vietos „Windows 10“ naujinimams naudodami išorinį saugyklos įrenginį.</span><span class="sxs-lookup"><span data-stu-id="38bac-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="38bac-106">Jei vietos diske vis dar mažai net ir išvalius diską, gali būti, jog jūsų aplankas „Temp“ greitai užsipildo programų (.appx) failais, kuriuos naudojat „Microsoft Store“.</span><span class="sxs-lookup"><span data-stu-id="38bac-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="38bac-107">Norėdami išspręsti šią problemą, nustatykite „Store“ iš naujo, išvalykite „Store“ podėlį, o tuomet paleiskite „Windows Update“ trikčių diagnostikos priemonę.</span><span class="sxs-lookup"><span data-stu-id="38bac-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="38bac-108">Prieš pereidami prie kitų žingsnių, įsitikinkite, kad „Microsoft Store“ yra uždaryta.</span><span class="sxs-lookup"><span data-stu-id="38bac-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="38bac-109">**1 žingsnis: „Microsoft Store“ nustatymas iš naujo**</span><span class="sxs-lookup"><span data-stu-id="38bac-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="38bac-110">**Pastaba** Tai visam laikui panaikins įrenginio programų duomenis, įskaitant jūsų nuostatas ir prisijungimo informaciją.</span><span class="sxs-lookup"><span data-stu-id="38bac-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="38bac-111">Pasirinkite **Pradžia** > **Parametrai** > **Programos** > **Programos ir funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="38bac-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="38bac-112">Programų sąraše raskite ir pasirinkite „Microsoft Store“.</span><span class="sxs-lookup"><span data-stu-id="38bac-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="38bac-113">Pasirinkite **Išplėstinės parinktys**.</span><span class="sxs-lookup"><span data-stu-id="38bac-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="38bac-114">Slinkite žemyn ir pasirinkite **Nustatyti iš naujo**, o tuomet **Patvirtinti nustatymą iš naujo**.</span><span class="sxs-lookup"><span data-stu-id="38bac-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="38bac-115">**2 žingsnis: „Microsoft Store“ podėlio išvalymas**</span><span class="sxs-lookup"><span data-stu-id="38bac-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="38bac-116">Paspauskite „Windows“ logotipo klavišą + R, kad atidarytumėte dialogo langą Vykdyti.</span><span class="sxs-lookup"><span data-stu-id="38bac-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="38bac-117">Įveskite wsreset.exe ir pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="38bac-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="38bac-118">Bus atidarytas tuščias langas Komandinė eilutė.</span><span class="sxs-lookup"><span data-stu-id="38bac-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="38bac-119">Praėjus maždaug 10 sekundžių, langas užsidarys ir automatiškai atsidarys „Store“.</span><span class="sxs-lookup"><span data-stu-id="38bac-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="38bac-120">**3 žingsnis: „Windows Update“ nustatymas iš naujo**</span><span class="sxs-lookup"><span data-stu-id="38bac-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="38bac-121">Pasirinkite **Pradžia** > **Parametrai** > **Naujinimas ir sauga** > **Trikčių diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="38bac-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="38bac-122">Slinkite žemyn ir iš sąrašo pasirinkite **„Windows Update“**, tuomet pasirinkite **Paleisti trikčių diagnostiką**.</span><span class="sxs-lookup"><span data-stu-id="38bac-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="38bac-123">Paleiskite kompiuterį iš naujo ir patikrinkite, ar vis dar susiduriate su problema.</span><span class="sxs-lookup"><span data-stu-id="38bac-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

