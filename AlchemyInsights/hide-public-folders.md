---
title: Slėpti viešuosius aplankus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315433"
---
# <a name="hide-public-folders"></a><span data-ttu-id="67bc3-102">Slėpti viešuosius aplankus</span><span class="sxs-lookup"><span data-stu-id="67bc3-102">Hide public folders</span></span>

<span data-ttu-id="67bc3-103">**Norėdami paslėpti visą viešąjį aplanką medis**:</span><span class="sxs-lookup"><span data-stu-id="67bc3-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="67bc3-104">Atlikite [šiame](https://aka.ms/ControlPF) straipsnyje nurodytus veiksmus, kad paslėptumėte visą viešąjį aplankų medį nuo pasirinktinio arba visų vartotojų.</span><span class="sxs-lookup"><span data-stu-id="67bc3-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="67bc3-105">**Norėdami paslėpti konkretų viešąjį aplanką**:</span><span class="sxs-lookup"><span data-stu-id="67bc3-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="67bc3-106">Vartotojų, kuriems reikia prieigos prie viešojo aplanko, teisių įtraukimas</span><span class="sxs-lookup"><span data-stu-id="67bc3-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="67bc3-107">Pašalinkite vartotojo **numatytąjį** **teisių** sąrašą:</span><span class="sxs-lookup"><span data-stu-id="67bc3-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
