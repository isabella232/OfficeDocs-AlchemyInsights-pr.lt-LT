---
title: „Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813480"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>„Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas

Naujausios informacijos apie tai, kaip prisijungti prie „Exchange Online PowerShell“ nenaudojant bazinio autentifikavimo, [eikite čia](https://aka.ms/exops-docs). „PowerShell V2“ modulis nenaudoja bazinio autentifikavimo.

Atkreipkite dėmesį, kad Pagrindinis autentifikavimas vis dar turi būti įgalintas jūsų kliento kompiuteryje.
Naujasis „PowerShell v2“ modulis naudoja modernią autentifikavimo funkciją, kad būtų galima įjungti visas REST pagrįstas „V2 Cmdlet“ dalis. Be „V2 Cmdlet“, taip pat suteikia galimybę pasiekti senesnes nuotolinės „PowerShell“ (RPS) „Cmdlet“, kurioms nustatyti reikalingas nuotolinis „PowerShell“ seansas. „Windows“ kompiuteryje kuriant RPS seansą reikia, kad „WinRM BasicAuth“ būtų įgalintas kliento kompiuteryje, nors modulis naudoja modernią autentifikavimo mechanizmą, kad autentifikuotų tarnybą. „WinRM Basic Auth“ srautas naudojamas šiuolaikiniams autentifikavimo žetonams perduoti. Jei „WinRM Basic Auth“ išjungtas kliento kompiuteryje, nauja „V2 cmdlet“ ir toliau veiks (bet senesnė „RPS cmdlet“ – ne).
