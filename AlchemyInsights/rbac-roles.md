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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583946"
---
# <a name="rbac-rules"></a>RBAC taisyklės

Jei gaunate teisių klaidą: 

- **Klientas su objekto ID neturi leidimo atlikti veiksmą per aprėptį (kodas: autorizacija nepavyko)**: kai bandote sukurti išteklių, patikrinkite, ar šiuo metu esate prisijungę su vartotoju, kuriam priskirtas tam tikrą vaidmenį turintis vartotojas, kuriam buvo suteikta teisė naudoti išteklius pasirinktoje srityje. Pavyzdžiui, norėdami valdyti virtualiąsias mašinas išteklių grupėje, turite turėti [virtualiosios mašinos bendraautoriaus](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) vaidmenį išteklių grupėje (arba pirminėje aprėptyje). Kiekvieno įtaisytojo vaidmens teisių sąrašo ieškokite [Įtaisytieji "Azure" išteklių vaidmenys](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Neturite **teisės sukurti palaikymo užklausos**: kai bandote sukurti arba atnaujinti palaikymo bilietą, patikrinkite, ar šiuo metu esate prisijungę naudodami vartotoją, kuriam priskirtas "Microsoft". support/Paramttickets/rašyti teises, pvz., [palaikymo užklausos bendraautorius](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Negalima **kurti daugiau vaidmenų priskyrimų (kodas: Roleassigmentlimitviršyta)**: kai bandote priskirti vaidmenį, pabandykite sumažinti vaidmenų priskyrimų skaičių priskirdami vaidmenis grupėms, o ne. "Azure" palaiko iki **2000** vaidmenų priskyrimus per produktų paketą.

Daugiau informacijos apie "Azure RBAC" vaidmenis ieškokite " [AZURE RBAC" vaidmenys](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
