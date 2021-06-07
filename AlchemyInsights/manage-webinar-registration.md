---
title: Internetinio seminaro registracijos valdymas
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793914"
---
# <a name="manage-webinar-registration"></a>Internetinio seminaro registracijos valdymas

Galite valdyti, kas gali registruotis Teams žiniatinklio seminaruose naudodami "Teams PowerShell" komandas. Norėdami įdiegti "Teams PowerShell", [žr. Teams "PowerShell".](/microsoftteams/teams-powershell-install) 

Pagal numatytuosius *nustatymus "WhoCanRegister"* yra įgalintas ir nustatytas **kaip EveryoneInCompany**. Norėdami leisti visiems, įskaitant anoniminius vartotojus, registruotis, turite nustatyti susitikimo strategiją visiems **naudodami** "PowerShell" komandą:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Pastaba:** jei anoniminis prisijungimas išjungtas susitikimo parametruose, anoniminiai vartotojai negali prisijungti prie žiniatinklio seminarų. Norėdami sužinoti daugiau ir įgalinti šį parametrą, [žr. Susitikimo parametrų valdymas Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Jei norite išjungti susitikimo registraciją, *nustatykite AllowMeetingRegistration kaip* **False**.

Norėdami sužinoti daugiau apie žiniatinklio seminarų registravimosi konfigūravimą, žr. Internetinių seminarų kas gali [registruotis konfigūravimas.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Daugiau informacijos apie "Microsoft" sąrašų parametrus žr. ["Microsoft" sąrašų parametrų valdymas](/sharepoint/control-lists).
