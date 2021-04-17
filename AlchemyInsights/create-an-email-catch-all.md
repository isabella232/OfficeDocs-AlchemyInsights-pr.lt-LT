---
title: El. laiško užgaudo kūrimas
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816208"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="ca2b7-102">El. laiško užgaudo kūrimas</span><span class="sxs-lookup"><span data-stu-id="ca2b7-102">Create an email catch all</span></span>

<span data-ttu-id="ca2b7-103">Laimikio naudojimas yra labai neskatinantis.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="ca2b7-104">Geriau pateikti siuntėjui atšokti, kad siuntėjai žinotų, jog jų laiško nepavyko pristatyti kaip adreso, kad jie galėtų imtis veiksmų.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="ca2b7-105">Taip pat galite apriboti stebimos pašto dėžutės gaudo tik anksčiau galiojančius el. pašto adresus.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="ca2b7-106">Visos pašto dėžutės gaus daug pašto šiukšlių ir galiausiai gali užpildyti, jei nebus atidžiai stebimos.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="ca2b7-107">(Yra gavimo apribojimų.)</span><span class="sxs-lookup"><span data-stu-id="ca2b7-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="ca2b7-108">Jei nuspręsite tęsti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="ca2b7-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="ca2b7-109">Dinaminio paskirstymo grupės kūrimas & "Visi gavėjų tipai".</span><span class="sxs-lookup"><span data-stu-id="ca2b7-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="ca2b7-110">Sukurkite specialią pašto dėžutę, kad gaudysite el. laiškus, pvz., catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="ca2b7-111">Konkretaus domeno domeno tipą nustatykite kaip "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="ca2b7-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="ca2b7-112">Jei vėliau pašalinsite viską, įsitikinkite, kad domenas vėl bus patikimas.</span><span class="sxs-lookup"><span data-stu-id="ca2b7-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="ca2b7-113">Sukurkite "Mailflow" transportavimo taisyklę taip:</span><span class="sxs-lookup"><span data-stu-id="ca2b7-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="ca2b7-114">Jei siuntėjas yra "Už organizacijos ribų"</span><span class="sxs-lookup"><span data-stu-id="ca2b7-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="ca2b7-115">Peradresuoti laišką į Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="ca2b7-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="ca2b7-116">Išskyrus atvejus, kai gavėjas yra allusers@domain.com narys (siuntimo grupėje yra visi nariai)</span><span class="sxs-lookup"><span data-stu-id="ca2b7-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="ca2b7-117">Įsitikinkite, kad į dinaminio paskirstymo grupę įtraukta naujų pašto dėžučių</span><span class="sxs-lookup"><span data-stu-id="ca2b7-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
