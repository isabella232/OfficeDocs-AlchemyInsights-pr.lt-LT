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
# <a name="manage-webinar-registration"></a><span data-ttu-id="99cda-102">Internetinio seminaro registracijos valdymas</span><span class="sxs-lookup"><span data-stu-id="99cda-102">Manage webinar registration</span></span>

<span data-ttu-id="99cda-103">Galite valdyti, kas gali registruotis Teams žiniatinklio seminaruose naudodami "Teams PowerShell" komandas.</span><span class="sxs-lookup"><span data-stu-id="99cda-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="99cda-104">Norėdami įdiegti "Teams PowerShell", [žr. Teams "PowerShell".](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="99cda-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="99cda-105">Pagal numatytuosius *nustatymus "WhoCanRegister"* yra įgalintas ir nustatytas **kaip EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="99cda-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="99cda-106">Norėdami leisti visiems, įskaitant anoniminius vartotojus, registruotis, turite nustatyti susitikimo strategiją visiems **naudodami** "PowerShell" komandą:</span><span class="sxs-lookup"><span data-stu-id="99cda-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="99cda-107">**Pastaba:** jei anoniminis prisijungimas išjungtas susitikimo parametruose, anoniminiai vartotojai negali prisijungti prie žiniatinklio seminarų.</span><span class="sxs-lookup"><span data-stu-id="99cda-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="99cda-108">Norėdami sužinoti daugiau ir įgalinti šį parametrą, [žr. Susitikimo parametrų valdymas Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="99cda-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="99cda-109">Jei norite išjungti susitikimo registraciją, *nustatykite AllowMeetingRegistration kaip* **False**.</span><span class="sxs-lookup"><span data-stu-id="99cda-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="99cda-110">Norėdami sužinoti daugiau apie žiniatinklio seminarų registravimosi konfigūravimą, žr. Internetinių seminarų kas gali [registruotis konfigūravimas.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="99cda-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="99cda-111">Daugiau informacijos apie "Microsoft" sąrašų parametrus žr. ["Microsoft" sąrašų parametrų valdymas](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="99cda-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
