---
title: Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826099"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos

Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategiją, rodomas toks klaidos pranešimas:

*HandleError : nepavyko gauti produkto strategijos su PolicyId 'AllowSelfServicePurchase', ErrorMessage – pagrindinis ryšys buvo uždarytas: siunčiant įvyko netikėta klaida.*

Taip gali būti dėl senesnės transportavimo lygmens saugos (TLS) versijos. Norėdami prijungti MSCommerce tarnybą, turite naudoti TLS 1.2 arba didesnę.  

Pabandykite atlikti šiuos veiksmus, kad įgalintumėte / nustatykite TLS protokolą kaip 1.2, patikrinkite ir bandykite dar kartą.
 1. "PowerShell" komandinėje eilutėje (PS C: įveskite šią komandą, kad \) TLS protokolą nustatytų kaip 1.2 versiją:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Patikrinkite, ar naudojamas (-i) TLS protokolas (-ai), naudodami šią komandą:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Iš naujo bandykite komandas Gauti arba Naujinti, jei reikia.

