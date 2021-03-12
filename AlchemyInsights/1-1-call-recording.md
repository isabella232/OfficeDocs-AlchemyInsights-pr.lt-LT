---
title: 1:1 skambučių įrašymas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733857"
---
# <a name="11-call-recording"></a><span data-ttu-id="bc57e-102">1:1 skambučių įrašymas</span><span class="sxs-lookup"><span data-stu-id="bc57e-102">1:1 call recording</span></span>

<span data-ttu-id="bc57e-103">Administratoriai turi imtis veiksmų dabar, kad vartotojai galėtų įrašyti "1:1" iškvietimus.</span><span class="sxs-lookup"><span data-stu-id="bc57e-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="bc57e-104">Pradėję balandžio 12 d., 2021, pradėsime vykdyti naują komandų skambinimo strategijos parinktį *Allowcloudrecordingforcalls*.</span><span class="sxs-lookup"><span data-stu-id="bc57e-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="bc57e-105">Šiuo metu "1:1" skambučių įrašymo galimybes kontroliuoja "teams" susitikimo strategijų parinktis *Allowcloudrecording* .</span><span class="sxs-lookup"><span data-stu-id="bc57e-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="bc57e-106">Jei vartotojams leidžiama įrašyti komandų susitikimus, jie taip pat gali įrašyti "1:1" skambutį.</span><span class="sxs-lookup"><span data-stu-id="bc57e-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="bc57e-107">Jei norite blokuoti visus vartotojus, kad įrašytumėte "1:1" iškvietimus, jums nereikia imtis jokių veiksmų.</span><span class="sxs-lookup"><span data-stu-id="bc57e-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="bc57e-108">Numatytoji parinktis *Allowcloudrecordingforcalls* skambinimo strategija bus $FALSE.</span><span class="sxs-lookup"><span data-stu-id="bc57e-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="bc57e-109">Šis pakeitimas dokumentuojamas šiame pranešimų centro pranešime: [(atnaujinta) "1:1" skambučių įrašymo strategijos Įvadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Norėdami nustatyti "teams" skambinimo strategijos parinktį, turite naudoti " [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)".</span><span class="sxs-lookup"><span data-stu-id="bc57e-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="bc57e-110">**Skambučio įrašymo įgalinimas "1:1" pokalbiuose:** Set-CsTeamsCallingPolicy – tapatybė visuotinis – AllowCloudRecordingForCalls $TRUE</span><span class="sxs-lookup"><span data-stu-id="bc57e-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="bc57e-111">**Norėdami išjungti skambučio įrašymą "1:1" pokalbiuose:** Set-CsTeamsCallingPolicy – tapatybė visuotinis – AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="bc57e-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

