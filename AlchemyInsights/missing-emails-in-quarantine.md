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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539832"
---
# <a name="missing-emails-in-quarantine"></a>Sulaikyti trūksta el. laiškų"

Administratoriai gali [peržiūrėti, išleisti arba panaikinti šiuos pranešimus.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Norėdami atidaryti saugos & centrą, eikite į [https://protection.office.com](https://protection.office.com/) . Norėdami atidaryti sulaikymo puslapį tiesiogiai, eikite į [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Galite ieškoti pagal šias reikšmes:  

- **Pranešimo ID**: visuotinai unikalus pranešimo identifikatorius. Jei sąraše pasirinksite pranešimą, rodomame išskridimo  srityje Išsami informacija bus rodoma pranešimo **ID** reikšmė. Administratoriai gali naudoti [laiškų sekimą,](/microsoft-365/security/office-365-security/message-trace-scc) kad rastų laiškus ir jų atitinkamas pranešimo ID reikšmes.
- **Siuntėjo el.** pašto adresas: vieno siuntėjo el. pašto adresas.
- **Gavėjo el.** pašto adresas: vieno gavėjo el. pašto adresas.
- **Tema**: naudokite visą laiško temą. Ieškai skiriamos ne abc nuo abc.

Įvedėte ieškos kriterijus, spustelėkite mygtuką ![ Atnaujinti, ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **kad filtruokite** rezultatus.

Cmdlet, kurią naudojate laiškams ir failams sulaikyti peržiūrėti ir tvarkyti, yra:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Atkreipkite dėmesį, kad ši "cmdlet" skirta tik laiškams, o ne kenkėjiškų programų failams iš "Microsoft" sargybos, skirtai "Office 365", skirtai "SharePoint Online", ""OneDrive" verslui" arba "Teams".
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)