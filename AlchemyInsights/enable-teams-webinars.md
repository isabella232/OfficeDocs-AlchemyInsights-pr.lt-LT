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
# <a name="enable-teams-webinars"></a><span data-ttu-id="96f3a-102">Žiniatinklio Teams įgalinkite</span><span class="sxs-lookup"><span data-stu-id="96f3a-102">Enable Teams Webinars</span></span>

<span data-ttu-id="96f3a-103">Žiniatinklio seminarai įgalinami pagal numatytuosius parametrus.</span><span class="sxs-lookup"><span data-stu-id="96f3a-103">Webinars are enabled by default.</span></span> <span data-ttu-id="96f3a-104">Galite valdyti, kas gali planuoti ir registruotis žiniatinklio Teams naudodami "Teams PowerShell" komandas.</span><span class="sxs-lookup"><span data-stu-id="96f3a-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="96f3a-105">Visi vartotojai, kurie gali kurti susitikimą, taip pat gali sukurti internetinio seminaro susitikimą.</span><span class="sxs-lookup"><span data-stu-id="96f3a-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="96f3a-106">Jei norite valdyti, kas gali planuoti žiniatinklio Teams, naudokite *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="96f3a-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="96f3a-107">Pagal numatytuosius *nustatymus "WhoCanRegister"* yra įgalintas ir nustatytas **kaip Visi**.</span><span class="sxs-lookup"><span data-stu-id="96f3a-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="96f3a-108">Jei norite išjungti susitikimo registraciją, *nustatykite AllowMeetingRegistration kaip* **False**.</span><span class="sxs-lookup"><span data-stu-id="96f3a-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="96f3a-109">Norėdami pakeisti šiuos parametrus, turite įdiegti ["Teams PowerShell".](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="96f3a-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="96f3a-110">Be to, susitikimo strategijos yra vykdomos Teams žiniatinklio seminaruose.</span><span class="sxs-lookup"><span data-stu-id="96f3a-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="96f3a-111">Pavyzdžiui, jei anoniminis prisijungimas išjungtas susitikimo parametruose, anoniminiai vartotojai negali prisijungti prie žiniatinklio seminarų.</span><span class="sxs-lookup"><span data-stu-id="96f3a-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="96f3a-112">Norėdami sužinoti daugiau apie žiniatinklio seminarų registravimosi konfigūravimą, žr. Internetinių seminarų kas gali [registruotis konfigūravimas.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="96f3a-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="96f3a-113">Daugiau informacijos apie "Microsoft" sąrašų parametrus žr. ["Microsoft" sąrašų parametrų valdymas](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="96f3a-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>