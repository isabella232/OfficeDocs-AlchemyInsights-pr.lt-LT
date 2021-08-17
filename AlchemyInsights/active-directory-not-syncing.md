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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889226"
---
# <a name="active-directory-not-syncing"></a>"Active Directory" nesinchronizuojama

Jei gaunate sinchronizavimo klaidų, pvz., "nėra naujausio sinchronizavimo", arba pastebėjote katalogų sinchronizavimo būseną "Office" administravimo portale sako: "Paskutinį kartą sinchronizuota daugiau nei prieš 3 dienas", gali būti, kad "AADConnect" turi neteisingus parametrus arba nepakanka teisių sinchronizuoti.  

"AADConnect" diegimas iš naujo naudojant skubius parametrus gali greitai išspręsti šią problemą:

1. [Atsisiųskite naujausią "AADConnect" versiją.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Vykdykite nurodymus, kaip atlikti skubią įdiegtį.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

„Azure AD Connect“ turi būti diegiama „Windows Server 2012“ arba naujesnėje versijoje. Šis serveris turi būti prijungtas prie domeno ir gali būti domeno valdiklis arba nario serveris. Jei reikia viso "Azure AD" Prisijungimas reikalavimų ir išankstinių sąlygų, [peržiūrėkite Būtinosios "Azure AD" Prisijungimas.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Daugiau informacijos apie "AADConnect" tarnybos paskyras žr. ["Azure AD Prisijungimas: Paskyros ir teisės](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
