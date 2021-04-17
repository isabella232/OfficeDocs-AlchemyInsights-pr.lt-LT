---
title: "\"Active Directory\" nesinchronizuojama"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822859"
---
# <a name="active-directory-not-syncing"></a>"Active Directory" nesinchronizuojama

Jei gaunate sinchronizavimo klaidų, pvz., "nėra naujausio sinchronizavimo", arba pastebėjote katalogų sinchronizavimo būseną "Office" administravimo portale sako: "Paskutinį kartą sinchronizuota daugiau nei prieš 3 dienas", gali būti, kad "AADConnect" turi neteisingus parametrus arba nepakanka teisių sinchronizuoti.  

"AADConnect" diegimas iš naujo naudojant skubius parametrus gali greitai išspręsti šią problemą:

1. [Atsisiųskite naujausią "AADConnect" versiją.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Vykdykite nurodymus, kaip atlikti skubią įdiegtį.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Daugiau informacijos apie "AADConnect" tarnybos paskyras žr. ["Azure AD Connect": paskyros ir teisės](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
