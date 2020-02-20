---
title: Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158569"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos

Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategija, galite gauti tokį klaidos pranešimą:

*HandleError: nepavyko gauti produkto politikos su PolicyId "AllowSelfServicePurchase", ErrorMessage-pagrindinis ryšys buvo uždarytas: siuntimo metu įvyko netikėta klaida.*

Taip gali būti dėl senesnės versijos transportavimo lygmens saugos (TLS). Norėdami prisijungti prie MSCommerce paslaugos, turite naudoti TLS 1,2 arba didesnis.  

Pabandykite šiuos veiksmus, Norėdami įjungti/nustatyti TLS protokolo 1,2, patikrinti, ir bandykite dar kartą.
 1. "PowerShell" komandinėje eilutėje (PS C\) : įveskite šią komandą, kad TLS protokolo versija 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Patikrinkite, ar TLS protokolo (-ų) naudojimo, su šia komanda:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Bandykite kartoti komandas gauti arba naujinti, jei reikia.

