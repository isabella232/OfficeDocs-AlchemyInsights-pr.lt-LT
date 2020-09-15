---
title: El. laiško kūrimas visiems
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712994"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="42994-102">El. laiško kūrimas visiems</span><span class="sxs-lookup"><span data-stu-id="42994-102">Create an email catch all</span></span>

<span data-ttu-id="42994-103">Naudokite sugavimo visi primygtinai nenori.</span><span class="sxs-lookup"><span data-stu-id="42994-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="42994-104">Jei norite, kad būtų lengviau grįžti prie siuntėjo, pranešantiems siuntėjams žinotų, kad pranešimo negalima pristatyti, kad jie galėtų imtis veiksmų.</span><span class="sxs-lookup"><span data-stu-id="42994-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="42994-105">Taip pat galite apriboti stebimą pašto dėžutę, kad tik galėtumėte sugauti anksčiau galiojančius el. pašto adresus.</span><span class="sxs-lookup"><span data-stu-id="42994-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="42994-106">Bet koks laimikis visos pašto dėžutės gaus gerą pašto šiukšlių ir galiausiai gali būti užpildytas, jei nėra atidžiai stebimas.</span><span class="sxs-lookup"><span data-stu-id="42994-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="42994-107">(Yra gaunamų apribojimų.)</span><span class="sxs-lookup"><span data-stu-id="42994-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="42994-108">Jei nuspręsite tęsti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="42994-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="42994-109">Dinaminio paskirstymo grupės kūrimas & įtraukti "visi gavėjų tipai".</span><span class="sxs-lookup"><span data-stu-id="42994-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="42994-110">Sukurkite specialią pašto dėžutę, kad galėtumėte sugauti laiškus, pvz., catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="42994-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="42994-111">Konkrečiam domenui nustatykite DomainType "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="42994-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="42994-112">Jei po to norite pašalinti viską, įsitikinkite, kad domeną norite grąžinti į patikimą.</span><span class="sxs-lookup"><span data-stu-id="42994-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="42994-113">Sukurkite pašto srauto transportavimo taisyklę taip:</span><span class="sxs-lookup"><span data-stu-id="42994-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="42994-114">Jei siuntėjas yra "už organizacijos ribų"</span><span class="sxs-lookup"><span data-stu-id="42994-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="42994-115">Peradresuokite pranešimą į "Catchall@domain.com"</span><span class="sxs-lookup"><span data-stu-id="42994-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="42994-116">Išskyrus atvejus, kai gavėjas yra "allusers@domain.com" narys (paskirstymo grupėje yra visi nariai)</span><span class="sxs-lookup"><span data-stu-id="42994-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="42994-117">Įsitikinkite, kad patvirtintumėte, jog naujos pašto dėžutės įtraukiamos į dinaminio paskirstymo grupę</span><span class="sxs-lookup"><span data-stu-id="42994-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
