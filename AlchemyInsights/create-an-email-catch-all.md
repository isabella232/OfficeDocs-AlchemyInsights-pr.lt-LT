---
title: Sukurkite el. Laiško sugavimo viską
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286200"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="bdc4f-102">Sukurkite el. Laiško sugavimo viską</span><span class="sxs-lookup"><span data-stu-id="bdc4f-102">Create an email catch all</span></span>

<span data-ttu-id="bdc4f-103">Laimikio naudojimas yra labai varžomas.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="bdc4f-104">Geriau pateikti atmetimą siuntėjui, kad siuntėjai žinotų, jog jų pranešimas negali būti pristatytas taip, kaip sprendžiama, kad jie galėtų imtis veiksmų.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="bdc4f-105">Taip pat galite apriboti stebimą pašto dėžutę tik sugavimo tik anksčiau galiojančius el. pašto adresus.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="bdc4f-106">Bet koks laimikis visos pašto dėžutės gaus nemažai šlamštas ir galiausiai gali užpildyti, jei nėra atidžiai stebimi.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="bdc4f-107">(Yra gavimo ribos.)</span><span class="sxs-lookup"><span data-stu-id="bdc4f-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="bdc4f-108">Jei nuspręsite tęsti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="bdc4f-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="bdc4f-109">Dinaminio paskirstymo grupės kūrimas & apima "Visi gavėjų tipai".</span><span class="sxs-lookup"><span data-stu-id="bdc4f-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="bdc4f-110">Sukurkite specialią pašto dėžutę el. laiškams sugauti, pvz., catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="bdc4f-111">Konkretaus domeno, nustatykite DomainType į "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="bdc4f-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="bdc4f-112">Jei vėliau pašalinsite visus sugavimus, būtinai nustatykite domeną atgal į Autoritetingą.</span><span class="sxs-lookup"><span data-stu-id="bdc4f-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="bdc4f-113">Sukurkite Mailflow transportavimo taisyklę taip:</span><span class="sxs-lookup"><span data-stu-id="bdc4f-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="bdc4f-114">Jei siuntėjas yra "už organizacijos ribų"</span><span class="sxs-lookup"><span data-stu-id="bdc4f-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="bdc4f-115">Peradresuoti pranešimą į Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="bdc4f-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="bdc4f-116">Išskyrus atvejus, kai gavėjas yra allusers@domain.com narys (paskirstymo grupėje yra visi nariai)</span><span class="sxs-lookup"><span data-stu-id="bdc4f-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="bdc4f-117">Įsitikinkite, kad patikrinti, ar naujos pašto dėžutės yra įtrauktos į dinaminio paskirstymo grupės</span><span class="sxs-lookup"><span data-stu-id="bdc4f-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
