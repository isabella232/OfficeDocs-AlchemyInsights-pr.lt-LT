---
title: Slaptažodžių sinchronizavimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387885"
---
# <a name="troubleshoot-password-synchronization"></a>Slaptažodžių sinchronizavimo trikčių diagnostika

Norėdami pašalinti slaptažodžių sinchronizavimo problemas, pradėkite naudoti šią AAD prisijungimo trikčių šalinimo užduotį, kad nustatytumėte, kodėl slaptažodžiai nesinchronizuojami. Norėdami pradėti, eikite į [Tvarkyti tiesioginį sinchronizavimą](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Atidarykite naują "Windows PowerShell" seansą savo "Azure AD Connect" serveryje ir pasirinkite parinktį **Paleisti administratoriaus teisėmis.**

2. Paleiskite Set-ExecutionPolicy RemoteSigned arba Set-ExecutionPolicy Unrestricted.

3. Paleiskite Azure AD Connect vedlį.

4. Eikite į puslapį Papildomos užduotys > **Šalinti**  >  **triktis toliau**.

5. Pasirinkite **Paleisti,** kad atidarytumėte "PowerShell" trikčių diagnostikos meniu.

6. Pasirinkite **Slaptažodžių sinchronizavimo trikčių diagnostika**.

    Problema yra paprastai, kad slaptažodis nėra sinchronizuojami tam tikrą vartotojo abonementą.

    **Pastabos** Slaptažodžio sinchronizavimas nepavyksta, jei paskutinis sėkmingas slaptažodžio sinchronizavimas buvo prieš kurį laiką.

Daugiau pagalbos dėl slaptažodžių sinchronizavimo trikčių diagnostika, [peržiūrėkite slaptažodžio maišos sinchronizavimo su "Azure AD Connect" sinchronizavimo trikčių diagnostika](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).