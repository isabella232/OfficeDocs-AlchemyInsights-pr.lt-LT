---
title: Susitikimo strategijos parametrai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704614"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="5b02c-102">"Microsoft teams" susitikimų strategijų valdymas</span><span class="sxs-lookup"><span data-stu-id="5b02c-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="5b02c-103">**Pastaba: gali užtrukti iki 24 valandų, kol strategijos pokyčiai įsigalios vartotojams.**</span><span class="sxs-lookup"><span data-stu-id="5b02c-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="5b02c-104">Jums gali nepavykti iš karto pakeisti naujai sukurtų strategijų. Palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą strategiją.</span><span class="sxs-lookup"><span data-stu-id="5b02c-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="5b02c-105">Susitikimo strategijos naudojamos norint valdyti funkcijas, kurios pasiekiamos susitikimo dalyviams susitikimams, kuriuos suplanavo jūsų organizacijos vartotojai.</span><span class="sxs-lookup"><span data-stu-id="5b02c-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="5b02c-106">Kai kurios susitikimo strategijų funkcijos gali būti neįgyvendintos "teams" administravimo centre, tačiau jie yra pažymėti "jau greitai" dokumentacijoje.</span><span class="sxs-lookup"><span data-stu-id="5b02c-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="5b02c-107">Šiuo atveju arba jei gaunate klaidos pranešimą, pvz., "negalime atnaujinti strategijos dabar, bet pabandykite dar kartą vėliau" "Microsoft teams" administravimo centre rekomenduojame naudoti "PowerShell", kad sukurtumėte arba modifikuotumėte "teams" susitikimo strategijas.</span><span class="sxs-lookup"><span data-stu-id="5b02c-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="5b02c-108">Daugiau informacijos apie susitikimų strategijas rasite šiuose šaltiniuose:</span><span class="sxs-lookup"><span data-stu-id="5b02c-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="5b02c-109">Norėdami sužinoti apie strategijų kūrimą, keitimą ir vartotojų priskyrimą strategijai, peržiūrėkite [susitikimo strategijų valdymas "teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)".</span><span class="sxs-lookup"><span data-stu-id="5b02c-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="5b02c-110">Norėdami atlikti strategijos keitimą naudodami "PowerShell" "cmdlet", peržiūrėkite "teams" " [PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="5b02c-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="5b02c-111">Jums reikia naudoti ["Skype" verslui "PowerShell" modulį](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) komandoms susitikimo strategijoms.</span><span class="sxs-lookup"><span data-stu-id="5b02c-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="5b02c-112">Norėdami gauti daugiau informacijos, peržiūrėkite [\*-csteamaimeetingpolicy "cmdlet" dokumentus](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="5b02c-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

