---
title: Klaida AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709159"
---
# <a name="error-attributevaluemustbeunique"></a>Klaida: AttributeValueMustBeUnique

Dažniausia "AttributeValueMustBeUnique" klaidos priežastis yra du objektai su skirtingais SourceAnchor (immutableId) turi tą pačią reikšmę ProxyAddresses ir (arba) UserPrincipalName atributus. Norėdami pataisyti "AttributeValueMustBeUnique" klaidą:
  
1. Identifikuokite pasikartojančius proxyAddresses, userPrincipalName arba kitą atributo reikšmę, dėl kurios kyla klaida. Taip pat nustatykite, kurie du (ar daugiau) objektai yra susiję su konfliktu. Ataskaita, kurią sugeneravo "Azure AD Connect Health for Sync", gali padėti nustatyti du objektus.
    
2. Nustatykite, kuris objektas turėtų būti ir toliau dubliuojamas, o kuris objektas neturėtų.
    
3. Pašalinkite dubliuotos reikšmės objektą, kurio reikšmė neturėtų būti. Nepamirškite, kad pakeiskite katalogą, kuriame yra objektas. Kai kuriais atvejais gali reikėti panaikinti vieną iš konflikto objektų.
    
4. Jei pakeitėte vietinį skelbimą, paleiskite "Azure AD Connect" sinchronizavimo keitimą, kad būtų išspręsta klaida.
    

