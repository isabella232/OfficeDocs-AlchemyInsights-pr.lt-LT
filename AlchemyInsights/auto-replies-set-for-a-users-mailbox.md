---
title: Automatinių atsakymų nustatymas pašto dėžutei
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046616"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Automatinių atsakymų nustatymas vartotojo pašto dėžutei

**1 būdas**

1. Prisijunkite prie „Microsoft 365“ portalo.

2. Eikite į **Vartotojai > Aktyvūs vartotojai** (arba **Grupės > Bendrinamos pašto dėžutės**, jei nustatote bendrai naudojamai pašto dėžutei).

3. Pasirinkite vartotoją, kuris turi „Microsoft Exchange“ pašto dėžutę.

4. Dešiniajame išskleidžiamajame meniu eikite į **Pašto parametrai > Automatiniai atsakymai** (jei tai bendrinama pašto dėžutė, išskleidžiamajame meniu spustelėkite **Automatiniai atsakymai**).

**2 būdas**

1. Prisijunkite prie „Microsoft 365“ administravimo portalo naudodami administratoriaus kredencialus.

2. Išplėskite **Administravimo centrai**, tada spustelėkite **Exchange**.

3. Viršutiniame dešiniajame kampe spustelėkite paveikslėlį, spustelėkite **Kitas vartotojas**, tada pasirinkite vartotojo pašto dėžutę, kurią norite keisti.

4. Kairiojoje pusėje pasirinkite **Parinktys**, spustelėkite **Tvarkyti el. paštą**, tada spustelėkite **Automatiniai atsakymai.**

**3 būdas**

„Exchange Online PowerShell“ vykdykite tolesnę cmdlet:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Daugiau informacijos apie šią cmdlet žr. [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
