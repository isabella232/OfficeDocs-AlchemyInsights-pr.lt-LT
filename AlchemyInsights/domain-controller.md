---
title: Domeno valdiklis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901028"
---
# <a name="domain-controller"></a>Domeno valdiklis

**Nepavyksta įjungti "AAD" arba diegimo.**

Jei norite išspręsti "Azure AD" domenų tarnybos (AAD – DS) problemą, kuri neįgalinta arba nepavyksta įdiegti, atlikite šiuos veiksmus:

1. Jei naudojate jau esamą virtualiojo tinklo, patikrinkite savo NSG taisykles, kurios blokuoja prievadus, reikalingus sinchronizuoti naudojant "AAD-DS" portale https://aka.ms/aadds-networking .
2. Patikrinkite, ar jūsų klaidos pranešimas atsakomas šiame trikčių diagnostikos vadove, kuris pasiekiamas  https://aka.ms/aadds-troubleshoot-enable .
3. Pabandykite diegti "Azure AD" domenų tarnybas naujame virtualiame tinkle.
4. Vadovaukitės darbo pradžios vadovu, kaip įdiegti "AAD-DS", kurį galima naudoti [mokymo programoje "AZURE AD" domenų paslaugoms kurti](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jei kyla problemų diegiant "Azure AD" domenų tarnybas, peržiūrėkite " [AZURE AD" domenų tarnybų trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kad būtų išspręstos Dažniausios klaidos, padedančios gauti darbą dar kartą. 

**Negalima išjungti AAD – DS**

AAD – DS negali būti pristabdytas. Jei nebenorite naudoti valdomo domeno, jį reikia naikinti.

Jei susidūrėte su problemomis, Norėdami išspręsti dažnai pasitaikančių klaidų ir susijusių trikčių šalinimo veiksmus, kad galėtumėte vėl atlikti veiksmus, skaitykite " [Azure Active Directory" domenų tarnybos trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
