---
title: "\"Intune Win32\" taikomųjų programų diegimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461873"
---
# <a name="intune-win32-app-deployment"></a>"Intune Win32" taikomųjų programų diegimas

"Microsoft Intune" leidžia Win32 taikomąsias programas, įskaitant, bet neapsiribojant, MSI ir. EXE turi būti įdiegtas į "Windows 10" įrenginius. Naudojamam diegimo mechanizmui reikalingas Intune Management Extension (IME) paskirties įrenginyje. IME bus automatiškai įdiegta kaip "PowerShell" scenarijų arba "Win32" taikomųjų programų diegimas vartotojui/įrenginiui.

Taip pat yra išankstinių sąlygų, kurios turi būti įvykdytos norint įdiegti Win32 taikomąsias programas, kurios apima:

- Palaikomos platformos: "Windows 10" versija 1607 arba naujesnė ("Enterprise", "Pro" ir "Education" versijos).
- Palaikoma architektūra: x86 ir x64.
- Įrenginių valdymas: AAD sujungtos ir automatiškai užregistruotos (įskaitant hibridinį domeną, sujungtą su grupe ir grupės strategija).
- Taikomosios programos paketo formatas:. **intunewin**  failas, parengtas ["Microsoft Win32" turinio prep įrankyje](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Apribojimai
    - Maksimalus dydis: 8GB.
    - Nepalaikoma architektūra: ginklai.

Norėdami gauti informacijos, susijusios su tais veiksmais, peržiūrėkite "[Microsoft Intune" Win32 programos "įtraukti, priskirti ir stebėti](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" dok.

Išsami informacija apie taikomųjų programų diegimo sistemoje "Windows", įskaitant "Win32" taikomąsias programas, galima peržiūrėti šiuose dokumentuose

- [Taikomųjų programų diegimo problemų šalinimas](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- ["Win32" taikomųjų programų trikčių šalinimas](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)