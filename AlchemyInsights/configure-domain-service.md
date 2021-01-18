---
title: Domeno paslaugos konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885694"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nepavyksta įjungti "AAD" arba diegimo.

Jei norite išspręsti "Azure AD" domenų tarnybos (AAD – DS) problemą, kuri neįgalinta arba nepavyksta įdiegti, atlikite šiuos veiksmus:

1. Jei naudojate jau esamą virtualiojo tinklo, patikrinkite savo NSG taisykles, kurios blokuoja prievadus, reikalingus sinchronizuoti naudojant "AAD-DS" portale https://aka.ms/aadds-networking .
2. Patikrinkite, ar jūsų klaidos pranešimas atsakomas šiame trikčių diagnostikos vadove, kuris pasiekiamas  https://aka.ms/aadds-troubleshoot-enable .
3. Pabandykite diegti "Azure AD" domenų tarnybas naujame virtualiame tinkle.
4. Vadovaukitės darbo pradžios vadovu, kaip įdiegti "AAD-DS": [kurti ir KONFIGŪRUOTI AAD domenų tarnybas](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Jei kyla problemų diegiant "Azure AD" domenų tarnybas, peržiūrėkite " [AZURE AD" domenų tarnybų trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kad būtų išspręstos Dažniausios klaidos, padedančios gauti darbą dar kartą. 

**Negalima išjungti AAD – DS**

AAD – DS negali būti pristabdytas. Jei nebenorite naudoti valdomo domeno, jį reikia naikinti.
Norėdami panaikinti valdomą domeną, žiūrėkite [Naikinti AAD domenų tarnybą](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



