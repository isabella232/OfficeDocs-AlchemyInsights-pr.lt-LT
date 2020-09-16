---
title: Viršytas dienos el. pašto limitas. Darbo eiga sustabdoma.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731571"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="60c2a-103">Viršytas dienos el. pašto limitas.</span><span class="sxs-lookup"><span data-stu-id="60c2a-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="60c2a-104">Darbo eiga sustabdoma.</span><span class="sxs-lookup"><span data-stu-id="60c2a-104">Workflow is suspended.</span></span>

<span data-ttu-id="60c2a-105">Ši klaida gali būti gauta šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="60c2a-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="60c2a-106">Naudojate "SharePoint Online" darbo eigą, kuri naudoja "SharePoint 2010" arba "SharePoint 2013" darbo eigos platformos tipą.</span><span class="sxs-lookup"><span data-stu-id="60c2a-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="60c2a-107">Darbo eiga sukonfigūruota siųsti pasirinktiniam el. laiškui daugiau nei 200 vartotojams vienu metu, daugiau nei 10 000 gavėjams per dieną arba daugiau nei 30 pranešimų per minutę.</span><span class="sxs-lookup"><span data-stu-id="60c2a-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="60c2a-108">Paleidus darbo eigą, el. laiškas neatsiųstas, o jūs pastebėsite tokį veikimą:</span><span class="sxs-lookup"><span data-stu-id="60c2a-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="60c2a-109">Jei naudojate darbo eigą naudodami "SharePoint" 2013 platformos tipą, pereikite į **darbo eigos būsenos** puslapį.</span><span class="sxs-lookup"><span data-stu-id="60c2a-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="60c2a-110">Darbo eigos būsenos puslapyje **Vidinė būsena** nustatyta kaip **paleista**, o informacijos debesėlyje rodoma **negalima išsiųsti gavėjui**.</span><span class="sxs-lookup"><span data-stu-id="60c2a-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="60c2a-111">Norėdami išspręsti šią problemą, sukonfigūruokite darbo eigą, kad siųstumėte el. laiškus, neviršijant " [Exchange Online" siuntėjo limitų](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="60c2a-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="60c2a-112">Pvz., naudokite darbo eigą pristabdyti, siųskite el. laišką į "Microsoft" 365 grupę, platinimo grupę arba pašto įgalintos saugos grupę arba išsiųskite laišką mažiau nei "200" gavėjams vienu metu.</span><span class="sxs-lookup"><span data-stu-id="60c2a-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="60c2a-113">Daugiau informacijos ieškokite šiame [straipsnyje](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="60c2a-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="60c2a-114">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="60c2a-114">Related topics</span></span>
- [<span data-ttu-id="60c2a-115">Kurti srautą</span><span class="sxs-lookup"><span data-stu-id="60c2a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="60c2a-116">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="60c2a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 