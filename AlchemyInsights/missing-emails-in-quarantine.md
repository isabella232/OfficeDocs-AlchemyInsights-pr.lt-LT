---
title: Nėra el. laiškų karantine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569234"
---
# <a name="missing-emails-in-quarantine"></a>Trūksta el. laiškų karantine"

Administratoriai gali [peržiūrėti, paleisti arba naikinti šiuos pranešimus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Norėdami atidaryti saugos & atitikties centrą, eikite į [https://protection.office.com](https://protection.office.com/) . Norėdami tiesiogiai atidaryti puslapį Karantinas, eikite į [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Galite ieškoti pagal šias reikšmes:  

- **Pranešimo ID**: visame pasaulyje unikalus pranešimo identifikatorius. Jei sąraše pasirinksite pranešimą, pasirodžiusioje **išsamios informacijos iškeliamajoje** srityje bus rodoma **pranešimo ID** reikšmė. Administratoriai gali naudoti [pranešimų sekimą,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kad rastų pranešimus ir atitinkamas pranešimo ID reikšmes.
- **Siuntėjo el. pašto adresas**: Vieno siuntėjo el. pašto adresas.
- **Gavėjo el. pašto adresas**: Vieno gavėjo el. pašto adresas.
- **Tema**: Naudokite visą pranešimo temą. Ieškaneskiriamos didžiąsias ir mažąsias raides.

Įvedę ieškos kriterijus, spustelėkite ![ Atnaujinti mygtuką ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atnaujinti,** kad filtruotumėte rezultatus.  

Cmdlet, kurias naudojate peržiūrėti ir tvarkyti pranešimus ir failus karantine yra:
- [Naikinti sulaikymo pranešimą](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksportuoti-quarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Gauti KarantinePranešimą](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Atkreipkite dėmesį, kad ši cmdlet skirta tik pranešimams, o ne kenkėjiškų programų failams iš ATP, skirtam "SharePoint Online", "OneDrive" verslui arba "Teams".
- [Išleidimo-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)