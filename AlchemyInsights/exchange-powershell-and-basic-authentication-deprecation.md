---
title: „Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015697"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>„Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas

Naujausios informacijos apie tai, kaip prisijungti prie „Exchange Online PowerShell“ nenaudojant bazinio autentifikavimo, [eikite čia](https://aka.ms/psbasicauth).

Atkreipkite dėmesį, kad Pagrindinis autentifikavimas vis dar turi būti įgalintas jūsų kliento kompiuteryje.
Naujasis „PowerShell v2“ modulis naudoja modernią autentifikavimo funkciją, kad būtų galima įjungti visas REST pagrįstas „V2 Cmdlet“ dalis. Be „V2 Cmdlet“, taip pat suteikia galimybę pasiekti senesnes nuotolinės „PowerShell“ (RPS) „Cmdlet“, kurioms nustatyti reikalingas nuotolinis „PowerShell“ seansas. „Windows“ kompiuteryje kuriant RPS seansą reikia, kad „WinRM BasicAuth“ būtų įgalintas kliento kompiuteryje, nors modulis naudoja modernią autentifikavimo mechanizmą, kad autentifikuotų tarnybą. „WinRM Basic Auth“ srautas naudojamas šiuolaikiniams autentifikavimo žetonams perduoti. Jei „WinRM Basic Auth“ išjungtas kliento kompiuteryje, nauja „V2 cmdlet“ ir toliau veiks (bet senesnė „RPS cmdlet“ – ne).
