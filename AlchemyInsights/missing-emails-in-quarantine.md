---
title: Trūksta laiškų karantinui
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673722"
---
# <a name="missing-emails-in-quarantine"></a>Trūksta laiškų karantinui "

Administratoriai gali [Peržiūrėti, išleisti arba panaikinti šiuos el. pašto pranešimams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Norėdami atidaryti saugos & atitikties centrą, eikite į [https://protection.office.com](https://protection.office.com/) . Norėdami atidaryti puslapį Karantinas tiesiogiai, eikite į [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Galite ieškoti pagal šias reikšmes:  

- **Pranešimo ID**: visuotinis Unikalusis pranešimo identifikatorius. Jei sąraše pasirenkate pranešimą, pasirodo  **pranešimo ID**  reikšmė, esanti srityje  **išsami**  iškeliamojo pranešimo sritis. Administratoriai gali naudoti [pranešimų](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) sekimą, kad rastų laiškus ir jų atitinkamas pranešimo ID reikšmes.
- **Siuntėjo elektroninio pašto adresas**: vieno siuntėjo elektroninio pašto adresas.
- **Gavėjo elektroninio pašto adresas**: vieno gavėjo elektroninio pašto adresas.
- **Tema**: naudokite visą pranešimo temą. Ieška Didžiosios ir mažosios raidės neskiriamas.

Įvedę ieškos kriterijus spustelėkite ![ mygtuką atnaujinti, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** kad filtruotumėte rezultatus.  

"Cmdlet", kurias peržiūrite ir tvarkote ir tvarkote karantine laikomus failus, yra:
- [Naikinti – Karantinemessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksportas – Karantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Gauti – Karantinemessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Peržiūra – Karantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Pastaba, kad šis cmdlet skirtas tik pranešimams, o ne kenkėjiškų programų FAILAMS iš ATP, skirtos "SharePoint Online", "OneDrive" verslui arba komandoms.
- [Leidimas – Karantinemessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)