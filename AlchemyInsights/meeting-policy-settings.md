---
title: Susitikimų strategijos parametrai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627582"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="3f671-102">Tvarkykite susitikimų strategijas programoje "Microsoft teams"</span><span class="sxs-lookup"><span data-stu-id="3f671-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="3f671-103">Susitikimų strategijos naudojamos valdyti funkcijoms, kurios pasiekiamos jūsų organizacijos vartotojų suplanuotų susitikimų dalyviams.</span><span class="sxs-lookup"><span data-stu-id="3f671-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="3f671-104">Kai kurios susitikimų strategijos funkcijos "teams" administravimo centre gali būti neįgyvendintos (tai yra pažymėta "netrukus" dokumentacijoje).</span><span class="sxs-lookup"><span data-stu-id="3f671-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="3f671-105">Tokiu atveju arba, jei gaunate klaidos pranešimą "negalime atnaujinti strategijos dabar, bet bandykite ją dar kartą" Microsoft teams "administravimo centras, rekomenduojame naudoti" PowerShell "komandų susitikimo strategijų kūrimas arba modifikavimas.</span><span class="sxs-lookup"><span data-stu-id="3f671-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="3f671-106">Daugiau informacijos apie susitikimų strategijas rasite šiuose šaltiniuose:</span><span class="sxs-lookup"><span data-stu-id="3f671-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="3f671-107">Norėdami sužinoti, kaip kurti strategijas, atlikti keitimus ir priskirti vartotojus politikai [, žr.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="3f671-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="3f671-108">Norėdami, kad strategijos pakeitimai naudojant "PowerShell" cmdlet, ieškokite [komandos "PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="3f671-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="3f671-109">Jums reikia naudoti ["Skype" Business PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) komandų susitikimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="3f671-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="3f671-110">Peržiūrėkite [\*-csteamsmeetingpolicy cmdlet dokumentaciją](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="3f671-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="3f671-111">**Pastaba:** Tai gali užtrukti iki 24 valandų, kad politikos pakeitimai įsigaliotų vartotojams.</span><span class="sxs-lookup"><span data-stu-id="3f671-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="3f671-112">Gali nepavykti iš karto keisti naujai sukurtų strategijų; Palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą politiką.</span><span class="sxs-lookup"><span data-stu-id="3f671-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="3f671-113">Jei vis tiek kyla problemų, bandykite "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="3f671-113">If you're still having problems, try PowerShell.</span></span>  