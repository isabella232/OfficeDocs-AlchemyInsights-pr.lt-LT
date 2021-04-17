---
title: Susitikimo strategijos parametrai
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825451"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="c595d-102">"Microsoft Teams" susitikimų strategijų valdymas</span><span class="sxs-lookup"><span data-stu-id="c595d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="c595d-103">**Pastaba: gali užtrukti iki 24 valandų, kad strategijos pakeitimai įsigalios vartotojams.**</span><span class="sxs-lookup"><span data-stu-id="c595d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="c595d-104">Jums gali nepavykti iš karto atlikti naujai sukurtų strategijų pakeitimų; palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą strategiją.</span><span class="sxs-lookup"><span data-stu-id="c595d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="c595d-105">Susitikimų strategijos naudojamos valdyti funkcijas, kurios susitikimo dalyviams prieinamos susitikimams, kuriuos suplanuoja jūsų organizacijos vartotojai.</span><span class="sxs-lookup"><span data-stu-id="c595d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="c595d-106">Kai kurios susitikimų strategijų funkcijos dar gali būti neį įgyvendinamos "Teams" administravimo centre (dokumentuose jos žymimos "netrukus").</span><span class="sxs-lookup"><span data-stu-id="c595d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="c595d-107">Šiuo atveju arba jei gaunate klaidos pranešimą, pvz., "Šiuo metu negalime atnaujinti strategijos, bet bandykite ją dar kartą vėliau" "Microsoft Teams" administravimo centre, rekomenduojame naudoti "PowerShell" "Teams" susitikimų strategijai kurti arba modifikuoti.</span><span class="sxs-lookup"><span data-stu-id="c595d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="c595d-108">Daugiau informacijos apie susitikimų strategijas žr. šie ištekliai:</span><span class="sxs-lookup"><span data-stu-id="c595d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="c595d-109">Norėdami sužinoti apie strategijų kūrimas, pakeitimų keitimų ir vartotojų priskyrimą strategijai, žr. [Susitikimų strategijų valdymas "Teams".](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="c595d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="c595d-110">Norėdami keisti strategiją naudodami "PowerShell" "cmdlet", žr. ["Teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="c595d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="c595d-111">Turite naudoti ["Skype" verslui "PowerShell" modulį, skirtą "Teams"](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) susitikimo strategijai.</span><span class="sxs-lookup"><span data-stu-id="c595d-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="c595d-112">Daugiau informacijos [žr. \*-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentacijoje.</span><span class="sxs-lookup"><span data-stu-id="c595d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

