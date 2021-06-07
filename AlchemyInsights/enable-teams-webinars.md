---
title: Žiniatinklio Teams įgalinkite
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793785"
---
# <a name="enable-teams-webinars"></a>Žiniatinklio Teams įgalinkite

Žiniatinklio seminarai įgalinami pagal numatytuosius parametrus. Galite valdyti, kas gali planuoti ir registruotis žiniatinklio Teams naudodami "Teams PowerShell" komandas.

- Visi vartotojai, kurie gali kurti susitikimą, taip pat gali sukurti internetinio seminaro susitikimą. Jei norite valdyti, kas gali planuoti žiniatinklio Teams, naudokite *AllowMeetingRegistration*. 
- Pagal numatytuosius *nustatymus "WhoCanRegister"* yra įgalintas ir nustatytas **kaip Visi**. Jei norite išjungti susitikimo registraciją, *nustatykite AllowMeetingRegistration kaip* **False**.

Norėdami pakeisti šiuos parametrus, turite įdiegti ["Teams PowerShell".](/microsoftteams/teams-powershell-install) Be to, susitikimo strategijos yra vykdomos Teams žiniatinklio seminaruose. Pavyzdžiui, jei anoniminis prisijungimas išjungtas susitikimo parametruose, anoniminiai vartotojai negali prisijungti prie žiniatinklio seminarų.

Norėdami sužinoti daugiau apie žiniatinklio seminarų registravimosi konfigūravimą, žr. Internetinių seminarų kas gali [registruotis konfigūravimas.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Daugiau informacijos apie "Microsoft" sąrašų parametrus žr. ["Microsoft" sąrašų parametrų valdymas](/sharepoint/control-lists).