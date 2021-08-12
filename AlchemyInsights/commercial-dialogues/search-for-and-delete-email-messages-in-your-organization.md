---
title: El. laiškų ieška ir naikinimas organizacijoje
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948891"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>El. laiškų ieška ir naikinimas organizacijoje

Atlikite šiuos veiksmus:

1. Jei esate ne visuotinis administratorius, norėdami ieškoti pranešimų, jūsų paskyra turi būti įtraukta į **el.** duomenų aptikimo tvarkytuvo vaidmenų grupę arba **atitikties ieškos valdymo vaidmenį**. Norėdami panaikinti laiškus, turėsite prisijungti prie organizacijos **valdymo vaidmenų grupės** arba **ieškos ir valymo valdymo vaidmens.** Šių vaidmenų teisės priskiriamos saugos ir [& centre.](https://protection.office.com)
2. [Sukurkite turinio iešką,](https://docs.microsoft.com/office365/securitycompliance/content-search) kad rastumėte pranešimą, kurį norite panaikinti.
3. [Prisijungimas į saugos & "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Jei naudojate MFA, žr. šias instrukcijas: ["Prisijungimas" & centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Panaikinkite pranešimą: paleiskite `New-ComplianceSearchAction` "cmdlet", kad panaikinsite pranešimą. Panaikinti laiškai perkeliami į vartotojo aplanką Atkuriami elementai. Pavyzdinės komandos žr. [3 veiksmas: pranešimo naikinimas.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
