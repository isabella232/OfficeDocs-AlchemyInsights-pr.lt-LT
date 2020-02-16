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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042852"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="14b94-102">Tvarkykite susitikimų strategijas programoje "Microsoft teams"</span><span class="sxs-lookup"><span data-stu-id="14b94-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="14b94-103">**Pastaba: politikos pakeitimai, kurie įsigalios vartotojams, gali užtrukti iki 24 valandų.**</span><span class="sxs-lookup"><span data-stu-id="14b94-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="14b94-104">Gali nepavykti iš karto keisti naujai sukurtų strategijų; Palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą politiką.</span><span class="sxs-lookup"><span data-stu-id="14b94-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="14b94-105">Susitikimų strategijos naudojamos valdyti funkcijoms, kurios pasiekiamos jūsų organizacijos vartotojų suplanuotų susitikimų dalyviams.</span><span class="sxs-lookup"><span data-stu-id="14b94-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="14b94-106">Kai kurios susitikimų strategijos funkcijos "teams" administravimo centre gali būti neįgyvendintos (tai yra pažymėta "netrukus" dokumentacijoje).</span><span class="sxs-lookup"><span data-stu-id="14b94-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="14b94-107">Tokiu atveju arba, jei gaunate klaidos pranešimą "negalime atnaujinti strategijos dabar, bet bandykite ją dar kartą" Microsoft teams "administravimo centras, rekomenduojame naudoti" PowerShell "komandų susitikimo strategijų kūrimas arba modifikavimas.</span><span class="sxs-lookup"><span data-stu-id="14b94-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="14b94-108">Daugiau informacijos apie susitikimų strategijas rasite šiuose šaltiniuose:</span><span class="sxs-lookup"><span data-stu-id="14b94-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="14b94-109">Norėdami sužinoti, kaip kurti strategijas, atlikti keitimus ir priskirti vartotojus politikai [, žr.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="14b94-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="14b94-110">Norėdami, kad strategijos pakeitimai naudojant "PowerShell" cmdlet, ieškokite [komandos "PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="14b94-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="14b94-111">Jums reikia naudoti ["Skype" Business PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) komandų susitikimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="14b94-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="14b94-112">Peržiūrėkite [\*-csteamsmeetingpolicy cmdlet dokumentaciją](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="14b94-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

