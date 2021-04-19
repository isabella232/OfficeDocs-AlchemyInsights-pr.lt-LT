---
title: "\"Windows\" atminties diagnostikos paleidimas sistemoje \"Windows 10\""
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826675"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="3fed5-102">"Windows" atminties diagnostikos paleidimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="3fed5-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="3fed5-103">Jei "Windows" ir kompiuterio programėlės sugenda, užstringa arba veikia nestabiliai, gali kilti kompiuterio atminties (RAM) problemų.</span><span class="sxs-lookup"><span data-stu-id="3fed5-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="3fed5-104">Galite paleisti "Windows" atminties diagnostiką, kad patikrinsite kompiuterio RAM problemas.</span><span class="sxs-lookup"><span data-stu-id="3fed5-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="3fed5-105">Užduočių juostos ieškos lauke įveskite atminties **diagnostika**, tada pasirinkite **"Windows" atminties diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="3fed5-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="3fed5-106">Norėdami vykdyti diagnostiką, kompiuteris turi būti paleistas iš naujo.</span><span class="sxs-lookup"><span data-stu-id="3fed5-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="3fed5-107">Turite galimybę iš naujo paleisti iš karto (pirmiausia įrašykite savo darbą ir uždarykite atidarytus dokumentus ir el. laiškus) arba suplanuoti diagnostiką, kad ji būtų vykdoma automatiškai, kai kompiuteris bus paleistas iš naujo:</span><span class="sxs-lookup"><span data-stu-id="3fed5-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

!["Windows" atminties diagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="3fed5-109">Kai kompiuteris bus paleistas iš naujo, **"Windows" atminties diagnostikos įrankis** bus paleistas automatiškai.</span><span class="sxs-lookup"><span data-stu-id="3fed5-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="3fed5-110">Būsena ir eiga bus rodomi kaip diagnostika, o jūs turite galimybę atšaukti diagnostiką paspaudus **klaviatūros klavišą ESC.**</span><span class="sxs-lookup"><span data-stu-id="3fed5-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="3fed5-111">Kai diagnostika bus baigta, "Windows" pradės įprastai.</span><span class="sxs-lookup"><span data-stu-id="3fed5-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="3fed5-112">Iš karto po paleidimo iš naujo, kai rodomas  darbalaukis, bus rodomas pranešimas (užduočių juostoje šalia veiksmų centro piktogramos), nurodantis, ar rasta atminties klaidų.</span><span class="sxs-lookup"><span data-stu-id="3fed5-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="3fed5-113">Toliau pateikiami pavyzdžiai.</span><span class="sxs-lookup"><span data-stu-id="3fed5-113">For example:</span></span>

<span data-ttu-id="3fed5-114">Štai veiksmų centro piktograma:</span><span class="sxs-lookup"><span data-stu-id="3fed5-114">Here's the Action Center icon:</span></span> ![Veiksmų centro piktograma](media/action-center-icon.png) 

<span data-ttu-id="3fed5-116">Ir pranešimo pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="3fed5-116">And a sample notification:</span></span> ![Nėra atminties klaidų](media/no-memory-errors.png)

<span data-ttu-id="3fed5-118">Jei praleidote pranešimą, užduočių juostoje galite pasirinkti veiksmų centro piktogramą, kad būtų rodomas veiksmų **centras** ir rodomas slenkamas pranešimų sąrašas. </span><span class="sxs-lookup"><span data-stu-id="3fed5-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="3fed5-119">Norėdami peržiūrėti išsamią informaciją, **įveskite įvykį** užduočių juostos ieškos lauke, tada pasirinkite Įvykių **peržiūros programa**.</span><span class="sxs-lookup"><span data-stu-id="3fed5-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="3fed5-120">Įvykių **peržiūros programos kairiojoje** srityje eikite į **"Windows" žurnalai > Sistema**.</span><span class="sxs-lookup"><span data-stu-id="3fed5-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="3fed5-121">Dešiniosios srities srityje nuskaitykite sąrašą žiūrėdami į stulpelį Šaltinis, kol pamatysite įvykius su šaltinio reikšme **MemoryDiagnostics-Results**. </span><span class="sxs-lookup"><span data-stu-id="3fed5-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="3fed5-122">Pažymėkite kiekvieną tokį įvykį ir peržiūrėkite rezultato informaciją lauke **po skirtuku Bendra** po sąrašu.</span><span class="sxs-lookup"><span data-stu-id="3fed5-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
