---
title: Administratoriaus sutikimo problemos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901518"
---
# <a name="admin-consent-issues"></a>Administratoriaus sutikimo problemos

1. Įgalinkite [administratoriaus sutikimo darbo eigą](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , kad vartotojai galėtų prašyti Administratoriaus patvirtinimo tiesiogiai iš sutikimo ekrano.

1. Jei jūs arba jūsų taikomosios programos vartotojai sutikime įvyksta netikėtų klaidų, skaitykite šį straipsnį, kaip atlikti trikčių diagnostikos veiksmus: [netikėta klaida gavus sutikimą su programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Sužinokite daugiau apie [administratoriaus sutikimą "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kaip veikia [sutikimo raginimas](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) ir kaip [įvertinti užklausą dėl nuomotojo masto administratoriaus sutikimo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Programos, kurios integruoja su "Microsoft" tapatybės platforma, pateikia leidimų modelį, kuris leidžia vartotojams ir administratoriams kontroliuoti, kaip galima pasiekti duomenis. Autorizacijos modelio diegimas buvo atnaujintas "Microsoft" tapatybės platformos galinio punkto ir pakeičiamas kaip taikomoji programa turi sąveikauti su "Microsoft" tapatybės platforma. Peržiūrėkite ["Microsoft" tapatybės platformos galinio punkto teises ir sutikimą](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) , kad galėtumėte peržiūrėti šio autorizavimo modelį, įskaitant aprėpčių, teisių ir sutikimo.