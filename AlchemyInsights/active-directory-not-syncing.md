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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937109"
---
# <a name="active-directory-not-syncing"></a>"Active Directory" nesinchronizuojama

Jei gaunate sinchronizavimo klaidų, pvz., "nėra naujausio sinchronizavimo", arba pastebėjote katalogų sinchronizavimo būseną "Office" administravimo portale sako: "Paskutinį kartą sinchronizuota daugiau nei prieš 3 dienas", gali būti, kad "AADConnect" turi neteisingus parametrus arba nepakankamas teises atlikti sinchronizavimą.  

"AADConnect" diegimas iš naujo naudojant skubius parametrus gali greitai išspręsti šią problemą:

1. [Atsisiųskite naujausią "AADConnect" versiją.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Vykdykite nurodymus, kaip atlikti skubią įdiegtį.](/azure/active-directory/hybrid/how-to-connect-install-express)

„Azure AD Connect“ turi būti diegiama „Windows Server 2012“ arba naujesnėje versijoje. Šis serveris turi būti prijungtas prie domeno ir gali būti domeno valdiklis arba nario serveris. Visą "Azure AD" reikalavimų ir Prisijungimas sąrašą, peržiūrėkite [Būtinosios "Azure AD" Prisijungimas.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Daugiau informacijos apie "AADConnect" tarnybos paskyras žr. ["Azure AD Prisijungimas: Paskyros ir teisės](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
