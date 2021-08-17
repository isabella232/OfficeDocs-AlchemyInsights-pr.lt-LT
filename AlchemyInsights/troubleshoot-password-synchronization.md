---
title: Slaptažodžių sinchronizavimo trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105763"
---
# <a name="troubleshoot-password-synchronization"></a>Slaptažodžių sinchronizavimo trikčių šalinimas

Norėdami šalinti slaptažodžių sinchronizavimo problemas, pradėkite naudodami šią AAD Prisijungimas trikčių diagnostikos užduotį, kad nustatytumėte, kodėl slaptažodžiai nesinchronizuojami. Norėdami pradėti, eikite į [Tiesioginio sinchronizavimo valdymas](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Atidarykite naują Windows PowerShell seansą "Azure AD Prisijungimas serveryje ir pasirinkite **parinktį Vykdyti administratoriaus** teisėmis.

2. Paleiskite Set-ExecutionPolicy RemoteSigned" arba Set-ExecutionPolicy neribotas.

3. Paleiskite "Azure AD" Prisijungimas vediklį.

4. Eikite į puslapį Papildomos užduotys, > **Šalinti**  >  **paskesnį trikčių diagnostiką.**

5. Pasirinkite **Paleisti,** kad atidarytumėte "PowerShell" trikčių diagnostikos meniu.

6. Pasirinkite **Šalinti slaptažodžių sinchronizavimo triktis**.

    Paprastai problema yra ta, kad konkrečios vartotojo paskyros slaptažodis nesinchronizuojamas.

    **Pastabos** Slaptažodžio sinchronizavimas nepavyko, jei paskutinį kartą sėkmingai sinchronizuotas slaptažodis buvo prieš kurį laiką.

Daugiau informacijos apie slaptažodžių sinchronizavimo trikčių diagnostiką žr. [Slaptažodžių hash sinchronizavimo trikčių šalinimas naudojant "Azure AD" Prisijungimas sinchronizavimą](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).