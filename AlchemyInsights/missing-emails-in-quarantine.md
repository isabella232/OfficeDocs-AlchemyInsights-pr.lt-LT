---
title: Sulaikyti trūkstami el. laiškai
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831742"
---
# <a name="missing-emails-in-quarantine"></a>Sulaikyti trūksta el. laiškų"

Administratoriai gali [peržiūrėti, išleisti arba panaikinti šiuos pranešimus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Norėdami atidaryti saugos & centrą, eikite į [https://protection.office.com](https://protection.office.com/) . Norėdami atidaryti sulaikymo puslapį tiesiogiai, eikite į [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Galite ieškoti pagal šias reikšmes:  

- **Pranešimo ID**: visuotinai unikalus pranešimo identifikatorius. Jei sąraše pasirinksite pranešimą, rodomame išskridimo  srityje Išsami informacija bus rodoma pranešimo **ID** reikšmė. Administratoriai gali naudoti [laiškų sekimą,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kad rastų laiškus ir jų atitinkamas pranešimo ID reikšmes.
- **Siuntėjo el.** pašto adresas: vieno siuntėjo el. pašto adresas.
- **Gavėjo el.** pašto adresas: vieno gavėjo el. pašto adresas.
- **Tema**: naudokite visą laiško temą. Ieškai skiriamos ne abc nuo abc.

Įvedėte ieškos kriterijus, spustelėkite mygtuką ![ Atnaujinti, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **kad filtruokite** rezultatus.  

Cmdlet, kurią naudojate laiškams ir failams sulaikyti peržiūrėti ir tvarkyti, yra:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Atkreipkite dėmesį, kad ši "cmdlet" skirta tik laiškams, o ne kenkėjiškų programų failams iš ATP, skirtos "SharePoint Online", "OneDrive" verslui arba "Teams".
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)