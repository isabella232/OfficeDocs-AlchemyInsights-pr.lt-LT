---
title: Spausdinimo kaupos problema išspręsta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801849"
---
# <a name="print-spooler-issue-is-resolved"></a>Spausdinimo kaupos problema išspręsta

Jei jūsų įrenginys buvo atnaujintas naudojant "Windows 10"  **OS komponavimo versiją 19041,329**, galite pastebėti problemą, dėl kurios kai kurie spausdintuvai nesugeba spausdinti. Spausdinimo kaupos programa gali mesti klaidą arba uždaryti netikėtai, kai bandote spausdinti, o išvesties nėra iš susijusio spausdintuvo. Ši problema išspręsta "OS Build  **19041,331**", [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Vykstantis tyrimas**

Vietinio saugos tarnybos posistemės tarnybos (LSASS) failas (**Isass.exe**) gali nepavykti kai kuriuose įrenginiuose su klaidos pranešimu "kritinis sistemos procesas, C:\WINDOWS\system32\Isass.exe, nepavyko dėl būsenos kodo c0000008. Dabar kompiuteris turi būti paleistas iš naujo ".  **"Microsoft" dirba su rezoliucija ir pateiks naujinimą būsimame leidime.**

Daugiau informacijos rasite  ["Windows 10" versijoje 2004 žinomos problemos](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).