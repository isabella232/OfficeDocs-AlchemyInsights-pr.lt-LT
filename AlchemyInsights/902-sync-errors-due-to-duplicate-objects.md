---
title: 902 (sinchronizavimo klaidų dėl pasikartojančių objektų)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481025"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="0039e-102">Sinchronizavimo klaidos dėl pasikartojančių objektų</span><span class="sxs-lookup"><span data-stu-id="0039e-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="0039e-103">Galite gauti vieną iš šių klaidos pranešimų kai katalogų sinchronizavimas bus:</span><span class="sxs-lookup"><span data-stu-id="0039e-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="0039e-104">Neįmanoma atnaujinti šio objekto Microsoft Online Services, nes šie atributai, susiję su šio objekto vertės, kuri jau gali būti susijusi su kito objekto vietos kataloge.</span><span class="sxs-lookup"><span data-stu-id="0039e-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="0039e-105">Sinchronizuoti objektą su pačiu tarpinio serverio adresas jau yra Microsoft Online Services Directory.</span><span class="sxs-lookup"><span data-stu-id="0039e-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="0039e-106">Neįmanoma atnaujinti šio objekto, nes šie atributai, susiję su šio objekto vertės, kuri jau gali būti susijusi su kito objekto jūsų vietinio katalogo tarnybose: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0039e-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="0039e-107">Norėdami identifikuoti ir išspręsti šią problemą, atsisiųskite ir paleiskite [IdFix DirSync klaidų taisymo įrankį](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="0039e-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="0039e-108">Norėdami gauti daugiau informacijos, žr [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="0039e-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

