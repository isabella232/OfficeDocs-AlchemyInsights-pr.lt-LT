---
title: Spausdinimo kaupos problema išspręsta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088401"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="2e69d-102">Spausdinimo kaupos problema išspręsta</span><span class="sxs-lookup"><span data-stu-id="2e69d-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="2e69d-103">Jei jūsų įrenginys buvo atnaujintas naudojant "Windows 10 **OS Build 19041.329",** galbūt pastebėjote problemą, dėl kurios tam tikriems spausdintuvams nepavyksta spausdinti.</span><span class="sxs-lookup"><span data-stu-id="2e69d-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="2e69d-104">Spausdinimo kaupos programa gali mesti klaidą arba netikėtai uždaryti bandant spausdinti, ir nėra išvesties iš susijusio spausdintuvo.</span><span class="sxs-lookup"><span data-stu-id="2e69d-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="2e69d-105">Ši problema išspręsta OS komponavimo versijos **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="2e69d-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="2e69d-106">**Vykdomas tyrimas**</span><span class="sxs-lookup"><span data-stu-id="2e69d-106">**Ongoing investigation**</span></span>

<span data-ttu-id="2e69d-107">Vietinės saugos tarnybos posistemės tarnybos (LSASS) failas (**Isass.exe**) gali nepavykti kai kuriuose įrenginiuose su klaidos pranešimu "Kritinis sistemos procesas, C:\WINDOWS\system32\Isass.exe nepavyko dėl būsenos kodo c0000008.</span><span class="sxs-lookup"><span data-stu-id="2e69d-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="2e69d-108">Dabar mašiną reikia paleisti iš naujo".</span><span class="sxs-lookup"><span data-stu-id="2e69d-108">The machine must now be restarted".</span></span>  <span data-ttu-id="2e69d-109">**"Microsoft" dirba su rezoliucija ir pateiks naujinimą būsimame leidime.**</span><span class="sxs-lookup"><span data-stu-id="2e69d-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="2e69d-110">Norėdami gauti daugiau informacijos, prašome patikrinti [Windows 10 versija 2004 žinomos problemos](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="2e69d-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>