---
title: "\"Teams\" leidžia arba išjungia IP vaizdo įrašą"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826351"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="1e58e-102">"Teams" leidžia arba išjungia IP vaizdo įrašą</span><span class="sxs-lookup"><span data-stu-id="1e58e-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="1e58e-103">**Susitikimo strategijos keitimas arba kūrimas**</span><span class="sxs-lookup"><span data-stu-id="1e58e-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="1e58e-104">Norėdami pakeisti arba sukurti susitikimo strategiją, eikite į **"Microsoft Teams" administravimo centrą > Susitikimai > susitikimų strategijas.**</span><span class="sxs-lookup"><span data-stu-id="1e58e-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="1e58e-105">Sąraše pasirinkite strategiją arba spustelėkite **Įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="1e58e-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="1e58e-106">Jei kuriate naują strategiją, įtraukite pavadinimą ir aprašą.</span><span class="sxs-lookup"><span data-stu-id="1e58e-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="1e58e-107">Pavadinime negali būti specialiųjų simbolių arba daugiau nei 64 simbolių.</span><span class="sxs-lookup"><span data-stu-id="1e58e-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="1e58e-108">Pasirinkite parametrus ir spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="1e58e-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="1e58e-109">Pvz., tarkime, kad turite daug vartotojų ir norite apriboti pralaidumą, kurio jiems reikės susitikimui.</span><span class="sxs-lookup"><span data-stu-id="1e58e-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="1e58e-110">Sukurtumėte naują pasirinktinę strategiją, pavadintą „Apribotas pralaidumas“ ir išjungtumėte šiuos parametrus:</span><span class="sxs-lookup"><span data-stu-id="1e58e-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="1e58e-111">Dalyje **Garsas ir vaizdas**:</span><span class="sxs-lookup"><span data-stu-id="1e58e-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="1e58e-112">Išjungti funkciją Leisti įrašymą debesyje.</span><span class="sxs-lookup"><span data-stu-id="1e58e-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="1e58e-113">Išjungti funkciją Leisti IP vaizdo įrašą.</span><span class="sxs-lookup"><span data-stu-id="1e58e-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="1e58e-114">Tuomet priskirkite strategijas vartotojams.</span><span class="sxs-lookup"><span data-stu-id="1e58e-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="1e58e-115">**Susitikimo strategijos priskyrimas vartotojams**</span><span class="sxs-lookup"><span data-stu-id="1e58e-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="1e58e-116">„Microsoft Teams“ administravimo centro kairiojoje naršymo srityje eikite į **Vartotojai**, tada spustelėkite vartotoją.</span><span class="sxs-lookup"><span data-stu-id="1e58e-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="1e58e-117">Pasirinkite vartotoją spustelėdami vartotojo vardo kairėje, tada spustelėkite **Redaguoti parametrus**.</span><span class="sxs-lookup"><span data-stu-id="1e58e-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="1e58e-118">Dalyje **Susitikimo** strategija pasirinkite strategiją, kurią norite priskirti, tada spustelėkite **Taikyti**.</span><span class="sxs-lookup"><span data-stu-id="1e58e-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="1e58e-119">Daugiau informacijos žr. ["Teams" susitikimų strategijų valdymas.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="1e58e-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
