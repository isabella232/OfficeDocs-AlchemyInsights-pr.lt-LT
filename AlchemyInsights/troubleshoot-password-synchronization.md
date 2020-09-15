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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664934"
---
# <a name="troubleshoot-password-synchronization"></a>Slaptažodžių sinchronizavimo trikčių šalinimas

Norėdami šalinti Slaptažodžių sinchronizavimo problemas, pradėkite naudodami šį AAD prijungti trikčių diagnostikos užduotį, kad nustatytumėte, kodėl slaptažodžiai nesinchronizuojami. Norėdami pradėti, eikite į [valdyti tiesioginį sinchronizavimą](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Atidarykite naują "Windows PowerShell" seansą savo "Azure AD Connect" serveryje ir pasirinkite parinktį **vykdyti kaip administratoriui** .

2. Vykdyti Set-Execucionpolicy Remotepasirašė arba Set-Execucionpolicy neribojama.

3. Paleiskite "Azure AD Connect" vediklį.

4. Eikite į puslapį papildomos užduotys > **trikčių diagnostika**  >  **toliau**.

5. Pasirinkite **Paleistis** , kad atidarytumėte "PowerShell" trikčių diagnostikos meniu.

6. Pasirinkite **Šalinti slaptažodžių sinchronizavimą**.

    Paprastai problema yra ta, kad slaptažodis nesinchronizuotas konkrečiam vartotojo abonementui.

    **Pastabos** Slaptažodžio sinchronizavimas nutrūksta, jei prieš kurį laiką buvo sukurtas Paskutinis sėkmingas slaptažodžių sinchronizavimas.

Jei turite daugiau pagalbos trikčių diagnostikos slaptažodžio sinchronizavimo, žiūrėkite [slaptažodžių maišos sinchronizavimo su "AZURE AD Connect" sinchronizavimo trikčių diagnostika](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).