---
title: Viršyta dienos el. paštas riba. Darbo eigos sustabdomas.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059646"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="315a9-103">Kasdien elektroniniu paÅ¡tu viršyta riba.</span><span class="sxs-lookup"><span data-stu-id="315a9-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="315a9-104">Darbo eigos sustabdomas.</span><span class="sxs-lookup"><span data-stu-id="315a9-104">Workflow is suspended.</span></span>

<span data-ttu-id="315a9-105">Ši klaida gali būti siunčiami šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="315a9-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="315a9-106">Jūs turite darbo eigos SharePoint Online, kuri naudoja SharePoint 2010 arba SharePoint 2013 darbo eigos platformos tipo.</span><span class="sxs-lookup"><span data-stu-id="315a9-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="315a9-107">Darbo eiga yra sukonfigūruotas siųsti el. pašto žinutę daugiau kaip 200 vartotojų vienu metu, daugiau nei 10 000 gavėjų per dieną ar daugiau nei 30 lai kai per minutę.</span><span class="sxs-lookup"><span data-stu-id="315a9-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="315a9-108">Kai paleidžiate darbo eigą, el. laiškas nesiunčiamas ir galite pastebėti toliau pateiktas parinktis:</span><span class="sxs-lookup"><span data-stu-id="315a9-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="315a9-109">Darbo eigos SharePoint 2013 platformos tipą, Jūs eikite į puslapį **Darbo eigos būsena** .</span><span class="sxs-lookup"><span data-stu-id="315a9-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="315a9-110">Darbo eigos būsenos puslapyje, **Vidaus būklė** yra nustatyta **pradėjo**ir informacijos rodo **negalima siųsti gavėjui**.</span><span class="sxs-lookup"><span data-stu-id="315a9-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="315a9-111">Norėdami išspręsti šią problemą, sukonfigūruokite savo darbo eigą, kad siųsti el. laiškus be [Exchange Online siuntėjas ribas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="315a9-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="315a9-112">Pvz., naudoti darbo eigą sustojimas, siųsti el. laišką į "Office 365" grupė, paskirstymo grupę ar paštas įgalintas saugos grupę arba siųsti žinutę mažiau nei 200 gavėjams vienu metu.</span><span class="sxs-lookup"><span data-stu-id="315a9-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="315a9-113">Daugiau informacijos rasite šiame [straipsnyje](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="315a9-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="315a9-114">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="315a9-114">Related topics</span></span>
- [<span data-ttu-id="315a9-115">Sukurti srauto</span><span class="sxs-lookup"><span data-stu-id="315a9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="315a9-116">SharePoint ir srauto</span><span class="sxs-lookup"><span data-stu-id="315a9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 