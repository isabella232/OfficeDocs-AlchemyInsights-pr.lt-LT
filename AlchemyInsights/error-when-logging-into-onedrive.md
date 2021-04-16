---
title: 0x8004de40 klaida paleidžiant "OneDrive"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813660"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="a7e62-102">0x8004de40 klaida paleidžiant "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="a7e62-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="a7e62-103">Jei gaunate klaidos pranešimą **0x8004de40** "OneDrive", iš naujo paleiskite kompiuterį prisijungę prie darbo arba mokymo įstaigos domeno.</span><span class="sxs-lookup"><span data-stu-id="a7e62-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="a7e62-104">Jei gaunate šią klaidą iš naujo paleidę kompiuterį, pabandykite tai padaryti prisijungę prie savo darbo arba mokymo įstaigos domeno:</span><span class="sxs-lookup"><span data-stu-id="a7e62-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="a7e62-105">Spustelėkite Pradėti ir ieškos **lauke įveskite cmd** **arba komandinę**  eilutę, dešiniuoju pelės mygtuku spustelėkite komandinės eilutės taikomąją programą ir pasirinkite  **Vykdyti administratoriaus teisėmis**.</span><span class="sxs-lookup"><span data-stu-id="a7e62-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="a7e62-106">Jei būsite paraginti įvesti administratoriaus slaptažodį arba patvirtinti, įveskite slaptažodį arba spustelėkite **Leisti**.</span><span class="sxs-lookup"><span data-stu-id="a7e62-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="a7e62-107">Komandinės eilutės lange įveskite **dsregcmd /leave**  ir palaukite, kol bus baigta komanda.</span><span class="sxs-lookup"><span data-stu-id="a7e62-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="a7e62-108">Tada įveskite **dsregcmd /join ir** palaukite, kol bus baigta komanda.</span><span class="sxs-lookup"><span data-stu-id="a7e62-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="a7e62-109">Iš naujo paleiskite kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="a7e62-109">Reboot your computer.</span></span>
