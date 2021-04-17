---
title: Savininkas negali sukurti poaplankių naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836143"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="833f0-102">Savininkas negali sukurti poaplankių naudodamas "Outlook"</span><span class="sxs-lookup"><span data-stu-id="833f0-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="833f0-103">**Nuolat kyla problemų dėl viešųjų aplankų savininkų, kurie kuria poaplankius naudodami "Outlook". Netrukus problema bus išspręsta.**</span><span class="sxs-lookup"><span data-stu-id="833f0-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="833f0-104">Tuo tarpu naudokite vieną iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="833f0-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="833f0-105">"Outlook for MAC" naudojimas norint sukurti poaplankį, nes problema veikia tik "Outlook", skirtą staliniams langams (visos versijos)</span><span class="sxs-lookup"><span data-stu-id="833f0-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="833f0-106">Administratoriaus sukurti poaplankį naudojant EXO apvalkalą arba EAC</span><span class="sxs-lookup"><span data-stu-id="833f0-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="833f0-107">"DefaultPublicFolderMailbox" / "EffectivePublicFolderMailbox" keitimas į kitą vartotojo pašto dėžutę, o ne į aplanko turinio pašto dėžutę, dėl kurios kyla problemų</span><span class="sxs-lookup"><span data-stu-id="833f0-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="833f0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="833f0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="833f0-109">Palaukite valandą, iš naujo paleiskite "Outlook" klientą</span><span class="sxs-lookup"><span data-stu-id="833f0-109">Wait for an hour, restart outlook client</span></span>