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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020200"
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

