---
title: 902 (Sinchronizavimo klaidos dėl pasikartojančių objektų)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767141"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="4b61c-102">Sinchronizavimo klaidos dėl pasikartojančių objektų</span><span class="sxs-lookup"><span data-stu-id="4b61c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="4b61c-103">Galite gauti vieną iš šių klaidos pranešimų, kai katalogų sinchronizavimas baigiamas "Microsoft 365":</span><span class="sxs-lookup"><span data-stu-id="4b61c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="4b61c-104">Microsoft Online Services šio objekto atnaujinti negalima, nes šie atributai, susiję su šiuo objektu, turi reikšmes, kurios jau gali būti susietos su kitu objektu vietiniame kataloge.</span><span class="sxs-lookup"><span data-stu-id="4b61c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="4b61c-105">Sinchronizuotas objektas su tuo pačiu tarpinio serverio adresu jau yra jūsų Microsoft Online Services kataloge.</span><span class="sxs-lookup"><span data-stu-id="4b61c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="4b61c-106">Neįmanoma atnaujinti šio objekto, nes šie atributai, susiję su šiuo objektu, turi reikšmes, kurios jau gali būti susietos su kitu objektu jūsų vietinio katalogo tarnybose: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4b61c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="4b61c-107">Norėdami nustatyti ir išspręsti problemą, atsisiųskite ir paleiskite [IdFix DirSync klaidų taisymo įrankį](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="4b61c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="4b61c-108">Daugiau informacijos ieškokite [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="4b61c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
