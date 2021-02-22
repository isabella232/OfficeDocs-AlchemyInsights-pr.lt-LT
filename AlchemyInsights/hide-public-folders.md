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
# <a name="hide-public-folders"></a>Slėpti viešuosius aplankus

**Norėdami paslėpti visą viešąjį aplanką medis**:

Atlikite [šiame](https://aka.ms/ControlPF) straipsnyje nurodytus veiksmus, kad paslėptumėte visą viešąjį aplankų medį nuo pasirinktinio arba visų vartotojų.

**Norėdami paslėpti konkretų viešąjį aplanką**:

1. Vartotojų, kuriems reikia prieigos prie viešojo aplanko, teisių įtraukimas

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Pašalinkite vartotojo **numatytąjį** **teisių** sąrašą:

    `Remove-PublicFolderClientPermission \test1 -User Default`
