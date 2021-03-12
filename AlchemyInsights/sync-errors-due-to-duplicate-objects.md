---
title: 902 (Sinchronizavimo klaidos dėl pasikartojančių objektų)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708070"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d9cb1-102">Sinchronizavimo klaidos dėl pasikartojančių objektų</span><span class="sxs-lookup"><span data-stu-id="d9cb1-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d9cb1-103">Galite gauti vieną iš šių klaidos žinučių, kai katalogų sinchronizavimas yra "Microsoft 365":</span><span class="sxs-lookup"><span data-stu-id="d9cb1-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="d9cb1-104">Negalima atnaujinti šio objekto "Microsoft Online Services", nes toliau nurodyti atributai, susiję su šiuo objektu, turi reikšmes, kurios gali būti jau susietos su kitu objektu jūsų vietiniame kataloge.</span><span class="sxs-lookup"><span data-stu-id="d9cb1-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="d9cb1-105">Sinchronizuotas objektas su tuo pačiu tarpinio serverio adresu jau yra jūsų "Microsoft Online Services" kataloge.</span><span class="sxs-lookup"><span data-stu-id="d9cb1-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="d9cb1-106">Negalima naujinti šio objekto, nes toliau nurodyti atributai, susiję su šiuo objektu, turi reikšmes, kurios gali būti jau susietos su kitu objektu jūsų vietinio katalogo tarnybose: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="d9cb1-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="d9cb1-107">Norėdami nustatyti ir išspręsti šią problemą, atsisiųskite ir paleiskite " [IDFix DirSync" klaidų taisymo įrankį](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="d9cb1-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="d9cb1-108">Daugiau informacijos ieškokite [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="d9cb1-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
