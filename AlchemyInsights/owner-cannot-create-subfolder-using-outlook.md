---
title: Savininkas negali kurti antrinio aplanko naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665726"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="25df6-102">Savininkas negali kurti antrinio aplanko naudodamas "Outlook"</span><span class="sxs-lookup"><span data-stu-id="25df6-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="25df6-103">**Yra vykstanti problema su viešojo aplanko savininkais kuriant poaplankius naudojant "Outlook". Problema bus išspręsta netrukus.**</span><span class="sxs-lookup"><span data-stu-id="25df6-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="25df6-104">Tuo tarpu naudokite vieną iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="25df6-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="25df6-105">Naudokite "Outlook", skirtą "MAC", Norėdami sukurti poaplankį, nes problemos poveikis tik "Outlook", skirtoje staliniams kompiuteriams</span><span class="sxs-lookup"><span data-stu-id="25df6-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="25df6-106">Ar administratorius sukuria poaplankį naudodamas "EXO Shell" arba EAC</span><span class="sxs-lookup"><span data-stu-id="25df6-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="25df6-107">Pakeiskite DefaultPublicFolderMailbox/EffectivePublicFolderMailbox vartotojui į kitą pašto dėžutę, nei dėl problemų sukėlusio aplanko turinio pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="25df6-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="25df6-108">*Set-Mailbox 1 vartotojas DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="25df6-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="25df6-109">Palaukite valandą, iš naujo paleiskite "Outlook Client"</span><span class="sxs-lookup"><span data-stu-id="25df6-109">Wait for an hour, restart outlook client</span></span>