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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892055"
---
# <a name="missing-emails-in-quarantine"></a>Sulaikyti trūkstami el. laiškai

Administratoriai gali [peržiūrėti, išleisti arba panaikinti šiuos pranešimus](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

""Microsoft 365" sargyba portale <https://security.microsoft.com> eikite į **Sulaikyti** \> **peržiūra**. Arba, norėdami pereiti tiesiai į sulaikymo **puslapį,** naudokite <https://security.microsoft.com/quarantine> .  

Daugiau informacijos apie ieškos / filtro reikšmes, kurias galite naudoti, žr. Sulaikytų laiškų ir failų valdymas [kaip administratorius EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

"cmdlet", kurias naudojate laiškams ir failams sulaikyti peržiūrėti ir tvarkyti, yra:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Atkreipkite dėmesį, kad ši "cmdlet" skirta tik laiškams, o ne Seifas "SharePoint", ""OneDrive"" arba "Microsoft Teams".
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
