---
title: Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735207"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos

Kai bandote nustatyti arba peržiūrėti AllowSelfServicePurchase strategiją, gaunate šį klaidos pranešimą:

*HandleError: nepavyko gauti produkto strategijos su strategijos ID "AllowSelfServicePurchase", ErrorMessage – esamas prisijungimas buvo uždarytas: įvyko netikėta klaida siunčiant.*

Taip gali būti dėl senesnės transportavimo lygmens saugos (TLS) versijos. Norėdami prijungti MSCommerce paslaugą, turite naudoti TLS 1,2 arba daugiau.  

Pabandykite atlikti toliau nurodytus veiksmus, kad įgalintumėte/nustatytumėte TLS protokolą iki 1,2, patikrinti ir bandyti dar kartą.
 1. "PowerShell" komandų eilutėje (PS C: \) įvesti šią komandą, kad TLS protokolas būtų nustatytas į 1,2 versiją:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Patikrinkite naudojamą TLS protokolą (-us), naudodami šią komandą:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Jei reikia, iš naujo bandykite gauti arba atnaujinti komandas.

