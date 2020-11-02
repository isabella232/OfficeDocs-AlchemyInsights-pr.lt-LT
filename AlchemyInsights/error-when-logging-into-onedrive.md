---
title: 0x8004de40 klaida paleidžiant "OneDrive"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823111"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="9e66e-102">0x8004de40 klaida paleidžiant "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="9e66e-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="9e66e-103">Jei gaunate klaidos pranešimą **0x8004de40** , kai prisijungiate prie "OneDrive", iš naujo paleiskite kompiuterį prisijungę prie savo darbo arba mokymo įstaigos domeno.</span><span class="sxs-lookup"><span data-stu-id="9e66e-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="9e66e-104">Jei gaunate šią klaidą paleidę kompiuterį iš naujo, Išbandykite tai būdami prisijungę prie savo darbo arba mokymo įstaigos domeno:</span><span class="sxs-lookup"><span data-stu-id="9e66e-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="9e66e-105">Spustelėkite pradėti, tada ieškos lauke įveskite **cmd** arba **Komandinė eilutė**  , dešiniuoju pelės mygtuku spustelėkite Komandinė eilutė ir pasirinkite  **paleisti kaip administratoriui** .</span><span class="sxs-lookup"><span data-stu-id="9e66e-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="9e66e-106">Jei esate raginami įvesti administratoriaus slaptažodį arba patvirtinti, įveskite slaptažodį arba spustelėkite **leisti** .</span><span class="sxs-lookup"><span data-stu-id="9e66e-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="9e66e-107">Lange Komandinė eilutė įveskite **dsregcmd/Leave**  ir palaukite, kol komanda bus baigta.</span><span class="sxs-lookup"><span data-stu-id="9e66e-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="9e66e-108">Tada įveskite **dsregcmd/Join** ir palaukite, kol komanda bus baigta.</span><span class="sxs-lookup"><span data-stu-id="9e66e-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="9e66e-109">Iš naujo paleiskite kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="9e66e-109">Reboot your computer.</span></span>
