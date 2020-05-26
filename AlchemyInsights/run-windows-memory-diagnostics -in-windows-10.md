---
title: "\"Windows\" atminties diagnostikos paleidimas sistemoje \"Windows 10\""
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357788"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="c5ca3-102">"Windows" atminties diagnostikos paleidimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="c5ca3-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="c5ca3-103">Jei "Windows" ir kompiuterio programėlės genda, užstringa arba veikia nestabiliai, gali būti, kad kilo kompiuterio atminties (RAM) problemų.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="c5ca3-104">Galite paleisti "Windows" atminties diagnostiką ir patikrinti, ar nėra kompiuterio RAM problemų.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="c5ca3-105">Užduočių juostos ieškos lauke įveskite **atminties diagnostika**, tada pasirinkite **"Windows" atminties diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="c5ca3-106">Norint paleisti diagnostiką, kompiuteris turi būti paleistas iš naujo.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="c5ca3-107">Jūs turite galimybę iš naujo paleisti iš karto (prašome įrašyti savo darbą ir uždaryti atidarytus dokumentus ir elektroninius laiškus pirmą kartą) arba suplanuoti diagnostikos paleisti automatiškai, kai kitą kartą kompiuteris bus paleistas iš naujo:</span><span class="sxs-lookup"><span data-stu-id="c5ca3-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

!["Windows" atminties diagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="c5ca3-109">Kai kompiuteris bus paleistas iš naujo, **"Windows" atminties diagnostikos įrankis** veiks automatiškai.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="c5ca3-110">Būsena ir eiga bus rodoma vykdant diagnostiką, o jūs turite galimybę atšaukti diagnostiką pataikyti į **klaviatūros KLAVIŠĄ ESC.**</span><span class="sxs-lookup"><span data-stu-id="c5ca3-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="c5ca3-111">Kai diagnostika bus baigta, sistema Windows bus paleista įprastai.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="c5ca3-112">Iškart po paleidimo iš naujo, kai pasirodo darbalaukis, pasirodys pranešimas (šalia **užduočių centro** piktogramos užduočių juostoje), nurodantis, ar rasta atminties klaidų.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="c5ca3-113">Pavyzdžiui:</span><span class="sxs-lookup"><span data-stu-id="c5ca3-113">For example:</span></span>

<span data-ttu-id="c5ca3-114">Toliau nurodyta veiksmų centro piktograma:</span><span class="sxs-lookup"><span data-stu-id="c5ca3-114">Here's the Action Center icon:</span></span> ![Veiksmų centro piktograma](media/action-center-icon.png) 

<span data-ttu-id="c5ca3-116">Ir pranešimo pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="c5ca3-116">And a sample notification:</span></span> ![Nėra atminties klaidų](media/no-memory-errors.png)

<span data-ttu-id="c5ca3-118">Jei praleidote pranešimą, užduočių juostoje galite pasirinkti **veiksmų centro** piktogramą, kad būtų rodomas **veiksmų centras,** ir peržiūrėti slenkamatį pranešimų sąrašą.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="c5ca3-119">Norėdami peržiūrėti išsamią informaciją, užduočių juostos ieškos lauke įveskite **įvykis,** tada pasirinkite **Įvykių peržiūros programa**.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="c5ca3-120">Įvykių **peržiūros programos**kairiojoje srityje eikite į **"Windows" žurnalus > sistema**.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="c5ca3-121">Dešiniojoje srityje nuskaitykite sąrašą žiūrėdami į stulpelį **Šaltinis,** kol pamatysite įvykius, kurių šaltinio reikšmė **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="c5ca3-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="c5ca3-122">Pažymėkite kiekvieną tokį įvykį ir pamatyti rezultatų informaciją laukelyje po sąrašu esančiame skirtuke **Bendra.**</span><span class="sxs-lookup"><span data-stu-id="c5ca3-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
