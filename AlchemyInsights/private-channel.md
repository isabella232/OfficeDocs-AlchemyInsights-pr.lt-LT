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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="1a615-102">Privatūs kanalai programoje "Microsoft Teams"</span><span class="sxs-lookup"><span data-stu-id="1a615-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="1a615-103">Privatūs kanalai yra nauja "Microsoft Teams" funkcija.</span><span class="sxs-lookup"><span data-stu-id="1a615-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="1a615-104">Atminkite, kad privačių kanalų negalima konvertuoti iš standartinių kanalų arba atvirkščiai.</span><span class="sxs-lookup"><span data-stu-id="1a615-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="1a615-105">Daugiau informacijos apie privačius kanalus, pvz., informaciją apie [privačių kanalų kūrimą ir narystę](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) bei [privatų kanalą "SharePoint" svetainėse,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)rasite [Privatūs kanalai programoje "Microsoft Teams".](https://docs.microsoft.com/MicrosoftTeams/private-channels)</span><span class="sxs-lookup"><span data-stu-id="1a615-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="1a615-106">**Pastaba:** Kadangi privačių kanalų pranešimų saugojimo konfigūracija dar nepalaikoma, nuomininkams, kuriuose įgalintos saugojimo strategijos, pagal numatytuosius nustatymus nebus įgalinti privatūs kanalai.</span><span class="sxs-lookup"><span data-stu-id="1a615-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="1a615-107">Privatūs kanalai gali būti įgalinti "Teams" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="1a615-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="1a615-108">Be to, atminkite, kad nors privačių kanalų pranešimų saugojimas nepalaikomas, palaikomas privačių kanalų bendrinamų failų saugojimas.</span><span class="sxs-lookup"><span data-stu-id="1a615-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="1a615-109">**Reikia naujo komandos savininko?**</span><span class="sxs-lookup"><span data-stu-id="1a615-109">**Need a new team owner?**</span></span>

<span data-ttu-id="1a615-110">Jei išeisite iš privataus kanalo savininko, galite pridėti naują komandos savininką naudodami "Teams PowerShell".</span><span class="sxs-lookup"><span data-stu-id="1a615-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="1a615-111">Eikite [čia](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) norėdami įdiegti "Teams PowerShell".</span><span class="sxs-lookup"><span data-stu-id="1a615-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="1a615-112">Čia yra cmdlet jums reikės:</span><span class="sxs-lookup"><span data-stu-id="1a615-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="1a615-113">Daugiau informacijos apie "Teams PowerShell" rasite ["Teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="1a615-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
