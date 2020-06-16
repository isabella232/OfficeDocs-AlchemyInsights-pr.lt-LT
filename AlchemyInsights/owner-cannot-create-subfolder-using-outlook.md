---
title: Savininkas negali sukurti poaplankio naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749138"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="8dcea-102">Savininkas negali sukurti poaplankio naudodamas "Outlook"</span><span class="sxs-lookup"><span data-stu-id="8dcea-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="8dcea-103">**Yra problema su viešųjų aplankų savininkai sukurti poaplankius naudojant "Outlook". Problema bus išspręsta netrukus.**</span><span class="sxs-lookup"><span data-stu-id="8dcea-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="8dcea-104">Tuo tarpu, naudokite vieną iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="8dcea-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="8dcea-105">Naudokite "Outlook", skirta MAC sukurti poaplankį, kaip problema turi įtakos tik "Outlook", skirta darbalaukio windows (visos versijos)</span><span class="sxs-lookup"><span data-stu-id="8dcea-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="8dcea-106">Ar administratorius sukurti poaplankį naudojant EXO Shell arba EAC</span><span class="sxs-lookup"><span data-stu-id="8dcea-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="8dcea-107">Pakeisti DefaultPublicFolderMailbox/EffectivePublicFolderMailbox vartotojo į kitą pašto dėžutę nei turinio pašto dėžutės aplanko sukelia problema</span><span class="sxs-lookup"><span data-stu-id="8dcea-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="8dcea-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="8dcea-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="8dcea-109">Palaukite valandą, iš naujo paleiskite "Outlook" kliento</span><span class="sxs-lookup"><span data-stu-id="8dcea-109">Wait for an hour, restart outlook client</span></span>