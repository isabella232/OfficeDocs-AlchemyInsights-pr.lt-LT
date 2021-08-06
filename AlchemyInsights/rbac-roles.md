---
title: 'RBAC vaidmenys '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923139"
---
# <a name="rbac-rules"></a>RBAC taisyklės

Jei gaunate teisių klaidą: 

- Klientas, kurio objekto ID, neturi teisės atlikti veiksmo aprėpties **(kodas: AuthorizationFailed):** kai bandote sukurti išteklių, patikrinkite, ar šiuo metu esate prisijungę su vartotojui, kuriam priskirtas vaidmuo, kuriam priskirtos rašymo teisės į išteklius pasirinktoje aprėgoje. Pvz., norėdami valdyti virtualias mašinas išteklių grupėje, turėtumėte turėti vaidmenį [Virtualiosios mašinos bendraautorių](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) išteklių grupėje (arba pirminės aprėpties). Kiekvieno įtaisytųjų vaidmenų teisių sąrašą žr. Įtaisytieji ["Azure"](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)išteklių vaidmenys .
- **Neturite teisės kurti** palaikymo užklausos: kai bandote sukurti arba atnaujinti palaikymo kvitą, patikrinkite, ar šiuo metu esate prisijungę naudodami vartotoją, kuriam priskirtas vaidmuo, kuris turi "Microsoft.Support" / "supportTickets" / rašymo teises, pvz., palaikymo užklausos bendraautorių . [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Daugiau negalima kurti vaidmenų priskyrimų **(kodas: RoleAssignmentLimitExceeded)**: kai bandote priskirti vaidmenį, pabandykite sumažinti vaidmenų priskyrimų skaičių priskirdami vaidmenis grupėms. "Azure" palaiko **iki 2 000 vaidmenų** priskyrimų vienai prenumeratai.

Daugiau informacijos apie "Azure RBAC" vaidmenis žr. ["Azure RBAC" vaidmenys](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
