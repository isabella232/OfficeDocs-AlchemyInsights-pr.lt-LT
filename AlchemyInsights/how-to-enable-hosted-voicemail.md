---
title: Kaip įgalinti nuomojamų išteklių balso paštą
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677996"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="8580f-102">Kaip įgalinti nuomojamų išteklių balso paštą</span><span class="sxs-lookup"><span data-stu-id="8580f-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="8580f-103">Norėdami įjungti balso paštą, **Hostedbalso paštas** turi būti nustatytas į $True.</span><span class="sxs-lookup"><span data-stu-id="8580f-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="8580f-104">Ypatybės **Hostedbalso paštas** , esanti vartotojui naudojant nuotolinį "PowerShell" (RPS).</span><span class="sxs-lookup"><span data-stu-id="8580f-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="8580f-105">Daugiau informacijos apie prisijungimą prie RPS rasite straipsnyje ["Microsoft teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , kur rasite daugiau informacijos apie prisijungimą prie RPS.</span><span class="sxs-lookup"><span data-stu-id="8580f-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="8580f-106">Komandos administratorius turi būti prisijungęs prie "Remote PowerShell" komandoms.</span><span class="sxs-lookup"><span data-stu-id="8580f-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="8580f-107">"PowerShell" paraginti komandų administratorius gali paleisti " **Set-CsUser" User@contoso.com-Hostedbalso pašto $True** , kur yra atitinkamo vartotojo SIP URI.</span><span class="sxs-lookup"><span data-stu-id="8580f-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="8580f-108">Strategijų keitimas gali užtrukti iki 24 valandų.</span><span class="sxs-lookup"><span data-stu-id="8580f-108">Changes to policies can take up to 24 hours to replicate.</span></span>