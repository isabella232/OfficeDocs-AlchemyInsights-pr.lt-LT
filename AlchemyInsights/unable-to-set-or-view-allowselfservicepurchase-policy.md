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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091734"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos

Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategija, galite gauti tokį klaidos pranešimą:

*HandleError: nepavyko gauti produkto politikos su PolicyId "AllowSelfServicePurchase", ErrorMessage-pagrindinis ryšys buvo uždarytas: siuntimo metu įvyko netikėta klaida.*

Taip gali būti dėl senesnės versijos transportavimo lygmens saugos (TLS). Norėdami prisijungti prie MSCommerce paslaugos, turite naudoti TLS 1,2 arba didesnis.  

Pabandykite šiuos veiksmus, Norėdami įjungti/nustatyti TLS protokolo 1,2, patikrinti, ir bandykite dar kartą.
 1. "PowerShell" komandinėje eilutėje (PS C\) : įveskite šią komandą, kad TLS protokolo versija 1,2:

    \[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12

2. Patikrinkite, ar TLS protokolo (-ų) naudojimo, su šia komanda:

    \[Net. ServicePointManager]:: SecurityProtocol 

3. Bandykite kartoti komandas gauti arba naujinti, jei reikia.

