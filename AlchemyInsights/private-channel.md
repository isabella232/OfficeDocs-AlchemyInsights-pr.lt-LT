---
title: Privatus kanalas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005446"
---
# <a name="private-channels-in-microsoft-teams"></a>Privatūs kanalai programoje "Microsoft Teams"

Privatūs kanalai yra nauja "Microsoft Teams" funkcija. Atminkite, kad privačių kanalų negalima konvertuoti iš standartinių kanalų arba atvirkščiai.

Daugiau informacijos apie privačius kanalus, pvz., informaciją apie [privačių kanalų kūrimą ir narystę](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) bei [privatų kanalą "SharePoint" svetainėse,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)rasite [Privatūs kanalai programoje "Microsoft Teams".](https://docs.microsoft.com/MicrosoftTeams/private-channels) 

**Pastaba:** Kadangi privačių kanalų pranešimų saugojimo konfigūracija dar nepalaikoma, nuomininkams, kuriuose įgalintos saugojimo strategijos, pagal numatytuosius nustatymus nebus įgalinti privatūs kanalai. Privatūs kanalai gali būti įgalinti "Teams" administravimo centre. Be to, atminkite, kad nors privačių kanalų pranešimų saugojimas nepalaikomas, palaikomas privačių kanalų bendrinamų failų saugojimas.

**Reikia naujo komandos savininko?**

Jei išeisite iš privataus kanalo savininko, galite pridėti naują komandos savininką naudodami "Teams PowerShell".


- Eikite [čia](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) norėdami įdiegti "Teams PowerShell".

Čia yra cmdlet jums reikės:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Daugiau informacijos apie "Teams PowerShell" rasite ["Teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
